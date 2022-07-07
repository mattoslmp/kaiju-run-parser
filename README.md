# kaiju-run-parser (run_kaiju2-phyloseq.py)

* This takes a directory with all fasta scaffolds (Ex: All-assemblies) generates from Spades and performed all steps of kaiju classification (http://kaiju.binf.ku.dk/)
- Put all your scaffolds.fasta (from MetaSpades) in the directory (All-assemblies), localization where will stay the script: run_kaiju2-phyloseq.py. 
   Example: All_assembly/run_kaiju2-phyloseq.py
- kaiju-run-parser output: kaiju classification: files summary, OTU and Tax tables format to be imported into Phyloseq (R-software). 
- The programs use kaiju-multi, kaiju2table and kaiju-addTaxonNames has to be in your PATH: these programs are part of the kaiju installation.

*Before to follow to perform run_kaiju2-phyloseq.py.

- Metaspades installation
- Run metaspades to get the Scaffolds.fasta for each sample.
- mkdir All-assemblies
- Save all scaffolds in the dir: All-assemblies
- kaiju installation
- kaiju databased files download (including: names.dmp and nodes.dmp from taxonomy database of NCBI and kaiju.fmi
- kaiju.fmi: indexed files of ncbi in kaiju format).
- Theses cited database files can be obtained with kaiju: kaiju-makedb -s nr_euk (more info here: https://github.com/bioinformatics-centre/kaiju).
- python3 -m venv kaiju2-parser
- source kaiju2-parser/bin/activate
- cd All-assemblies
- Download requeriments.txt to dir: All-assemblies
- pip3 install -r /path/to/All-assemblies/requirements.txt
- python3 run_kaiju2-phyloseq.py -h (the required arguments to run_kaiju2-phyloseq.py will be shown).
       



