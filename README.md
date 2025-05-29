# orf-finder

A Python-based tool to identify Open Reading Frames (ORFs) in DNA sequences provided in FASTA format, across all six reading frames. 

## Project Description

Open Reading Frames (ORFs) are sequences in DNA that potentially encode proteins. This program scans for ORFs in all six frames—three in the forward strand and three in the reverse complement—using custom Python functions.

The tool supports:
- Parsing FASTA files
- Handling multi-line, whitespace-containing, mixed-case sequences
- User-defined minimum ORF length
- Outputs in FASTA-like format with codons grouped

## System Requirements

- Python 3.6 or higher
- Any operating system (macOS, Linux, Windows)
- Terminal or command-line access
- Optional: Jupyter Notebook to open `.ipynb` file

---

## How to Run the Tool
1. Clone this repository:
   ```bash
   git clone https://github.com/shatakshi30/orf-finder.git
   ```
   
2. Make sure you have a FASTA file, e.g., sequence.fasta.

3. Run the script:

```bash
python "final code.ipynb"
```

4. When prompted, enter:
Enter FASTA file: sequence.fasta
Enter minimum length in bp for ORFs: 300

## Methods Used

- **FASTA File Parsing**
- **Codon Extraction**
- **Six Reading Frame Generation**
- **ORF Detection**
- **FASTA-Style Output Formatting**

## Results
**Sample input:**
FASTA file: sequence.fasta  
Minimum ORF length: 300

Sample output:
```text 
>Test1 | FRAME = 1 POS = 25 LEN = 996  
ATG GCT CCC AAG GGT TTA ATC TTT TTG GCT GTG TTA TGC TTC TCA  
GCA CTG TCA CTG AGT CGT TGT CTT GCG GAG GAT AAT GGA CTT GTT  
ATG AAC TTC TAC AAG GAA TCA TGC CCT CAG GCT GAA GAC ATC ATC  
AAA GAA CAA GTC AAG CTT CTC TAC AAG CGC CAC AAG AAC ACT GCT  
TTC TCC TGG CTC AGA AAC ATC TTC CAT GAC TGT GCT GTT CAG AGT  
...

>Test1 | FRAME = 6 POS = -933 LEN = 324  
ATG GCA CCA AAC TTG TCA AGA ACT GCA GAA ATG GAT TCA TTG TGG  
TCT GGG AGG AAC TGC TCT ACC ACA TCG GCT CTG CTC CTT CTA CCA  
TCC CTT CTT CCT GTT TTA AGA GGG ATA TGG GGA CCT CCT AGC GAA  
...

```

## Files in This Repository

- `sequence.fasta`: Input sequence file
- `final code.ipynb`: Main code for ORF detection.
- `output.txt`: Example output with ORFs found in a sample FASTA file.


## Learnings

- Implemented biological data processing logic using Python.
- Gained experience in handling real-life data formats like FASTA.
- Practiced collaborative code integration and modular design.
- Developed debugging and exception-handling strategies.
