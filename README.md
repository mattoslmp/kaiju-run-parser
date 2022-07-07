# kaiju-run-parser: run_kaiju2-phyloseq.py

Its necessary install the modules:

- Bio
- glob
- pandas
- subprocess
- sys

* Sugestion You should creat the conda environment with these modules installed and python 3.7

# The fist step is kaiju installation and after you shoud run metaspades, before to follow for run_kaiju2-phyloseq.py

* This takes a directory with fasta scaffolds generates from Spades and performed kaiju classification (http://kaiju.binf.ku.dk/)

- kaiju-run-parser output: kaiju classification, files summary, creates OTU and Tax tables format to be imported into Phyloseq 
- The programs use kaiju-multi, kaiju2table and kaiju-addTaxonNames has to be in your PATH: these programs are part of the kaiju installation.

- The files names.dmp and nodes.dmp from obtained of taxonomy database of NCBI and kaiju.fmi (indexed nr ncbi files) are need to Kaiju run.

