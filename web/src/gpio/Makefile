include ../../config

EXECDIR = ../../cgi-bin/
EXEC = gpio.cgi


OBJS	= gpio.o

%.o: %.c
	$(CC) -I$(INC) -g  -c -o $*.o $<
default: $(OBJS)
	$(CC) $(OBJS) -o $(EXECDIR)$(EXEC) $(LIBS) $(CFLAGS) -lcrypt --static
	
clean:
	rm -f *.o
