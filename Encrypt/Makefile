CC = gcc
CFLAGS = -g -Wall -o
DEPS = encrypt.c fileRecursor.c curlHelper.c
OBJECTS =encrypt.o curlHelper.o fileRecursor.o
EXECS = encrypt 

all:
	$(CC) -c encrypt.c
	$(CC) -c fileRecursor.c -lcrypto
	$(CC) -c curlHelper.c -lcmurl


	$(CC) $(CFLAGS) encrypt encryptDriver.c $(OBJECTS) -lcrypto -lcurl


clean:
	rm *.o $(EXECS)