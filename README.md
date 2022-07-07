# kaiju-run-parser (run_kaiju2-phyloseq.py)

*Before to follow for run_kaiju2-phyloseq.py.

*Steps: 1 - Metaspades installation
        2 - Run metaspades to obtain scaffolds.fasta
       4 - mkdir All-assemblies
       5 - Save scaffolds in the dir: All-assemblies
       3 - kaiju installation
       4 - kaiju databased download (included files: names.dmp and nodes.dmp from taxonomy database of NCBI and kaiju.fmi.
           * This files can be obtained wwith kaiju: kaiju-makedb -s nr_euk (more info here: https://github.com/bioinformatics-centre/kaiju).
       5 - python3 -m venv kaiju2-parser ###
       6 - source kaiju2-parser/bin/activate
       7 - cd All-assemblies
       8 - Download requeriments.txt to dir: All-assemblies
       9 - pip3 install -r /path/to/All-assemblies/requirements.txt
       10 - python3 run_kaiju2-phyloseq.py -h (The required parameters will be shown).
       
* This takes a directory with all fasta scaffolds (Ex: All-assemblies) generates from Spades and performed all steps of kaiju classification (http://kaiju.binf.ku.dk/)
- Put all your scaffolds.fasta (from MetaSpades) in the directory (All-assemblies), localization of script: run_kaiju2-phyloseq.py. 
   Example: All_assembly/run_kaiju2-phyloseq.py
- kaiju-run-parser output: kaiju classification: files summary, OTU and Tax tables format to be imported into Phyloseq (R-software). 
- The programs use kaiju-multi, kaiju2table and kaiju-addTaxonNames has to be in your PATH: these programs are part of the kaiju installation.



