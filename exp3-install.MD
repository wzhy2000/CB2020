#1. Copy experiment data

from Xiaochen Yang's host (password: kaobeionly)

cd /home

rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/ex3_data .

rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/ex4_data .

------or copy from Lirui han------

cd home

rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/ex3_data .

rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/ex4_data .


#2 For aarch64, install packages using APT

apt install curl

apt install libcurl4-openssl-dev

apt install libboost-all-dev

apt install libtbb-dev

apt install libjemalloc-dev

apt install libcereal-dev

apt install libdivsufsort-dev

apt install libgff-dev

apt install staden

apt install libstaden-read-dev

apt install blast2

apt install libhts-dev

apt install samtools

apt install hmmer

apt install rsem

apt install augustus

#3  Install software for x86_64

apt install bowtie2

apt install blast2

apt install libhts-dev

apt install samtools

apt install hmmer

apt install rsem

apt install augustus

apt install libboost-all-dev

apt install libtbb-dev

apt install libjemalloc-dev

apt install libcereal-dev

apt install libdivsufsort-dev

apt install libgff-dev

apt install staden

apt install libstaden-read-dev


#3. Install R packages (for aarch64 and x86_64)

R packages

if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(version="3.6")

BiocManager::install("Biobase",version="3.6")

BiocManager::install("qvalue",version="3.6")

install.package("fastcluster")

install.packages("https://cran.r-project.org/src/contrib/Archive/locfit/locfit_1.5-9.tar.gz")

BiocManager::install("edgeR",version="3.6")

BiocManager::install("DESeq2",version="3.6")



(For aarch64 only)

rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/workdir .
(For aarch64 only)

rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/workdir .

