COMMON_DIR=../appendix
INC_DIR=../headers
SRC_DIR=src

CC=gcc
CFLAGS=-I $(INC_DIR)

DEPS=$(INC_DIR)/apue.h
DEPSC=$(COMMON_DIR)/apue.c

all: minils.out echo.out

.PHONY: clean
clean:
	rm *.out

minils.out: $(SRC_DIR)/minils.c $(DEPSC) $(DEPS)
	$(CC) $(CFLAGS) $< $(DEPSC) -o $@ 

echo.out: $(SRC_DIR)/echo.c $(DEPSC) $(DEPS)
	$(CC) $(CFLAGS) $< $(DEPSC) -o $@ 
