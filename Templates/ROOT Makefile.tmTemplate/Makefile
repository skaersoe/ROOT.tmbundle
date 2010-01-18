# Morten Dam 2009
# CERN ROOT Makefile skeleton

# Compiler
CC=g++

# Sources
SOURCES=rootapp.cpp

#Name of binary
EXECUTABLE=MyROOTApplication


#######################

OBJECTS=$(SOURCES:.cpp=.o)

# Flags
CFLAGS=-c `root-config --cflags`
LDFLAGS=`root-config --glibs`

all: $(SOURCES) $(EXECUTABLE)

$(EXECUTABLE): $(OBJECTS)
	$(CC) $(LDFLAGS) $(OBJECTS) -o $@

.cpp.o:
	$(CC) $(CFLAGS) $< -o $@
	

clean:
	rm -rf *.o $(EXECUTABLE)