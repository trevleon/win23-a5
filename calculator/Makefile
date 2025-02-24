CC = gcc
CFLAGS = -Wall -Wextra -std=c11
OBJ = main.o addition.o subtraction.o multiplication.o division.o
TARGET = calculator

all: $(TARGET)

$(TARGET): $(OBJ)
	$(CC) $(CFLAGS) -o $(TARGET) $(OBJ)

%.o: %.c operations.h
	$(CC) $(CFLAGS) -c $< -o $@

clean:
	rm -f $(OBJ) $(TARGET)