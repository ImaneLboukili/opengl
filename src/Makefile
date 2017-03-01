CFLAGS = -g -Wall -std=c++11 $(DEBUG)
all: main

main:  main.o UserInterface.o
	g++  $(CFLAGS) main.o UserInterface.o -o main -lGL -lglut -lGLU

main.o: main.cpp UserInterface.h
	g++  $(CFLAGS)-c  main.cpp   -o main.o -lGL -lglut -lGLU

UserInterface.o: UserInterface.cpp UserInterface.h
	g++ $(CFLAGS) -c   UserInterface.cpp  -o UserInterface.o -lGL -lglut -lGLU

clean:
	rm -f *.o
