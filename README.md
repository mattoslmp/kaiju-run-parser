# kaiju-run-parser

* This takes a directory with fasta scaffolds generates from Spades and performed kaiju classification (http://kaiju.binf.ku.dk/)
- Output: kaiju classification, files summary, creates OTU and Tax tables format to be imported into Phyloseq 
- The programs use kaiju-multi, kaiju2table and kaiju-addTaxonNames. 
- kaiju-multi, kaiju2table and kaiju-addTaxonNames has to be in your PATH: these programs are part of the kaiju installation to add taxa names to each OTU.
- The files names.dmp and nodes.dmp from obtained of taxonomy database of NCBI and kaiju.fmi (indexed nr ncbi files) are need to Kaiju run.
