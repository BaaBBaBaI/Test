CXX = g++

CXXFLAGS = -Wall -Wextra -std=c++17

TARGET = hello_app

OBJS = main.o hello.o 

all: $(TARGET)

$(TARGET): $(OBJS)
	$(CXX) $(CXXFLAGS) -o $(TARGET) $(OBJS)

main.o: main.cpp hello.h
	$(CXX) $(CXXFLAGS) -c main.cpp

hello.o: hello.cpp hello.h
	$(CXX) $(CXXFLAGS) -c hello.cpp

clean:
	rm -f $(OBJS) $(TARGET)
