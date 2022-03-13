all: server-chat

server.o: server.cpp
	g++ -c server.cpp

servernetwork.o: servernetwork.cpp
	g++ -c servernetwork.cpp

server-chat: server.o servernetwork.o
	g++ server.o servernetwork.o -o server-chat -lsfml-graphics -lsfml-window -lsfml-system -lsfml-network -lpthread

run:
	./server-chat

clean:
	rm servernetwork.o server.o
