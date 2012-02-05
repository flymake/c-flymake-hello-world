CC     = gcc

all: flymake_hello_world

flymake_hello_world: flymake_hello_world.o

flymake_hello_world.o: flymake_hello_world.c

check-syntax:
	$(CC) -Wall -Wextra -pedantic -fsyntax-only $(CHK_SOURCES)
# Fake gcc 4.5 output
#	echo "flymake_hello_world.c:1:1: warning: return type of ‘main’ is not ‘int’"
#	echo "flymake_hello_world.c: In function ‘main’:"
#	echo "flymake_hello_world.c:2:4: warning: implicit declaration of function ‘printf’"
#	echo "flymake_hello_world.c:2:4: warning: incompatible implicit declaration of built-in function ‘printf’"
#	echo "flymake_hello_world.c:4:1: error: expected declaration or statement at end of input"


clean:
	rm -f flymake_hello_world flymake_hello_world.o
