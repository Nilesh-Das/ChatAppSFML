all: client-chat

client.o: client.cpp
	g++ -c client.cpp

clientnetwork.o: clientnetwork.cpp
	g++ -c clientnetwork.cpp

client-chat: client.o clientnetwork.o
	g++ client.o clientnetwork.o -o client-chat -lsfml-graphics -lsfml-window -lsfml-system -lsfml-network -lpthread

run:
	./client-chat

clean:
	rm clientnetwork.o client.o
