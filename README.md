# kaiju2-data-parser 

- Put all your scaffolds.fasta metagenomes (from MetaSpades) in the directory (All-assemblies), same location of the script: run_kaiju2-phyloseq.py 
- Example: All_assembly/run_kaiju2-phyloseq.py
- run_kaiju2-phyloseq.py takes all fasta scaffolds (Ex: All-assemblies) generates from Spades and performed all steps of kaiju classification (https://github.com/bioinformatics-centre/kaiju)
- kaiju-run-parser output: 

  kaiju files summary, OTU and Taxonomy tables format to be imported into R (Ex: Phyloseq) or Python.
 
- The run_kaiju2-phyloseq.py use kaiju-multi, kaiju2table and kaiju-addTaxonNames which is need to be in your PATH: these programs are part of the kaiju.

 *Before to follow to perform run_kaiju2-phyloseq.py.
 
- Metaspades installation
- Run metaspades to get the Scaffolds.fasta for each sample.
- mkdir All-assemblies
- Save all scaffolds in the dir: All-assemblies
- kaiju installation
- kaiju databased files download (including: names.dmp and nodes.dmp from taxonomy database of NCBI and kaiju.fmi)
- kaiju.fmi: its is the indexed files of ncbi in kaiju format.
- Theses cited database files can be obtained with kaiju: kaiju-makedb -s nr_euk (more info here: https://github.com/bioinformatics-centre/kaiju).
- python3 -m venv kaiju2-parser
- source kaiju2-parser/bin/activate
- cd All-assemblies
- Download requeriments.txt to dir: All-assemblies
- pip3 install -r /path/to/All-assemblies/requirements.txt
- python3 run_kaiju2-phyloseq.py -h 
  The required arguments to run_kaiju2-phyloseq.py will be shown.
       



