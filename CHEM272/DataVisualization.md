# Data Visualization and File I/O

1. Reading/Writing Files
* Pandas and Data Frames
  - most common file formats
  - import pandaas as pd
  - df = pd.read_csv('Moluecules.csv')
  - df.head() => shows header
  - df.index => returns rows
  - df.columns => returns columns
  - df.corr() => returns Pearsons' correlation coefficient
  - Corr = df[df.columns[:-1]]/corr()
* a data frame has numerous functions
  - df[['logP', 'label']] => returns data frame of selected columns
  - df.iloc[4:6, 5:9] => slicing data frame using iloc
  - df.iloc[4,5] = 999 => manipulating individual entires
  - df.inset(2, 'New', df.ilocp:,1]) => inserting another low
* Saving the dat frame to an excel file
  - df.to_excel('Moluculers.xlsx)
* pandas can also read text files
  - cf = pd.read_csv('systfibr.txt')

* Faster Alternative
  - pandass is the standard library, but it is slow
  - reading a 130MB excel file: 83 sec
  - reading a 180MB csv file with the same content: 1.2 sec
  - reading a 180MB txt file with the same content: 1.5 seconds
  - dask: 0.016 sec => however, we might need to transfer: 1.7 sec
  - polars: 8.2 sec

* More about.txt
  - syntax of open
```python
    with open('List.txt', 'r') as read_f:
      with open('List_copy.txt', 'w') as write_f:
        for r in read_f:
          write_f.write(r)
```

2. Visualization
* Matplotlib

* Seaborn

* plt, ax, fig
