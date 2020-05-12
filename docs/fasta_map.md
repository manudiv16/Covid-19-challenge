# Fasta map class

### *class* FastaMap
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
