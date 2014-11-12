# source files.
SRC =  	xbox/xboxlib.c eeprom/BootHddKey.c crypto/rc4.c crypto/sha1.c 

OBJ = $(SRC:.c=.o)

OUT = ../libeeprom.a

# include directories
INCLUDES = -I. 

# C++ compiler flags (-g -O2 -Wall)
CCFLAGS = -g

# compiler
CCC = gcc

# library paths
LIBS = -L/usr/local/lib -lm

# compile flags
LDFLAGS = -g

.SUFFIXES: .c

.c.o:
	$(CCC) $(INCLUDES) $(CCFLAGS) -c $< -o $@

$(OUT): $(OBJ)
	ar rcs $(OUT) $(OBJ)
