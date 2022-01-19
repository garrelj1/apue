BUILD_DIR=build
COMMON_DIR=../appendix
INC_DIR=../headers
SRC_DIR=src

CC=gcc
CFLAGS=-I $(INC_DIR)

DEPS=$(COMMON_DIR)/apue.c

minils: src/minils.c $(DEPS)
	$(CC) $(CFLAG) -o $< $(BUILD_DIR)/$@ 

.PHONY clean:
clean: 
	rm -rf $(BUILD_DIR)
