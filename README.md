# Methylation
This research project developed an SI-metrologically traceable plasmid-based DNA methylation reference material system to resolve inter-laboratory quantification inconsistency in clinical epigenetic sequencing. 
The bioinformatic workflows rely on standard bioinformatics tools. 

Ensure the following tools are installed and available in your PATH:
Core Dependencies:
FastQC (>= v0.11.9)
Trim Galore! (>= v0.6.7) / Cutadapt
Bowtie2 (>= v2.4.4)
Bismark (>= v0.23.1)
BWA (>= v0.7.17)
Samtools (>= v1.13)
Picard (>= v2.26.0)
rastair (for TAPS CpG calling)
bedtools (>= v2.30.0)
htslib / tabix

Conda Environment Setup
conda create -n meth_benchmark python=3.9 -y
conda activate meth_benchmark
conda install -c bioconda -c conda-forge \
  bismark bowtie2 bwa samtools picard bedtools fastqc trim-galore htslib
# Install rastair according to its official documentation if using TAPS
