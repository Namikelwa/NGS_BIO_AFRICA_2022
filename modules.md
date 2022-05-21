# NGSBioAfrica
 ## Module 1: Unix
Reading and Editing files
SED
AWK
BASH Scripting

 ## Module 2: NGS Technologies
1st generation-sangersequencing(short reads)
2nd generation-illumina,ion torrent/thermo fischer(short reads)
3rd generation-nanopore,pacbio SMRT (long reads)

Long and short reads can complement each other
* Long reads improve genome assembly
* Assembly can be corrected by short reads
* Long reads bridge regions with high error rate
* Short reads can correct base calls of long reads

High Throughput Sequencing offeres a broad range of applications
* Discover variants
* Population studies
* Analyze clinical isolates
* Study rare diseases
* Characterize the genome
* Characterize DNA-Protein(TF)interactions

Challenges of HT Sequencing 
* Data collection-extensive uses of resources,sampling accuracy
* Data analysis and interpretation
* Analytical/Computational challenges

 ## Module 3: NGS Data Analysis Overview and Data Formats
  
Obtaining data to be used
 
 cd course_data/data_formats/data
 unzip SRR957824
 cd SRR957824
 
 Quality check
 
 fastqc SRR957824_1.fastq.gz
 fastqc SRR957824_2.fastq.gz
           or
 fastqc SRR957824_1.fastq.gz  SRR957824_2.fastq.gz
           or 
 fastqc *.fastq.gz   (using a wildcard) 
 
 multiqc ./
 
 #to view the quality reports
 firefox SRR957824_1.fastq.html
 firefox SRR957824_2.fastq.html 
 firefox multiqc*.html
 
