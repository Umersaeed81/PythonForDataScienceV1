# Chapter 12: General Operations on Pandas Data Frames

**Import Required Libraries**


```python
import os
import numpy as np
import pandas as pd
```

**Set Working Directory**


```python
working_directory = 'E:/Python_For_DS_V2/Chapter12'
os.chdir(working_directory)
```

## 12.1 Head

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.head.html)
- This function returns the first n rows for the object based on position.
- It is useful for quickly testing if your object has the right type of data in it.

**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.head()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>14905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>2</th>
      <td>HDIKBSC02</td>
      <td>6939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>2</td>
      <td>16939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>16939</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>3</th>
      <td>HDIKBSC02</td>
      <td>6939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>3</td>
      <td>26939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>26939</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>4</th>
      <td>HDIKBSC02</td>
      <td>6939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>4</td>
      <td>36939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>36939</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.head(n=2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>14905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.head(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>14905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 34 columns</p>
</div>



## 12.2 Tail 

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.tail.html#:~:text=Return%20the%20last%20n%20rows,after%20sorting%20or%20appending%20rows.)
- Return the last n rows.

**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.tail()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>11691</th>
      <td>HKNWBSC02</td>
      <td>CII-2553_Chak No 141 M Bahawalnagar Sahiwal (3...</td>
      <td>201</td>
      <td>CII-2553-2_Chak No 141 M Bahawalnagar Sahiwal ...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>22553</td>
      <td>5</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11692</th>
      <td>HKNWBSC02</td>
      <td>CII-2553_Chak No 141 M Bahawalnagar Sahiwal (3...</td>
      <td>202</td>
      <td>CII-2553-3_Chak No 141 M Bahawalnagar Sahiwal ...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>32553</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11693</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>229</td>
      <td>CII-2560-1_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>12560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11694</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>249</td>
      <td>CII-2560-2_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>22560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11695</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>253</td>
      <td>CII-2560-3_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>32560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>5 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.tail(n=2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>11694</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>249</td>
      <td>CII-2560-2_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>22560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11695</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>253</td>
      <td>CII-2560-3_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>32560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.tail(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>11694</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>249</td>
      <td>CII-2560-2_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>22560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11695</th>
      <td>HKNWBSC02</td>
      <td>CII-2560_Din Pur Khanewal (3G-CII-4423)</td>
      <td>253</td>
      <td>CII-2560-3_Din Pur Khanewal (3G-CII-4423)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>32560</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 34 columns</p>
</div>



## 12.3 Sample

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.sample.html)
- Return a random sample of items from an axis of object.

**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample()
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>6804</th>
      <td>HBWPBSC03</td>
      <td>4176_Moza Sui Wala Samma Satta Lodhran</td>
      <td>69</td>
      <td>14176_Moza Sui Wala Samma Satta Lodhran</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>54437</td>
      <td>14176</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>1 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(n=3)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2133</th>
      <td>HLHRBSC09</td>
      <td>CI-1611_Tariq Road Near Airport Lahore-Z2 (3G-...</td>
      <td>302</td>
      <td>CI-1611-3_Tariq Road Near Airport Lahore-Z2 (3...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57705</td>
      <td>31611</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>DEACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>9134</th>
      <td>HMLTBSC05</td>
      <td>4122_Bosan Road Multan (3G-CII-3128)</td>
      <td>120</td>
      <td>34122_Bosan Road Multan (3G-CII-3128)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54402</td>
      <td>34122</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>3426</th>
      <td>HHFZBSC01</td>
      <td>3803_Pindi Bhattian Sargodha (3G-CI-2132)</td>
      <td>75</td>
      <td>33803_Pindi Bhattian Sargodha (3G-CI-2132)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53330</td>
      <td>33803</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>3 rows × 34 columns</p>
</div>



**Example**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(3)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>1359</th>
      <td>HGJWBSC04</td>
      <td>3371_Haji Street Kamonki Gujranwala (3G-CI-4921)</td>
      <td>11</td>
      <td>33371_Haji Street Kamonki Gujranwala (3G-CI-4921)</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>53340</td>
      <td>33371</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11595</th>
      <td>HKNWBSC02</td>
      <td>4550_Zamir Colony Kassowal Sahiwal (3G-CII-4422)</td>
      <td>64</td>
      <td>24550_Zamir Colony Kassowal Sahiwal (3G-CII-4422)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>24550</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>1</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11444</th>
      <td>HBRWBSC03</td>
      <td>4574_Gulshan e Ghani Colony Vehari (3G-CII-3521)</td>
      <td>30</td>
      <td>34574_Gulshan e Ghani Colony Vehari (3G-CII-3521)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54456</td>
      <td>34574</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>3 rows × 34 columns</p>
</div>



### 12.3.1 random_state 

- Extract 3 random elements from the Data Frame: Note that we use ```random_state``` to ensure the reproducibility of the examples.


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(n=3, random_state=1)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2897</th>
      <td>HMWLBSC03</td>
      <td>4309_Skaseer (Gold) Mianwali (3G-CII-3827)</td>
      <td>32</td>
      <td>34309_Skaseer (Gold) Mianwali (3G-CII-3827)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54407</td>
      <td>34309</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5465</th>
      <td>HFSDBSC07</td>
      <td>CII-2190_Chak No 78 GB Jawddi Faisalabad-Z2</td>
      <td>174</td>
      <td>CII-2190-2_Chak No 78 GB Jawddi Faisalabad-Z2</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54404</td>
      <td>22190</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>6811</th>
      <td>HBWPBSC03</td>
      <td>5572_Jalapur Pirwala Multan</td>
      <td>79</td>
      <td>25572_Jalapur Pirwala Multan</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>54437</td>
      <td>25572</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>3 rows × 34 columns</p>
</div>



### 12.3.2 fract


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(frac=0.001,random_state=1)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>2897</th>
      <td>HMWLBSC03</td>
      <td>4309_Skaseer (Gold) Mianwali (3G-CII-3827)</td>
      <td>32</td>
      <td>34309_Skaseer (Gold) Mianwali (3G-CII-3827)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54407</td>
      <td>34309</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5465</th>
      <td>HFSDBSC07</td>
      <td>CII-2190_Chak No 78 GB Jawddi Faisalabad-Z2</td>
      <td>174</td>
      <td>CII-2190-2_Chak No 78 GB Jawddi Faisalabad-Z2</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54404</td>
      <td>22190</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>6811</th>
      <td>HBWPBSC03</td>
      <td>5572_Jalapur Pirwala Multan</td>
      <td>79</td>
      <td>25572_Jalapur Pirwala Multan</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>54437</td>
      <td>25572</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>4288</th>
      <td>HLHRBSC08</td>
      <td>7069_Chamra Mandi Lahore-Z1 (3G-CI-4322)</td>
      <td>249</td>
      <td>37069_Chamra Mandi Lahore-Z1 (3G-CI-4322)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57704</td>
      <td>37069</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11384</th>
      <td>HHFZBSC02</td>
      <td>3780_Bugga Hafizabad</td>
      <td>111</td>
      <td>33780_Bugga Hafizabad</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53329</td>
      <td>33780</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5800</th>
      <td>HKASBSC03</td>
      <td>7621_Rehman Pura (Gold) Kasur (3G-CI-4983)</td>
      <td>88</td>
      <td>37621_Rehman Pura (Gold) Kasur (3G-CI-4983)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53309</td>
      <td>37621</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11654</th>
      <td>HKNWBSC02</td>
      <td>5501_Kot Islam Khanewal (3G-CII-4359)</td>
      <td>123</td>
      <td>35501_Kot Islam Khanewal (3G-CII-4359)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54436</td>
      <td>35501</td>
      <td>5</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5169</th>
      <td>HLHRBSC15</td>
      <td>7085_Salamat Pura Lahore-Z1 (3G-CI-4330)</td>
      <td>179</td>
      <td>37085_Salamat Pura Lahore-Z1 (3G-CI-4330)</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>57708</td>
      <td>37085</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5660</th>
      <td>HGJTBSC06</td>
      <td>3766_Wazirabad Sialkot (3G-CI-3925)</td>
      <td>260</td>
      <td>23766_Wazirabad Sialkot (3G-CI-3925)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53308</td>
      <td>23766</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>2717</th>
      <td>HFSDBSC06</td>
      <td>4035_Officer Colony Faisalabad-Z2 (3G-CII-3041)</td>
      <td>43</td>
      <td>24035_Officer Colony Faisalabad-Z2 (3G-CII-3041)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54424</td>
      <td>24035</td>
      <td>1</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>1</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>2391</th>
      <td>HLHRBSC11</td>
      <td>3542_Sheer e Rabbani Sheikhupura (3G-CI-3900)</td>
      <td>66</td>
      <td>33542_Sheer e Rabbani Sheikhupura (3G-CI-3900)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53316</td>
      <td>33542</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>6520</th>
      <td>HDIKBSC03</td>
      <td>4324_Imamia Road (Gold) DI Khan (3G-CII-3536)</td>
      <td>100</td>
      <td>24324_Imamia Road (Gold) DI Khan (3G-CII-3536)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54427</td>
      <td>24324</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>1</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>12 rows × 34 columns</p>
</div>



### 12.3.3 replace

- An upsample sample of the DataFrame with replacement: Note that ```replace``` parameter has to be True for frac parameter > 1.


```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(frac=1.5, replace=True,random_state=1)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>235</th>
      <td>HDIKBSC02</td>
      <td>5713_Muhalah Qazianwala Layyah (3G-CII-4151)</td>
      <td>272</td>
      <td>35713_Muhalah Qazianwala Layyah (3G-CII-4151)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>35713</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5192</th>
      <td>HLHRBSC15</td>
      <td>7088_PTCL Exchange Gulgasht Town Lahore-Z2 (3G...</td>
      <td>250</td>
      <td>27088_PTCL Exchange Gulgasht Town Lahore-Z2 (3...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57708</td>
      <td>27088</td>
      <td>5</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>1</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>905</th>
      <td>HLHRBSC14</td>
      <td>CI-1629_Rehman Plaza Queen Road Lahore-Z2 (3G-...</td>
      <td>179</td>
      <td>CI-1629-1_Rehman Plaza Queen Road Lahore-Z2 (3...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57702</td>
      <td>11629</td>
      <td>5</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>0</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>10955</th>
      <td>HGJWBSC03</td>
      <td>CI-1693_Sector Y Peoples Colony Gujranwala (3G...</td>
      <td>325</td>
      <td>CI-1693-3_Sector Y Peoples Colony Gujranwala (...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53303</td>
      <td>31693</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>7813</th>
      <td>HMLTBSC08</td>
      <td>5851_Vehari Road Multan (3G-CII-4039)</td>
      <td>242</td>
      <td>25851_Vehari Road Multan (3G-CII-4039)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54418</td>
      <td>25851</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>2748</th>
      <td>HFSDBSC06</td>
      <td>4079_Tech Society Faisalabad-Z2 (3G-CII-2000)</td>
      <td>74</td>
      <td>34079_Tech Society Faisalabad-Z2 (3G-CII-2000)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54424</td>
      <td>34079</td>
      <td>1</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>934</th>
      <td>HLHRBSC14</td>
      <td>7662_Mochi Gate Lahore-Z0 (3G-CI-1761)</td>
      <td>208</td>
      <td>37662_Mochi Gate Lahore-Z0 (3G-CI-1761)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57702</td>
      <td>37662</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>11011</th>
      <td>HGJTBSC04</td>
      <td>7870_Fateh Pur Gujrat (3G-CI-2191)</td>
      <td>39</td>
      <td>27870_Fateh Pur Gujrat (3G-CI-2191)</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>53313</td>
      <td>27870</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>7784</th>
      <td>HMLTBSC08</td>
      <td>4262_Chowk Metla Bahawalpur Road Vehari (3G-CI...</td>
      <td>213</td>
      <td>34262_Chowk Metla Bahawalpur Road Vehari (3G-C...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>51126</td>
      <td>34262</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1096</th>
      <td>HFSDBSC08</td>
      <td>4086_Pul Dhengro Sargodha Road Jhang</td>
      <td>63</td>
      <td>34086_Pul Dhengro Sargodha Road Jhang</td>
      <td>GSM900</td>
      <td>410</td>
      <td>3</td>
      <td>54423</td>
      <td>34086</td>
      <td>6</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>17544 rows × 34 columns</p>
</div>



### 12.3.4 weights

**Example-7**

- Using a DataFrame column as ```weights```. Rows with larger value in the num_specimen_seen column are more likely to be sampled.


```python
df = pd.DataFrame({'num_legs': [2, 4, 8, 0],
                   'num_wings': [2, 0, 0, 0],
                   'num_specimen_seen': [10, 2, 1, 8]},
                  index=['falcon', 'dog', 'spider', 'fish'])
df.sample(frac=0.5,replace=True,random_state=1, weights='num_specimen_seen')
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>num_legs</th>
      <th>num_wings</th>
      <th>num_specimen_seen</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>falcon</th>
      <td>2</td>
      <td>2</td>
      <td>10</td>
    </tr>
    <tr>
      <th>fish</th>
      <td>0</td>
      <td>0</td>
      <td>8</td>
    </tr>
  </tbody>
</table>
</div>




```python
df = pd.read_csv('GCELL.txt',header=1)
df.sample(frac=0.5,random_state=1, weights='Cell LAC')
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>4841</th>
      <td>HLHRBSC12</td>
      <td>CI-1383_Village karbath Lahore-Z2 (3G-CI-1798)</td>
      <td>165</td>
      <td>CI-1383-3_Village karbath Lahore-Z2 (3G-CI-1798)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57701</td>
      <td>31383</td>
      <td>1</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>8384</th>
      <td>HKNWBSC01</td>
      <td>6996_Kohiwala Khanewal (3G-CII-4074)</td>
      <td>51</td>
      <td>36996_Kohiwala Khanewal</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54421</td>
      <td>36996</td>
      <td>3</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HDIKBSC02</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>3531</th>
      <td>HSKTBSC04</td>
      <td>7876_Kotli Loharan (Gold) Sialkot (3G-CI-1071)</td>
      <td>145</td>
      <td>17876_Kotli Loharan (Gold) Sialkot (3G-CI-1071)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53331</td>
      <td>17876</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>0</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1709</th>
      <td>HSWLBSC03</td>
      <td>4672_Chak No 3 EB Pakpattan</td>
      <td>17</td>
      <td>34672_Chak No 3 EB Pakpattan</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54440</td>
      <td>34672</td>
      <td>1</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>...</th>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
      <td>...</td>
    </tr>
    <tr>
      <th>3968</th>
      <td>HLHRBSC10</td>
      <td>CI-1800_Johar block Bahria Town Lahore (3G-CI-...</td>
      <td>342</td>
      <td>CI-1800-3_Johar block Bahria Town Lahore (3G-C...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53311</td>
      <td>31800</td>
      <td>5</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>2</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5736</th>
      <td>HKASBSC03</td>
      <td>7616_Parnawa Kasur (3G-CI-3916)</td>
      <td>24</td>
      <td>17616_Parnawa Kasur (3G-CI-3916)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53309</td>
      <td>17616</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>83</th>
      <td>HDIKBSC02</td>
      <td>CII-2016_Mahala Shah Jahaniya Layyah (3G-CII-4...</td>
      <td>87</td>
      <td>CII-2016-1_Mahala Shah Jahaniya Layyah (3G-CII...</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>12016</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>5097</th>
      <td>HLHRBSC15</td>
      <td>CI-1135_Tajpura New Lahore-Z2 (3G-CI-1787)</td>
      <td>77</td>
      <td>CI-1135-3_Tajpura New Lahore-Z2 (3G-CI-1787)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>57708</td>
      <td>31135</td>
      <td>2</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>2554</th>
      <td>HLHRBSC11</td>
      <td>7676_Balarkay Sheikhupura (3G-CI-2167)</td>
      <td>229</td>
      <td>17676_Balarkay Sheikhupura (3G-CI-2167)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>53305</td>
      <td>17676</td>
      <td>4</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>5848 rows × 34 columns</p>
</div>



### 12.3.5 Random Sampling using skiprows


```python
df = pd.read_csv('GCELL.txt',header=1)
df.shape
```




    (11696, 34)




```python
df=pd.read_csv('GCELL.txt',header=1,skiprows=lambda x:x>0 and np.random.rand()>0.01)
df.shape
```




    (120, 34)



**How it works**

- ```skiprows``` accepts a function that is evaluated against integer index.
- ***x>0*** ensures that the header row is not skipped.
- ```np.random.rand()>0.01``` return ```True``` 99% of the time, thus skipping 99% of the rows.

## 12.4 Shape of the Data Frame

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.shape.html)
- Return a tuple representing the dimensionality of the DataFrame

**Example-1**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.shape
```




    (11696, 34)



**Example-2**


```python
df = pd.read_csv('GCELL.txt',header=1)
rows,columns=df.shape
print(rows,columns)
```

    11696 34
    

**Example-3**


```python
df = pd.read_csv('GCELL.txt',header=1)
rows,columns=df.shape
print("No of rows in the WHO Data Set:")
print(rows)
print("No of columns in the WHO Data Set:")
print(columns)
```

    No of rows in the WHO Data Set:
    11696
    No of columns in the WHO Data Set:
    34
    

## 12.5 Dimensions of the Data Frame

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.ndim.html)
- Return an int representing the number of axes / array dimensions.
- Return 1 if Series. Otherwise return 2 if DataFrame.

**Example-1**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.ndim
```




    2



**Example-2**


```python
df = pd.Series({'a': 1, 'b': 2, 'c': 3})
df.ndim
```




    1



## 12.6 Size of the Data Frame

- [Reference URL](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.size.html)
- Number of elements in the array.

**Example-1**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.size
```




    397664



**Example-2**


```python
df = pd.Series({'a': 1, 'b': 2, 'c': 3})
df.size
```




    3



## 12.7 Get Variables Name of the Data Frame

### 12.7.1 columns

- The column labels of the DataFrame.


```python
df = pd.read_csv('GCELL.txt',header=1)
df.columns
```




    Index(['BSC Name', 'BTS Name', 'Cell Index', 'Cell Name', 'Freq. Band', 'MCC',
           'MNC', 'Cell LAC', 'Cell CI', 'NCC', 'BCC', 'Cell Extension Type',
           'Cell IUO Type', 'Enhanced Concentric Allowed',
           'Cell Inner/Extra Property', 'Same Group Cell Index',
           'BCCH IUO of Double Frequency Cell', 'Start Flex MAIO Switch',
           'HSN Modification Switch', 'CS Voice Service PRI',
           'CS Data Service PRI', 'PS High PRI Service PRI',
           'PS Low PRI Service PRI', 'Number of PBCCH Blocks',
           'Number of PAGCH Blocks', 'Number of PRACH Blocks', 'VIP Cell',
           'MOCN Sharing Cell', 'Support Dual High Frequency Bands',
           'Local Cell ID', 'Remark', 'Administrative State', 'active status',
           'Operator Name'],
          dtype='object')



### 12.7.2 keys

- Pandas dataframe.keys() function returns the ‘info axis’ for the pandas object. 
- If the pandas object is series then it returns index. 
- If the pandas object is dataframe then it returns columns.
- [Reference URL](https://www.geeksforgeeks.org/python-pandas-dataframe-keys/#:~:text=keys()%20function%20returns%20the,panel%20then%20it%20returns%20major_axis.)


```python
df = pd.read_csv('GCELL.txt',header=1)
df.keys()
```




    Index(['BSC Name', 'BTS Name', 'Cell Index', 'Cell Name', 'Freq. Band', 'MCC',
           'MNC', 'Cell LAC', 'Cell CI', 'NCC', 'BCC', 'Cell Extension Type',
           'Cell IUO Type', 'Enhanced Concentric Allowed',
           'Cell Inner/Extra Property', 'Same Group Cell Index',
           'BCCH IUO of Double Frequency Cell', 'Start Flex MAIO Switch',
           'HSN Modification Switch', 'CS Voice Service PRI',
           'CS Data Service PRI', 'PS High PRI Service PRI',
           'PS Low PRI Service PRI', 'Number of PBCCH Blocks',
           'Number of PAGCH Blocks', 'Number of PRACH Blocks', 'VIP Cell',
           'MOCN Sharing Cell', 'Support Dual High Frequency Bands',
           'Local Cell ID', 'Remark', 'Administrative State', 'active status',
           'Operator Name'],
          dtype='object')



## 12.8 Index of the Data Frame

- The index (row labels) of the DataFrame.


```python
df = pd.read_csv('GCELL.txt',header=1)
df.index
```




    RangeIndex(start=0, stop=11696, step=1)



## 12.9 axes of the Data Frame

- Return a list representing the axes of the DataFrame.
- It has the row axis labels and column axis labels as the only members.
- They are returned in that order.


```python
df = pd.read_csv('GCELL.txt',header=1)
df.axes
```




    [RangeIndex(start=0, stop=11696, step=1),
     Index(['BSC Name', 'BTS Name', 'Cell Index', 'Cell Name', 'Freq. Band', 'MCC',
            'MNC', 'Cell LAC', 'Cell CI', 'NCC', 'BCC', 'Cell Extension Type',
            'Cell IUO Type', 'Enhanced Concentric Allowed',
            'Cell Inner/Extra Property', 'Same Group Cell Index',
            'BCCH IUO of Double Frequency Cell', 'Start Flex MAIO Switch',
            'HSN Modification Switch', 'CS Voice Service PRI',
            'CS Data Service PRI', 'PS High PRI Service PRI',
            'PS Low PRI Service PRI', 'Number of PBCCH Blocks',
            'Number of PAGCH Blocks', 'Number of PRACH Blocks', 'VIP Cell',
            'MOCN Sharing Cell', 'Support Dual High Frequency Bands',
            'Local Cell ID', 'Remark', 'Administrative State', 'active status',
            'Operator Name'],
           dtype='object')]



## 12.10 Set Index to the specfic Column

- Set the DataFrame index (row labels) using one or more existing columns

**Example-1**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.set_index('BSC Name',inplace=True)
df.head(3)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Cell Name</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>BCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
    <tr>
      <th>BSC Name</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>HDIKBSC02</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>14905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>HDIKBSC02</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>HDIKBSC02</th>
      <td>6939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>2</td>
      <td>16939_Chak No 90 Mor Layyah (3G-CII-4281)</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>16939</td>
      <td>0</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>3 rows × 33 columns</p>
</div>



**Example-2**


```python
df = pd.read_csv('GCELL.txt',header=1)
df.set_index(['BSC Name','Cell Name'],inplace=True)
df.head(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>BCC</th>
      <th>Cell Extension Type</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
    <tr>
      <th>BSC Name</th>
      <th>Cell Name</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="2" valign="top">HDIKBSC02</th>
      <th>14905_Qazia Abad Layyah</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>0</td>
      <td>Normal_cell</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>24905_Qazia Abad Layyah</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>0</td>
      <td>Normal_cell</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 32 columns</p>
</div>



## 12.11 Re-Set Index


```python
df = pd.read_csv('GCELL.txt',header=1)
df.set_index(['BSC Name','Cell Name'],inplace=True)
df.head(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th></th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>BCC</th>
      <th>Cell Extension Type</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
    <tr>
      <th>BSC Name</th>
      <th>Cell Name</th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
      <th></th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th rowspan="2" valign="top">HDIKBSC02</th>
      <th>14905_Qazia Abad Layyah</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>0</td>
      <td>Normal_cell</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>24905_Qazia Abad Layyah</th>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>0</td>
      <td>Normal_cell</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 32 columns</p>
</div>




```python
df.reset_index(['BSC Name','Cell Name'],inplace=True)
df.head(2)
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>BSC Name</th>
      <th>Cell Name</th>
      <th>BTS Name</th>
      <th>Cell Index</th>
      <th>Freq. Band</th>
      <th>MCC</th>
      <th>MNC</th>
      <th>Cell LAC</th>
      <th>Cell CI</th>
      <th>NCC</th>
      <th>...</th>
      <th>Number of PAGCH Blocks</th>
      <th>Number of PRACH Blocks</th>
      <th>VIP Cell</th>
      <th>MOCN Sharing Cell</th>
      <th>Support Dual High Frequency Bands</th>
      <th>Local Cell ID</th>
      <th>Remark</th>
      <th>Administrative State</th>
      <th>active status</th>
      <th>Operator Name</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>HDIKBSC02</td>
      <td>14905_Qazia Abad Layyah</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>0</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>14905</td>
      <td>7</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
    <tr>
      <th>1</th>
      <td>HDIKBSC02</td>
      <td>24905_Qazia Abad Layyah</td>
      <td>4905_Qazia Abad Layyah</td>
      <td>1</td>
      <td>GSM900_DCS1800</td>
      <td>410</td>
      <td>3</td>
      <td>54438</td>
      <td>24905</td>
      <td>0</td>
      <td>...</td>
      <td>4</td>
      <td>1</td>
      <td>NO</td>
      <td>NO</td>
      <td>NO</td>
      <td>4294967295</td>
      <td>-</td>
      <td>UNLOCK</td>
      <td>ACTIVATED</td>
      <td>opname</td>
    </tr>
  </tbody>
</table>
<p>2 rows × 34 columns</p>
</div>



## 12.12 set_axis

- Assign desired index to given axis.
- Indexes for column or row labels can be changed by assigning a list-like or Index

**Example-1**


```python
df = pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6]})
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A</th>
      <th>B</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.set_axis(['a', 'b', 'c'], axis='rows', inplace=True)
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A</th>
      <th>B</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>a</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>b</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>c</th>
      <td>3</td>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>



**Example-2**


```python
df = pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6]})
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A</th>
      <th>B</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.set_axis(['A1', 'B1'], axis='columns', inplace=True)
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A1</th>
      <th>B1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>1</td>
      <td>4</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2</td>
      <td>5</td>
    </tr>
    <tr>
      <th>2</th>
      <td>3</td>
      <td>6</td>
    </tr>
  </tbody>
</table>
</div>



## 12.13 first_valid_index

- Return index for first ```non-NA/null``` value.


```python
df = pd.DataFrame({
                   "A1":[np.NaN,np.NaN,np.NaN,5,6,np.NaN,np.NaN], 
                   })
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>5.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>6.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>6</th>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.first_valid_index()
```




    3



## 12.14 last_valid_index

- Return index for last ```non-NA/null``` value.


```python
df = pd.DataFrame({
                   "A1":[np.NaN,np.NaN,np.NaN,5,6,np.NaN,np.NaN], 
                   })
df
```




<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>A1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>1</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>2</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>3</th>
      <td>5.0</td>
    </tr>
    <tr>
      <th>4</th>
      <td>6.0</td>
    </tr>
    <tr>
      <th>5</th>
      <td>NaN</td>
    </tr>
    <tr>
      <th>6</th>
      <td>NaN</td>
    </tr>
  </tbody>
</table>
</div>




```python
df.last_valid_index()
```




    4



## 12.15 Why do some pandas commands end with parentheses (and others don't)?

- [Reference Video](https://youtu.be/1dfn8JpwBL8)
