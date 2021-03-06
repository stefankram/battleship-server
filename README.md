# battleship-server
This project is aimed at designing a custom server in C++ that is able to handle multiple instances of two-player games of battleship over the internet. The server uses TCP sockets to send and receive messages between clients. The server is designed so that each connection from a client to the server has its own thread that is contained in a session object. The session object contains both the data of the client and the client's opponent with semaphores used for synchronization between threads.

### Examples of client playing battleship
Setting ships on the playing field
![Setting ships on the playing field](https://github.com/stefankram/battleship-server/blob/master/images/img1.png "Setting ships on the playing field")

In the middle of a game
![In the middle of a game](https://github.com/stefankram/battleship-server/blob/master/images/img2.png "In the middle of a game")

Towards the end of a game
![Towards the end of a game](https://github.com/stefankram/battleship-server/blob/master/images/img3.png "Towards the end of a game")

Losing the game
![Losing the game](https://github.com/stefankram/battleship-server/blob/master/images/img4.png "Losing the game")

*Client designed by [KirklandLandry](https://github.com/KirklandLandry) from project [3313-battleship](https://github.com/KirklandLandry/3313-battleship)*

### How to install and run

**Make sure** `cmake` **is version >=3.2.2 and** `make` **is version >=4.0**

1. Download source files and extract to working directory named 'Server'
2. Create a directory in your working directory called 'build' and go into it

		mkdir build && cd build

3. Run cmake with the following command

		cmake ..

4. Run make with the following command

		make

5. Run the server using the following command

		./Server
