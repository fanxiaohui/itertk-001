include ../../config

EXECDIR = ../../cgi-bin/
EXEC = net.cgi


OBJS	= net.o

%.o: %.c
	$(CC) -I$(INC) -c -o $*.o $<
default: $(OBJS)
	$(CC) $(OBJS) -o $(EXECDIR)$(EXEC) $(LIBS) $(CFLAGS) -lcrypt --static
	
clean:
	rm -f *.o
