
bioinformatics task
	echo AGENYI_GODWIN
 # to print name
	mkdir AGENYI_GODWIN
 # to create folder titled name
	mkdir biocomputing
 # to create new folder ‘biocomputing’
cd biocomputing
 # to change to the new folder with a single command
	wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna 
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
# to download files
	mv wildtype.fna AGENYI_GODWIN 
# to move file to folder
	rm wildtype.gbk
 # to remove duplicate file
	grep ‘tatatata’ wildtype.fna
  # to scan file to confirm if mutant
	grep ‘tatatata’ wildtype.fna > mutant_file.txt 
# to print all matching line into a new file
	tail –n  +2 wildtype.gbk.1 | wc -l
# to count number of lines excluding header in .gbk file
	awk ‘/LOCUS/ {print $3}’ wildtype.gbk
# to print the sequence length of the .gbk file
	grep ‘^SOURCE’ wildtype.gbk | head –l
# to print source organism of .gbk file
	grep ‘/gene=’ wildtype.gbk
# to list gene names of .gbk file
	clear
# to clear terminal space 
history # to print all command used
	ls
cd ../
ls 
# to list files in folders

Project 2
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
# to activate base conda environment
conda config --add channels defaults
conda config --add channels bioconda
conda config --add channels conda-forge
# to configure channels for bioinformatics
	conda create -n funtools python=3.10
# to create conda environment 
conda activate funtools
# to activate funtools environment
	sudo  apt install figlet
# to install figlet
	figlet ‘AGENYI_GODWIN’
#to run figlet
conda deactivate
#to deactivate funtools 
conda install bwa
# to install bwa through biconda channel
conda install blast
# to install blast through biconda channel
conda install samtools
# to install samtools through biconda channel
 conda install bedtools
# to install bedtools through biconda channel
	conda install spades.py
# to intall spades.py through biconda channel
	conda install bcftools
# to install bcftools
	conda install fastp
# to install fastp
	conda install multiqc
# to install multiqc 

