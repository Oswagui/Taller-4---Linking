IDIR = ../include
CC = gcc
CFLAGS =-I$(IDIR)

ODIR=obj
LDIR =../lib

LIBS =-lm

_DEPS = vector.h
DEPS = $(patsubst %, $(IDIR)/%,$(_DEPS))

_OBJ = multvec.o addvec.o main2.o
OBJ = $(patsubst %, $(ODIR)/%,$(_OBJ))

$(ODIR)/%.o: %.c $(DEPS)
	$(CC) -c -o $@ $< $(CFLAGS)

main2: $(OBJ)
	gcc -o $@ $^ $(CFLAGS) $(LIBS)

.PHONY: clean

clean:
	rm -f $(ODIR)/*.o *~ core $(INCDIR)/*~ 
