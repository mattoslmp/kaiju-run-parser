# kaiju-run-parser

* This takes a directory with fasta scaffolds generates from Spades and performed kaiju classification (http://kaiju.binf.ku.dk/)
# The fist step is kaiju installation and after you shoud run metaspades

- Output: kaiju classification, files summary, creates OTU and Tax tables format to be imported into Phyloseq 
- The programs use kaiju-multi, kaiju2table and kaiju-addTaxonNames has to be in your PATH: these programs are part of the kaiju installation.

- The files names.dmp and nodes.dmp from obtained of taxonomy database of NCBI and kaiju.fmi (indexed nr ncbi files) are need to Kaiju run.

- Necessario instalar os módulos em python:
- Bio
- glob
- pandas
- subprocess
- sys
- import os

