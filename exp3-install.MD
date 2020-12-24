## 1. Copy experiment data

from Xiaochen Yang's host (password: ask me if dont know)

```
cd /home
rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/ex3_data .
rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/ex4_data .
```

------OR------

copy from Lirui Han
```
cd home
rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/ex3_data .
rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/ex4_data .
```

## 2 Install packages using APT for ***aarch64***, 

```
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
```

## 3  Install packages using APT for ***x86_64***

```
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
```

## 4. Install R packages (for aarch64 and x86_64)

If you use R 3.4
```
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(version="3.6")
BiocManager::install("Biobase",version="3.6", update=F)
BiocManager::install("qvalue",version="3.6", update=F)
install.package("fastcluster")
install.packages("https://cran.r-project.org/src/contrib/Archive/locfit/locfit_1.5-9.tar.gz")
BiocManager::install("edgeR",version="3.6")
BiocManager::install("DESeq2",version="3.6")
```

If you use R 3.6


```
if (!requireNamespace("BiocManager", quietly = TRUE))
    install.packages("BiocManager")

BiocManager::install(version="3.9")
BiocManager::install("Biobase",version="3.9", update=F)
BiocManager::install("qvalue",version="3.9", update=F)
install.package("fastcluster")
install.packages("https://cran.r-project.org/src/contrib/Archive/locfit/locfit_1.5-9.tar.gz")
BiocManager::install("edgeR",version="3.9")
BiocManager::install("DESeq2",version="3.9")
```

## 5. Install Trinity, bowtie2, jellyfish and cmake etc on ***aarch64***

1) copy codes from Xiaochen Yang's host

  rsync -rav --update --rsh=ssh cb2020@114.116.232.201:/home/workdir .

or copy codes from Lirui Han's host 

  rsync -rav --update --rsh=ssh cb2020@121.36.105.149:/home/workdir .

2) build CMake 3.15.0

  cmake .

  make 

  make install
