# TicTacToe

The project is an implementation of a client-server Tic Tac Toe game using Java sockets. 
It allows multiple clients to connect to the server, play the game, and communicate with each other using a chat feature. 
It consists of the following classes:

**Server:** Manages client connections, creates sessions for each client, and handles communication between clients. Sessions run in separate threads and handle message reception, broadcasting, and termination.

**Client:** The main client application for the game. It establishes a connection with the server, initializes the UI components, and handles user interactions. It includes panels for game statistics, the game board, chat, and rules display.

**Game:** Represents the Tic Tac Toe game board. It manages game logic, button actions, and win/draw conditions. It creates a grid of buttons, assigns action listeners, and updates the game state accordingly.

**Stats:** Displays the number of wins for each player (X and O) and provides a clock to show the current time. It reads the number of wins from files and updates the labels accordingly. It also includes a refresh button to update the statistics.

**ChatPanel:** Enables chat messaging between clients. It includes a chat area, a text field for entering messages, and a send button. It handles user interactions, updates the chat area, and communicates with the server via a socket.

There can be a maximum of five clients connected, and if a 6th one tries to connect they get a rejection message printed out in the chat area.

The users can play on one client and refresh game statistics after each win, and they can also communicate with other clients(users) through the chat. 

The user can close the client  by pressing the escape button. A dialog window will then pop up asking if they’re sure they want to close it.
