# Final Project Proposal

## Group Members:

Keith Hah

# Intentions:

I will be making a music library program that incorporates a system that manages the music library, a music player, and a way to access music data. Users will be able to select, store, and play audio files, as well as save the library data into a file.

(ideas so far: multiplayer game, music library, organizing files)

# Intended usage:

There will be a command line interface where users can add new music files to their library, view their library, view and play individual songs, and save their library data into binary files. This program will be using multiple processes.

# Technical Details:

I will be using structs to represent each song, which will allow me to allocate memory and store music files in memory, as well as a linked list to hold the collection of songs. I will also use semaphores and shared memory to control access to the music library (ex: so multiple parts of the program don't modify the library at same time). I can then use named and unamed pipes and sockets to have the program and the music player communicate (ex: to autoplay the next song). The program will handle signals to stop playing the songs or to terminate the program when needed.

I think I will break the project down into the basic music library (which includes adding/removing songs, viewing song info, displaying library, handling files) and the actual music player.

I will be using linked lists to create the music library, semaphores to access and modify the music library, and file operations to store and retreieve data from the library.

# Intended pacing:

Create the music library and add basic functions: 1/9
Implement saving and loading files function (maybe in binary): 1/11
Implement music player (fork and exec): 1/13
Implement semaphores to manage music library: 1/15
Implement shared memory: 1/17
Implement pipes and process communication: 1/19
Testing and debugging: 1/20