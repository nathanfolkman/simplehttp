CFLAGS = -I. -I../server -I$(LIBEVENT)/include -O2 -g
LIBS = -L. -L../server -L$(LIBEVENT)/lib -levent -lsimplehttp

pubsub: pubsub.c
	$(CC) $(CFLAGS) -o $@ $< $(LIBS)

install:
	/usr/bin/install pubsub $(LIBEVENT)/bin/

clean:
	rm -rf *.o pubsub *.dSYM
