CC=g++
SRC := $(MNIST_ML_ROOT)/KNN/src
CFLAGS := -std=c++11 -DEUCLID
INCLUDE_DIR := $(PWD)/include/*

all : main

main : $(SRC)/knn.cc
	$(CC) $(CFLAGS) $(SRC)/knn.cc -o main -L$(MNIST_ML_ROOT)/lib/ -ldata -I$(INCLUDE_DIR) \
	 -I$(MNIST_ML_ROOT)/include 

clean : 
	rm main

	#if libdata fails to load, export an env var...
	#LD_LIBRARY_PATH=$LD_LIBRARY_PATH://home/radimek/Desktop/git/mnist/MNIST_digits/lib
	#export LD_LIBRARY_PATH