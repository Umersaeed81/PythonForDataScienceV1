#  [Umer Saeed](https://www.linkedin.com/in/engumersaeed/)
Sr. RF Planning & Optimization Engineer<br>
BSc Telecommunications Engineering, School of Engineering<br>
MS Data Science, School of Business and Economics<br>
**University of Management & Technology**<br>
**Mobile:**     +923018412180<br>
**Email:**  umersaeed81@hotmail.com<br>
**Address:** Dream Gardens,Defence Road, Lahore<br>

# 2G Cell On Cluster BH

**Input Data**
- Following ***PRS Report*** use to prepare the **Cell On Cluster BH** data;
    - 2G Num Dem(Date and Time must be in different columns)
    - Cluster BH Report (Date and Time must be in different columns)
- Input File must be Following Formt;
    - .zip Format (csv Format)
    

**Reference Data Set**
   - Reference Data Set can be download from the following link;
       - [Cell Hourly Data Set](https://github.com/Umersaeed81/2G_NPM_NUM_Dem_Q2_2021/tree/main/AprKPIs)
       - [Cluster BH Data Set](https://github.com/Umersaeed81/KPI_Data_Set_For_Python_Scripts/blob/main/Quaterly%20Conformance%20Working.zip)

**Import required Libraries**


```python
import os
import zipfile
import pandas as pd
from glob import glob
import dask.dataframe as dd
```

**Set Working Path For Cell Houlry KPIs**


```python
working_directory = 'D:/DataSets/KPIs/2G_Num_Dem'
os.chdir(working_directory)
```

**Unzip the Cell Hourly Files**


```python
%%time
for file in os.listdir(working_directory):   # get the list of files
    if zipfile.is_zipfile(file): # if it is a zipfile, extract it
        with zipfile.ZipFile(file) as item: # treat the file as a zip
           item.extractall()  # extract it in the working directory
```

    Wall time: 25.3 s
    

**import Cell Hourly Data**


```python
%%time
cell = dd.read_csv('*.csv',\
                   skiprows=[0,1,2,3,4,5],\
                   skipfooter=1,
                    engine='python',\
                    na_values=['NIL','/0'],
                    parse_dates=["Date"],assume_missing=True)

#cell = cell.repartition(npartitions=cell.npartitions//100)
#cell= cell.compute()
#https://github.com/dask/dask/issues/1166
```

    Wall time: 124 ms
    

**Set Working Path For Cluster BH KPIs**


```python
folder_path = 'D:/DataSets/Conformance/Quaterly Conformance Working'
os.chdir(folder_path)
```

**Unzip the Cluster BH Files**


```python
%%time
for file in os.listdir(folder_path):   # get the list of files
    if zipfile.is_zipfile(file): # if it is a zipfile, extract it
        with zipfile.ZipFile(file) as item: # treat the file as a zip
           item.extractall()  # extract it in the working directory
```

    Wall time: 47.6 ms
    

**Import Cluster BH KPIs**


```python
busy_hour_files = sorted(glob('Umer Saeed_Cluster_BH*.csv'))
# concat all the Cluster DA Files
cluster=pd.concat((pd.read_csv(file,skiprows=[0,1,2,3,4],\
                           skipfooter=1,engine='python',\
                           usecols=['Date','Time','GCell Group'],\
                           parse_dates=["Date"]) for file in busy_hour_files)).sort_values('Date')

cluster=cluster.rename(columns={"GCell Group":"Location"})
```

**Cell On Cluster BH**


```python
%%time
ccbh = dd.merge(cell,cluster,on=['Date','Time','Location'])
ccbh = ccbh.compute()
```

    Wall time: 8min 28s
    

**Remove Duplicates**


```python
ccbh = ccbh.drop_duplicates()
```

**Output**


```python
working_directory = 'D:/DataSets/KPIs/2G_Num_Dem/Output'
os.chdir(working_directory)
for f in os.listdir(working_directory):
    os.remove(os.path.join(working_directory, f))

for i, g in ccbh.groupby('Location'):
    g.to_csv('Loc_{}.csv'.format(i), header=True,index=False)
```

**Delete unzip Files**


```python
working_directory = 'D:/DataSets/KPIs/2G_Num_Dem'
os.chdir(working_directory)

for filename in os.listdir(working_directory):
    if filename.endswith('.csv'):
        os.unlink(os.path.join(working_directory, filename))

folder_path = 'D:/DataSets/Conformance/Quaterly Conformance Working'
os.chdir(folder_path)

for filename in os.listdir(folder_path):
    if filename.endswith('.csv'):
        os.unlink(os.path.join(folder_path, filename))        
```
