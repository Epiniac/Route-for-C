# Makefile
 
CC = gcc -fsanitize=address
CPPFLAGS = -MMD
CFLAGS = -Wall -Wextra -std=c99 -O0 -g
LDFLAGS =
LDLIBS =
 
OBJ = matrix.o mathrix.o
DEP = ${OBJ:.o=.d}
 
all: mathrix
 
mathrix: ${OBJ}
 
.PHONY: clean
 
clean:
	${RM} ${OBJ} ${DEP} mathrix
 
-include ${DEP}
 
# END