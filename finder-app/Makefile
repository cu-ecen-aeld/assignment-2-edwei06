# Makefile for building the writer application

# Use native compiler or set CROSS_COMPILE for cross-compilation
CC ?= gcc
ifdef CROSS_COMPILE
    CC := $(CROSS_COMPILE)gcc
endif

CFLAGS = -Wall -Werror -O2

# Source file and target executable
SRC = writer.c
TARGET = writer

all: $(TARGET)

$(TARGET): $(SRC)
	$(CC) $(CFLAGS) -o $(TARGET) $(SRC)

clean:
	rm -f $(TARGET) *.o

.PHONY: all clean

