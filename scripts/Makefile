all: swolisten

swolisten.o: swolisten.c
	gcc -c -O0 --pedantic -Werror -I/usr/include/libusb-1.0/ -o $@ $<

swolisten: swolisten.o
	gcc -o $@ $< -lusb-1.0

clean:
	rm -f swolisten swolisten.o
