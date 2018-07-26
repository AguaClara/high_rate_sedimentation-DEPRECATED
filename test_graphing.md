#####Testing pandas functions
```python
import pandas as pd

data_file_path = '/Users/HannahSi/Desktop/AguaClara Summer/Data/datalog 7-16-2018.xls'
df = pd.read_csv(data_file_path, delimiter='\t')
print(list(df))
print(df.iloc[:,0])
print(np.array(df.iloc[:,0]))
print(list(df.iloc[:,0]))
print(df['Time'][:])

print(df.loc[:,"Influent"])

data_file_path = '7-26-18.txt'
df = pd.read_csv(data_file_path, delimiter='\t')
has_text = df.iloc[:,0].astype(str).str.contains('[a-z]', '[A-Z]')
print(has_text)
text_rows = list(has_text.index[has_text])
print(df.drop(text_rows))

```
What does this line do? `text_row_index = text_row.index[text_row].tolist()`
<br></br>

##### Testing ProCoDA_Parser.ftime
```python
from aguaclara_research.ProCoDA_Parser import ftime

time = ftime('sample_data2.txt', 0)
print(np.array(time))
print()

data_file_path = 'sample_data2.txt'
start = 0
end = -1
df = pd.read_csv(data_file_path, delimiter='\t')
start_time = pd.to_numeric(df.iloc[start, 0])*u.day
print(start_time)
day_times = pd.to_numeric(df.iloc[start:end, 0])
print(day_times)
time_data = np.subtract((np.array(day_times)*u.day), start_time)
print(np.array(time_data))
```
Things to fix:
* The line `day_times = pd.to_numeric(df.iloc[start:end, 0])` truncates the time array by one element.
* time_data is not returned as a numpy array
* how was the program able to parse numbers with notes in between?

<br></br>

#####Testing ProCoDA_Parser.column_of_data
```python
from aguaclara_research.ProCoDA_Parser import column_of_data

data_file_path = 'sample_data2.txt'
print(column_of_data(data_file_path, 0, 1))
```
Things to fix:
* Variable `data` is never assigned in certain cases!!!
* [start:end] still truncates data

<br></br>

#####Testing ProCoDA_Parser.notes
```python
from aguaclara_research.ProCoDA_Parser import notes

data_file_path = 'sample_data2.txt'
print(notes(data_file_path))
```
Things to fix:
* still misses last row
