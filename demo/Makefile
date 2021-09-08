CC = cl65
FILES_IN = $(wildcard *.s)
FILES_OUT := $(patsubst %s,%nes,$(FILES_IN))

.PHONY: default build run test
default: $(FILES_IN)
	$(CC) --target nes -o $(FILES_OUT) $(FILES_IN) && fceux $(FILES_OUT)
build: $(FILES_IN)
	$(CC) --target nes -o $(FILES_OUT) $(FILES_IN)
run: $(FILES_IN)
	$(CC) --target nes -o $(FILES_OUT) $(FILES_IN) && fceux $(FILES_OUT)
