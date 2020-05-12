# Csv table class

## *class* CsvTable
Helps to handle .csv files data and its processing.

A csv table is initialised using:
```
csv_table = CsvTable(path_file) # file_path: The path to the .csv file 
- We can also initialize the instance with the csv table
```
####  filter
Filters the csv by country for average length's
```pydocstring
        :return: CsvTable        
```
#### __read_csv
Reads a csv file
```pydocstring
        :return: List[Dict]
```
#### quick_select_median
Implementation quick select median sort 
```pydocstring
        :param values: List[tuple]
        :param pivot_fn:
        :param index: int
        :return: tuple
```


