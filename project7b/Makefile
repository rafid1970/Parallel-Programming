all: part1 part2 part3

part1:
	g++ mp.cpp -o part1_openMP -lm -fopenmp
	./part1_openMP

part2:
	g++ -c SIMD/simd.p5.cpp -o simd.p5.o
	g++ simd.cpp -o part2_simd simd.p5.o -lm -fopenmp
	./part2_simd

part3:
	g++ cl.cpp -o part3_openCL CL/libOpenCL.so -lm -fopenmp
	./part3_openCL

clean:
	rm -r *.csv part1_openMP part2_simd part3_openCL *.o
                                                                                                                    