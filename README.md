# orf-finder

A Python-based tool to identify Open Reading Frames (ORFs) in DNA sequences provided in FASTA format, across all six reading frames. 

## Project Description

Open Reading Frames (ORFs) are sequences in DNA that potentially encode proteins. This program scans for ORFs in all six frames—three in the forward strand and three in the reverse complement—using custom Python functions.

The tool supports:
- Parsing FASTA files
- Handling multi-line, whitespace-containing, mixed-case sequences
- User-defined minimum ORF length
- Outputs in FASTA-like format with codons grouped

## Methods Used

- **FASTA File Parsing**
- **Codon Extraction**
- **Six Reading Frame Generation**
- **ORF Detection**
- **FASTA-Style Output Formatting**

## Results

Sample input:
FASTA file: sequence.fasta
Minimum ORF length: 300


Sample output:
Test1 | FRAME = 1 POS = 25 LEN = 996
ATG GCT CCC AAG GGT TTA ...
...
Test1 | FRAME = 6 POS = -933 LEN = 324
ATG GCA CCA AAC TTG ...


## Files in This Repository

- 'sequence.fasta': Input sequence file
- `final code pcc.ipynb`: Main code for ORF detection.
- `output.txt`: Example output with ORFs found in a sample FASTA file.


## Learnings

- Implemented biological data processing logic using Python.
- Gained experience in handling real-life data formats like FASTA.
- Practiced collaborative code integration and modular design.
- Developed debugging and exception-handling strategies.
