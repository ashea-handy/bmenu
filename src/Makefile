CC = gcc
ODIR = obj
CFLAGS = -lncurses


_OBJ = bmenu.o
OBJ = $(patsubst %,$(ODIR)/%,$(_OBJ))

$(ODIR)/%.o: %.c
	$(CC) -c -o $@ $< $(CFLAGS)

HandyDev: $(OBJ)
	$(CC) -o $@ $^ $(CFLAGS)

clean:
	rm -f $(ODIR)/*.o HandyDev 
