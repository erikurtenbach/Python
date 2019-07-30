# Numpy
## Array
```
data = np.array([[1,2,3],[4,5,6],[6,7,8]])

data[0,2]
>3

data[0:,1]
>array([2, 5, 7])
```
               
# Pandas
## DataFrame
From array
```
data = np.array([['','Col1','Col2'],
                ['Row1',1,2],
                ['Row2',3,4]])
print(pd.DataFrame(data=data[1:,1:],
                  index=data[1:,0],
                  columns=data[0,1:]))
>>         Col1 Col2
    Row1    1    2
    Row2    3    4
```
From dictionary
```
# Take a dictionary as input to your DataFrame 
my_dict = {1: ['1', '3'], 2: ['1', '2'], 3: ['2', '4']}
print(pd.DataFrame(my_dict))
>>
       1  2  3
    0  1  1  2
    1  3  2  4
```
From series
```
# Take a Series as input to your DataFrame
my_series = pd.Series({"United Kingdom":"London", "India":"New Delhi", "United States":"Washington", "Belgium":"Brussels"})
print(pd.DataFrame(my_series))
>>
                             0
    Belgium           Brussels
    India            New Delhi
    United Kingdom      London
    United States   Washington
```
From Pandas DataFrame
```
# Take a DataFrame as input to your DataFrame 
my_df = pd.DataFrame(data=[4,5,6,7], index=range(0,4), columns=['A'])
print(pd.DataFrame(my_df))
>>>
       A
    0  4
    1  5
    2  6
    3  7
```
