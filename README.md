wsq2jpeg - A Wavelet Scalar Quantization algorithm (WSQ) conversion library (Please download the files in ./third_party separately!!!!!!!!!!!)
===========================

Is a library to convert wsq images to jpeg format and vice versa. Allows individual or batch processing. Only supports images in grayscale. 
# Building form sources
## I meet a strange problem in GitHub, that is when I download this code as .zip file, the codes in ./third_party directory cannot be downloaded. We must download these codes separately. Only when I download these codes, the program could be complied successfully.
## Pre-requisites
### Linux
```sh
 $ [sudo] apt-get install build-essential autoconf libtool pkg-config
```
## Compile NBIS
### Linux
```sh
 $ git clone https://github.com/rnhdev/wsq2jpeg
 $ cd third_party/nbis
 ./setup.sh . --without-X11 --64
 $ make config && make it
 $ cd ../..
 ```
 ## Compile and install
 ### Linux
 ```sh
 $ mkdir build 
 $ cd build
 $ cmake .. && make
 $ [sudo] make install
 ```
 ## Run examples
### WSQ to jpeg
```sh
 $ ./test_wsq ../test ../test 80
 ```
 ### jpeg to wsq 5:1
```sh
 $ ./test_jepg ../test ../test 2.25 
 ```
 
 ### jpeg to wsq 15:1
```sh
 $ ./test_jepg ../test ../test 0.75
 ```
