CC = gcc
INCLUDE =
CFLAGS = -c -Wall -g
TARGET = animal.exe
SOURCE = dog.c blackcow.c turtle.c main.c
OBJECT = $(SOURCE:.c=.o)
SOURCE2 = animal.h

.PHONY: all clean

all: $(TARGET)
$(TARGET): $(OBJECT)
	$(CC) -o $(TARGET) $(OBJECT)
%.o: %.c $(SOURCE2)
	$(CC) $(CFLAGS) -o $@ $<
clean:
	rm -f $(OBJECT) $(TARGET)

