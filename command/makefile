flags=-O2 -Wall -std=c23 -I../osapi
ldflags=

.PHONY: clean

all: clean command.com

command.com: command.o ../osapi/osapi.o
	cc $(flags) $^ -o $@ $(ldflags)

command.o: command.c command.h
	cc $(flags) -c $<

clean:
	rm -f *.o command.com
