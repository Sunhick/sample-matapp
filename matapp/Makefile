CC = gcc
DEBUG = -g -O0
LDFLAGS = 

IDIR = ./inc

CCFLAGS = -Wall $(DEBUG) -I $(IDIR)

all: main

main: main.o
	$(CC) -o $@ $(CFLAGS) $< -L ../modules/matlib/lib/ -lmatlib

main.o: main.c
	$(CC) -c $(CFLAGS) $<

.PHONY: clean
clean: 
	-rm *.o main *~