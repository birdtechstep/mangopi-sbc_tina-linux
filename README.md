# Tina-Linux
Tina-Linux for T113/D1-H/D1s



### Ubuntu environment 
  $ sudo apt-get install build-essential subversion git-core libncurses5-dev zlib1g-dev gawk flex quilt libssl-dev xsltproc libxml-parser-perl mercurial bzr ecj cvs unzip lib32z1 lib32z1-dev lib32stdc++6 libstdc++6 -y

### SDK download
  $ git clone  https://github.com/mangopi-sbc/Tina-Linux.git
  $ cd Tina-Linux/
  $ git submodule update --init --recursive
  $ wget https://github.com/mangopi-sbc/tina-static/releases/download/PRE/prebuilt.tar.gz .
  $ tar xzvf prebuilt.tar.gz
  $ wget https://github.com/mangopi-sbc/tina-static/releases/download/V1.0/riscv64-linux-x86_64-20200528.tar.xz -P ./lichee/brandy-2.0/tools/toolchain/
  $ wget https://github.com/mangopi-sbc/tina-static/releases/download/V1.0/gcc-linaro-7.2.1-2017.11-x86_64_arm-linux-gnueabi.tar.xz -P ./lichee/brandy-2.0/tools/toolchain/
 
 
### Compile
  $ source build/envsetup.sh
  $ lunch
``` 
  You're building on Linux

Lunch menu... pick a combo:
     1. f133_evb1-tina
     2. f133_pro-tina
     3. t113_evb1-tina
``` 
  $ 1 or 3
  
  $ muboot
  $ make
