wget https://github.com/trinityrnaseq/trinityrnaseq/releases/download/v2.8.6/trinityrnaseq-v2.8.6.FULL.tar.gz


#https://github.com/trinityrnaseq/trinityrnaseq/issues/178
#Remove -m64 in CMakefiles.txt
#
# trinityrnaseq-v2.8.6/trinity-plugins/ParaFly-0.1.0/configuare.ac


wget https://github.com/gmarcais/Jellyfish/releases/download/v2.3.0/jellyfish-2.3.0.tar.gz
tar -xvzf jellyfish-2.3.0.tar.gz
cd jellyfish-2.3.0
./configure
make
cd ..


wget https://sourceforge.net/projects/bowtie-bio/files/bowtie2/2.3.5.1/bowtie2-2.3.5.1-source.zip/download
cd bowtie2-2.3.5.1
make


apt ungrade cmake
#install libiconv 
wget http://ftp.gnu.org/pub/gnu/libiconv/libiconv-1.16.tar.gz
$ ./configure --prefix=/usr/local
$ make
$ make install

apt install boost
apt install libtbb-dev
apt install libcurl4-openssl-dev
apt install libjemalloc-dev
apt install libcereal-dev
apt install libdivsufsort-dev
apt install libgff-dev
 
wget https://github.com/COMBINE-lab/salmon/archive/v0.14.1.tar.gz


