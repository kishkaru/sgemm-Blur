OBJS=conv2d.o readjpeg.o counters.o

%.o: %.cpp readjpeg.h
	g++ -fopenmp -O3 -c $<

all: $(OBJS)
	g++ -pthread -fopenmp -O3 $(OBJS) -o conv2d -ljpeg

clean:
	rm -rf conv2d $(OBJS)