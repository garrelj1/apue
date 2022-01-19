COMMON_DIR=../appendix
INC_DIR=../headers
SRC_DIR=src

CC=gcc
CFLAGS=-I $(INC_DIR)

DEPS=$(INC_DIR)/apue.h
DEPSC=$(COMMON_DIR)/apue.c

minils.out: $(SRC_DIR)/minils.c $(DEPSC) $(DEPS)
	$(CC) $(CFLAGS) $< $(DEPSC) -o $@ 
