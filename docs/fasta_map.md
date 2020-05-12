# Fasta map class

- At first we create a named tuple that will contain the sample information needed for both sorting and filtering.
- We go through the CSV table once to create a dictionary as a key we will have the region and as a value a list where 
we will add those values registered in the named tuple.
- When we already have the dictionary, we pass the list to the function get_average_row that will return the sample 
line that has the average value in the samples of each region.
- Finally the list comprehension will filter the csv with our samples.

## *class* FastaMap
Represents a Map that stores RNA codes.

A fasta map is initialised using:
```
fasta_map = FastaMap(path_file) # file_path: The path to the .fasta file 
``` 
#### _read_fasta
Reads a fasta file and returns a dict where the keys are the accessions 
and the values are the RNA sequences
```pydocstring
        :param: file_path
        :return: sequences: Dict[str, str]
```
#### _get_rna
Get the header and the RNA from a String
```pydocstring
        :param: A String that contains info about the genome
        :return: A Id-value: Tuple[str, str]
```
#### group_samples
Creation Sets "family samples"
```pydocstring
        :param: csv_table:
        :return: tuple of relations: Tuple[List[set]]
```
#### compare_multi
Function to parallelize comparisons
```pydocstring
        :param ids :
        :return: Tuple of relations: Tuple[str, str, float]
```
#### generate_relations
Generate tuple of list where this list stores all sample's name
```pydocstring
        :param compares:
        :return: Tuple relation of samples: Tuple[List[set]]
```
