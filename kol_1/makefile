
CPP=g++
CPPFLAG=-c -Wall

myProgram.out: main.o employee.o address.o
	$(CPP) -o myProgram main.o employee.o address.o

main.o: main.cpp employee.h address.h
	$(CPP) $(CPPFLAG) -pedantic main.cpp

employee.o: employee.cpp address.h
	$(CPP) $(CPPFLAG) -pedantic employee.cpp

address.o: address.cpp
	$(CPP) $(CPPFLAG) address.cpp

