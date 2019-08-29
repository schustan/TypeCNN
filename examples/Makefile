CC=g++
CFLAGS=-std=c++14

.PHONY: test_different_archs benchmark fixed demo neural

all: test_different_archs benchmark fixed demo neural

test_different_archs:
	$(CC) $(CFLAGS) -fopenmp test_different_archs.cpp  ../src/*.cpp ../src/*/*.cpp ../3rdParty/*/*.cpp -O3 -o test_different_archs -I ..

benchmark:
	$(CC) $(CFLAGS) benchmark.cpp  ../src/*.cpp ../src/*/*.cpp ../3rdParty/*/*.cpp -O3 -o benchmark -I ..

neural:
	$(CC) $(CFLAGS) neural_network.cpp  ../src/*.cpp ../src/*/*.cpp ../3rdParty/*/*.cpp -O3 -o neural_network -I ..

fixed:
	$(CC) $(CFLAGS) fixed_point.cpp  ../src/*.cpp ../src/*/*.cpp ../3rdParty/*/*.cpp -O3 -o fixed_point -I ..

demo:
	$(CC) $(CFLAGS) demo.cpp  ../src/*.cpp ../src/*/*.cpp ../3rdParty/*/*.cpp -O3 -o demo -I ..