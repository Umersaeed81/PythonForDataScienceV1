<img src="https://github.com/Umersaeed81/PythonForDataScienceV0/blob/main/E1_V2.png" align="center" alt="Girl in a jacket" width="800" height="1000" align="center"/>

#  Preface

These notes were devloped for the course ***Python for Data Science*** at the [Center for Enterprise and Technology Advancement (CETA)](https://ceta.umt.edu.pk/) in [University of Management & Technology](www.umt.edu.pk). The goal is to provide an overiew of fundamental concepts in Python from first principles. I would like to  tanks [**Dr. Bilal Wajid**](https://www.linkedin.com/in/dr-bilal-wajid-98949276/) and [**Dr. Shahid Mahmood Awan**](https://uk.linkedin.com/in/shahidmawan) for their useful suggestions. I am also very grateful to all my class fellows for their feedback.
-                                                                                                                       [Umer Saeed](https://www.linkedin.com/in/engumersaeed/) 


 # Acknowledgments

I am deeply thankful to my advisors [**Dr. Shahid Mahmood Awan**](https://uk.linkedin.com/in/shahidmawan) and [**Dr. Bilal Wajid**](https://www.linkedin.com/in/dr-bilal-wajid-98949276/) for his inspiration and guidance throughout my studies at the [Department of Information System](https://sbe.umt.edu.pk/iss1/home.aspx), [School of Business and Economics](sbe.umt.edu.pk), [University of Management & Technology](www.umt.edu.pk). In the past 2 Years, his invaluable support and directions always helped me improve professional and academic skills. It has been an honor being his student.

I am very grateful to my friends [**Mr. Irfan Kareem**](https://www.linkedin.com/in/irfan-kareem-a89ba021/), [**Mr.Muneeb Ul Haque**](https://www.linkedin.com/in/muneeb-ul-haque-86551728/), [**Mr.Mansoor Waheed**](https://www.linkedin.com/in/mansoor-waheed-26925021/), [**Mr.Bilal Iqbal**](https://www.linkedin.com/in/bilal-iqbal-5354a324/) & [**Mr.AbdulRehman Azam**](https://www.linkedin.com/in/areh-azam/) for their friendship and help.


# <h1 align="center"> Table of contents

- ## [**Chapter 1: Introduction to Pandas**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html)

  - 1.1 [What is Data Science?](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1-What-is-Data-Science?)
     - 1.1.1 [Data Frames](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1.1-Data-Frames)
     - 1.1.2 [Characteristics of a Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1.2-Characteristics-of-a-Data-Frame)
     - 1.1.3 [Library Highlights](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1.3-Library-Highlights)
     - 1.1.4 [Pandas Documentation](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1.4-Pandas-Documentation)
     - 1.1.5 [Data Wrangling](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.1.5-Data-Wrangling)
  - 1.2 [Pandas Version](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.2-Pandas-Version)
     - 1.2.1 [Pandas Dependencies](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter1.html#1.2.1-Pandas-Dependencies)

- ## [**Chapter 2: Create Data Frame in Pandas**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html)

  - 2.1 [Create Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1-Create-Data-Frame)
    - 2.1.1 [Using Dictionary](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.1-Using-Dictionary)
    - 2.1.2 [Using Tuple](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.2-Using-Tuple)
    - 2.1.3 [Using ndarray](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.3-Using-ndarray)
    - 2.1.4 [Using List](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.4-Using-List)
    - 2.1.5 [Dictionary of Series](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.5-Dictionary-of-Series)
    - 2.1.6 [Using Random Number](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.6-Using-Random-Number)
    - 2.1.7 [Using Random Uniform Number](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.7-Using-Random-Uniform-Number)
    - 2.1.8 [Using Random randint Number](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.8-Using-Random-randint-Number)
    - 2.1.9 [empty Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter2.html#2.1.9-empty-Data-Frame)


- ## [**Chapter 3: Import Data Frame in Pandas From Local Clipboard**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter3.html)

  - 3.1 [How to read most commonly used file formats in Data Science (using Python/Pandas)?](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter3.html#3.1-How-to-read-most-commonly-used-file-formats-in-Data-Science-(using-Python/Pandas)?)
  - 3.2 [Local clipboard](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter3.html#3.2-Local-clipboard)

- ## [**Chapter 4: Import Data Frame in Pandas From CSV & Text Files**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html)
  - 4   [CSV & text files](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4-CSV-&-text-files)
  - 4.1 [read_table](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.1-read_table)
  - 4.2 [Define Header Row](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.2-Define-Header-Row)
    - 4.2.1 [Skip Row](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.2.1-Skip-Row)
    - 4.2.2 [Header Row](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.2.2-Header-Row)
    - 4.2.3 [Header set to None](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.2.3-Header-set-to-None)
    - 4.2.4 [Columns names](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.2.4-Columns-names)
  - 4.3 [rename columns](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.3-rename-columns)
    - 4.3.1 [Convert Header Name in lower Case](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.3.1-Convert-Header-Name-in-lower-Case)
    - 4.3.2 [Convert Header Name in upper Case](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.3.2-Convert-Header-Name-in-upper-Case)
    - 4.3.3 [Convert Header Name in Swapcase](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.3.3-Convert-Header-Name-in-Swapcase)
  - 4.4 [replace in column name](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.4-replace-in-column-name)
  - 4.5 [add_prefix in Header](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.5-add_prefix-in-Header)
  - 4.6 [add_suffix in Header](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.6-add_suffix-in-Header)
  - 4.7 [prefix](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.7-prefix)
  - 4.8 [Import Limited Number of Rows](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.8-Import-Limited-Number-of-Rows)
  - 4.9 [Import Limited Number of Columns](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.9-Import-Limited-Number-of-Columns)
  - 4.10 [skipfooter](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.10-skipfooter)
  - 4.11 [engine](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.11-engine)
  - 4.12 [Ignore Comments Lile](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.12-Ignore-Comments-Lile)
  - 4.13 [Sequency Of the Columns](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.13-Sequency-Of-the-Columns)
  - 4.14 [mangle_dupe_cols](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.14-mangle_dupe_cols)
  - 4.15 [skipinitialspace](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.15-skipinitialspace)
  - 4.16 [verbose](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.16-verbose)
  - 4.17 [converters](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.17-converters)
  - 4.18 [keep_default_na](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.18--keep_default_na)
  - 4.19 [true_values , false_value](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.19-true_values-,-false_value)
  - 4.20 [index_col](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.20-index_col)
  - 4.21 [thousands](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.21-thousands)
  - 4.22 [decimal](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.22-decimal)
  - 4.23 [squeeze](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.23-squeeze)
  - 4.24 [dtypes](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.24-dtypes)
    - 4.24.1 [dtype of a single Variable](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.24.1-dtype-of-a-single-Variable)
    - 4.24.2 [dtype of all the variables of the DataFrame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.24.2-dtype-of-all-the-variables-of-the-DataFrame)
    - 4.24.3 [set dtype during read_csv](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.24.3-set-dtype-during-read_csv)
  - 4.25 [parse_dates](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.25-parse_dates)
  - 4.26 [keep_date_col](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.26-keep_date_col)
  - 4.27 [na_values](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.27-na_values)
  - 4.28 [lineterminator](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter4.html#4.27-lineterminator)

- ## [**Chapter 5: Import Data Frame in Pandas From HTML**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter5.html)

  - 5.1 [Import csv File in Pandas From HTML](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter5.html#5.1-Import-csv-File-in-Pandas-From-HTML)
  - 5.2 [Import HTML Table](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter5.html#5.2-Import-HTML-Table)
  - 5.3 [Import HTML Table using attrs](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter5.html#5.3-Import-HTML-Table-using-attrs)
  - 5.4 [Import HTML Table using match](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter5.html#5.4-Import-HTML-Table-using-match)


- ## [**Chapter 6: Import Data Frame in Pandas From MS Excel**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html)

  - 6.1 [Import MS Excel File](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1-Import-MS-Excel-File)
    - 6.1.1 [sheet_name](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1.1-sheet_name)
    - 6.1.2 [Get all sheet names](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1.2-Get-all-sheet-names)
    - 6.1.3 [Import multiple Excel Sheets](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1.3-Import-multiple-Excel-Sheets)
    - 6.1.4 [Display all sheets](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1.4-Display-all-sheets)
    - 6.1.5 [converters](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter6.html#6.1.5-converters)

- ## [**Chapter 7: Import Data Frame in Pandas From Fixed-Width Text File**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter7.html)

  - 7.1 [Read Fixed-Width Text File](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter7.html#7.1-Read-Fixed-Width-Text-File)

- ## [**Chapter 8: Import Table From pdf file**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter8.html)
  - 8.1 [Install Tabula](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter8.html#8.1-Install-Tabula)
  - 8.2 [Read PDF FILE](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter8.html#8.2-Read-PDF-FILE)

- ## [**Chapter 9: Export Data Frame**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html)
  - 9.1 [Export Data Frame in CSV File](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1-Export-Data-Frame-in-CSV-File)
    - 9.1.1 [Export with Index Label](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.1-Export-with-Index-Label)
    - 9.1.2 [Export Without Index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.2-Export-Without-Index)
    - 9.1.3 [Export Specific Columns](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.3-Export-Specific-Columns)
    - 9.1.4 [Export Without Header](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.4-Export-Without-Header)
    - 9.1.5 [Export in .txt Format](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.5-Export-in-.txt-Format)
    - 9.1.6 [Export with specific sep](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.6-Export-with-specific-sep)
    - 9.1.7 [line_terminator](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.1.7-line_terminator)
  - 9.2 [Export Data Frame in Excel File](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2-Export-Data-Frame-in-Excel-File)
    - 9.2.1 [Sheet Name](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.1-Sheet-Name)
    - 9.2.2 [index_label](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.2-index_label)
    - 9.2.3 [Export without Index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.3-Export-without-Index)
    - 9.2.4 [startrow](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.4-startrow)
    - 9.2.5 [startcol](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.5-startcol)
    - 9.2.6 [Export multiple worksheets in the same workbook](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter9.html#9.2.6-Export-multiple-worksheets-in-the-same-workbook)

- ## [**Chapter 10: Convert the DataFrame to array**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html)
  - 10.1 [to_records](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.1-to_records)
    - 10.1.1 [Array with out Index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.1.1-Array-with-out-Index)
  - 10.2 [values](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.2-values)
  - 10.3 [to_numpy](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.3-to_numpy)
  - 10.4 [array](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.4-array)
  - 10.5 [to_list](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.5-to_list)
  - 10.6 [tolist](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.6-tolist)
  - 10.7 [explode](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter10.html#10.7-explode)
 
 - ## [**Chapter 11: Convert the DataFrame to array**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html)
  - 11.1 [to_dict](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html#11.1-to_dict)
    - 11.1.1 [series](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html#11.1.1-series)
    - 11.1.2 [split](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html#11.1.2-split)
    - 11.1.3 [index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html#11.1.3-index)
    - 11.1.4 [OrderedDict](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter11.html#11.1.4-OrderedDict)
  
- ## [**Chapter 12: General Operations on Pandas Data Frames**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html)
  - 12.1 [Head](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.1-Head)
  - 12.2 [Tail](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.2-Tail)
  - 12.3 [Sample](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.3-Sample)
  - 12.4 [Shape of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.4-Shape-of-the-Data-Frame)
  - 12.5 [Dimensions of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.5-Dimensions-of-the-Data-Frame)
  - 12.6 [Size of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.6-Size-of-the-Data-Frame)
  - 12.7 [Get Variables Name of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.7-Get-Variables-Name-of-the-Data-Frame)
    - 12.7.1 [columns](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.7.1-columns)
    - 12.7.2 [keys](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.7.2-keys)
  - 12.8 [Index of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.8-Index-of-the-Data-Frame)
  - 12.9 [axes of the Data Frame](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.9-axes-of-the-Data-Frame)
  - 12.10 [Set Index to the specfic Column](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.10-Set-Index-to-the-specfic-Column)
  - 12.11 [Re-Set Index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.11-Re-Set-Index)
  - 12.12 [set_axis](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.12-set_axis)
  - 12.13 [Why do some pandas commands end with parentheses (and others don't)?](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter12.html#12.13-Why-do-some-pandas-commands-end-with-parentheses-(and-others-don't)?)

- ## [**Chapter 13: General Operations on Pandas Data Frames**](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html)
  - 13.1 [dtypes](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.1-dtypes)
    - 13.1.1 [Check dtype of specific column](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.1.1-Check-dtype-of-specific-column)
    - 13.1.2 [value_counts](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.1.2-value_counts)
    - 13.1.3 [infer_objects](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.1.3-infer_objects)
  - 13.2 [Convert strings to numbers](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.2-Convert-strings-to-numbers)
  - 13.3 [to_datetime](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.3-to_datetime)
  - 13.4 [memory_usage](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.5-memory_usage)
    - 13.4.1 [memory_usage without Index](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.4.1-memory_usage-without-Index)
    - 13.4.2 [nbytes](https://htmlpreview.github.io/?https://github.com/Umersaeed81/PythonForDataScienceV1/blob/main/Chapter13.html#13.4.2-nbytes)


### Sponsers
<img src="https://upload.wikimedia.org/wikipedia/en/thumb/7/78/Higher_Education_Commission_of_Pakistan_%28logo%29.jpg/250px-Higher_Education_Commission_of_Pakistan_%28logo%29.jpg" align="left" alt="Girl in a jacket" width="100" height="100"> <img src="https://diceanalytics.pk/wp-content/uploads/2018/03/dice-logo.png" align="center" alt="Girl in a jacket" width="100" height="100"> <img src="https://e.jang.com.pk/jmimage_new/ejanglogo.png" align="left" alt="Girl in a jacket" width="100" height="100"> <img src="https://www.umt.edu.pk/style/images/umt-logo.jpg" align="left" alt="Girl in a jacket" width="250" height="100"> <img src="https://www.pnytrainings.com/assets/uploads//logo/1529168423-school-logo.jpg" align="left" alt="Girl in a jacket" width="100" height="100"> <img src="https://turnotech.com/wp-content/uploads/2020/01/logo-turnotech-color.png" align="left" alt="Girl in a jacket" width="250" height="100">

