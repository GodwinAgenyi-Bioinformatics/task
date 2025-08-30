# to print name
echo AGENYI_GODWIN
 
 # to create folder titled name
mkdir AGENYI_GODWIN

 # to create new folder ‘biocomputing’
mkdir biocomputing
 
# to change to the new folder with a single command
cd biocomputing

# to download files
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.fna 
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk
wget https://raw.githubusercontent.com/josoga2/dataset-repos/main/wildtype.gbk

# to move file to folder
mv wildtype.fna AGENYI_GODWIN 

 # to remove duplicate file
rm wildtype.gbk

 # to scan file to confirm if mutant
grep ‘tatatata’ wildtype.fna
 
 # to print all matching line into a new file
grep ‘tatatata’ wildtype.fna > mutant_file.txt 

# to count number of lines excluding header in .gbk file
tail –n  +2 wildtype.gbk.1 | wc -l

# to print the sequence length of the .gbk file
awk ‘/LOCUS/ {print $3}’ wildtype.gbk

# to print source organism of .gbk file
grep ‘^SOURCE’ wildtype.gbk | head –l

# to list gene names of .gbk file
grep ‘/gene=’ wildtype.gbk

# to clear terminal space 
clear

 # to print all command used
history 

# to list files in folders
ls
cd ../
ls 



Project 2

# to activate base conda environment
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh

# to configure channels for bioinformatics
conda config --add channels defaults
conda config --add channels bioconda
conda config --add channels conda-forge

# to create conda environment 
conda create -n funtools python=3.10

# to activate funtools environment
conda activate funtools

# to install figlet
sudo  apt install figlet

#to run figlet
figlet ‘AGENYI_GODWIN’

#to deactivate funtools 
6conda deactivate

# to install bwa through biconda channel
conda install bwa

# to install blast through biconda channel
conda install blast

# to install samtools through biconda channel
conda install samtools

# to install bedtools through biconda channel
conda install bedtools

# to install spades.py through biconda channel
conda install spades.py

# to install bcftools
conda install bcftools

# to install fastp
conda install fastp

# to install multiqc 
conda install multiqc
