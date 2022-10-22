# Усложненный make-file.  Введены переменные для параметров компиляции и исполняемых файлов

.PHONY: all debug release clean

RELEASE_FLAGS = -O2 -Wall -DNDEBUG
DEBUG_FLAGS   = -g -O0 -Wall
RELEASE_EXEC  = Kazino-Royal
DEBUG_EXEC    = Kazino-Royal-dbg
#SOURCE        =

all: debug release

debug: Kazino-Royal

Kazino-Royal-dbg: hello.cpp
	g++ hello hello.cpp -o hello-dbg 

release: Kazino-Royal

Kazino-Royal: Kazino-Royal.cpp
	g++ Kazino-Royal Kazino-Royal.cpp -o Kazino-Royal

clean:
	rm -f Kazino-Royal Kazino-Royal-dbg

