CXX = g++
CXXFLAGS = -Wall -Wextra -std=c++11

TARGET = kazino-royal
SRC = Kazino-Royal.cpp
OBJ = $(SRC:.cpp=.o)

.PHONY: all clean run show

all: $(TARGET)

$(TARGET): $(OBJ)
	$(CXX) $(CXXFLAGS) $(OBJ) -o $(TARGET)

%.o: %.cpp
	$(CXX) $(CXXFLAGS) -c $< -o $@

run: $(TARGET)
	./$(TARGET)

clean:
	rm -f $(TARGET) $(OBJ)

show:
	@echo "Compiler: $(CXX)"
	@echo "Flags: $(CXXFLAGS)"
	@echo "Source: $(SRC)"
	@echo "Target: $(TARGET)"
