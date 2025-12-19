This repository contains scripts and codes for the analysis of NGS data in Erdogdu et al. (under review):

Most analysis was performed using snakePipes (Bhardwaj et al., 2019), therefore it is recommended to install snakePipes in your system. For details, you can visit https://snakepipes.readthedocs.io/en/stable/.

Quick start:

Step 1: conda create -n snakePipes -c conda-forge -c bioconda -c mpi-ie snakePipes

Step 2: Download genome fasta and annotation files for mm10, hg38 and dm6 and create index files for mm10 at least for bowtie2, STAR, bwa-mem2. For spike-in normalizations, hybrid genomes of mm10 with dm6 or hg38 will be required. All of this is possible using createIndices pipeline of snakePipes.

Step 3: Make sure that the configuration of snakePipes is correct, e.g. paths to indices are set in snakePipes configuration (see snakePipes config --help).
