COMMON_DIR=../appendix
INC_DIR=../headers
SRC_DIR=src

CC=gcc
CFLAGS=-I $(INC_DIR)

DEPS=$(INC_DIR)/apue.h
DEPSC=$(COMMON_DIR)/apue.c

OBJS_FULL := $(wildcard $(SRC_DIR)/*.c)
OBJS_NAME := $(notdir $(OBJS_FULL))
ALL_OBJS := $(patsubst %.c, %.out, $(OBJS_NAME))

.PHONY: all
all: $(ALL_OBJS)

%.out: $(SRC_DIR)/%.c $(DEPSC) $(DEPS)
	$(CC) $(CFLAGS) $< $(DEPSC) -o $@ 

.PHONY: clean
clean:
	rm *.out
