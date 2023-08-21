# Terminal Commands 
The following provides a basic introduction into the world of Terminal (on Windows) and the Terminal Emulator on Mac OS, both of which provide text-based command line interaction with the respective operating system. This is designed to introduce users to the core commands needed to navigate files and directories as well as communicate and execute commands against the operating systems.
## Launching the Command Terminal.
The Terminal program can be launched graphically or with a text-based command both on Windows and Mac.

### Graphically on Windows

### Via the run command 

### Graphically on Mac
From your Mac Desktop, click the spotlight icon among the list of icons displayedin the top right corner. Type the word terminal as shown below and press Enter key.

![terminal-app-mac](img/terminal-app-mac.png "How to launch terminal on Mac")

### Present working directory (pwd)
When working in a terminal environment, it is important to have awareness of where you are executing commands from. Just like a house or a building, you need to know where you are starting from to be able to navigate to the room, floor or section of the house or building that you need to get to. Use the following command to determine your current location:
``` zsh
    pwd
```

![pwd-sample-output](img/pwd-sample-output.png "sample output on Mac for pwd terminal command")

### List files and directories in the current working directory (ls)
``` zsh
ls
```
![sample-output-for-ls-command](img/ls-sample-output.png "Sample output for ls command")
### List current directories in the current working directory (dir)

### Make a Directory (i.e. folder) in the current working directory (mkdir)

### Change location to another working directory (cd)


## Understanding Absolute (/) and Relative (./) Paths
Terminal offers great flexibility and timesaving features by allow users to give commands using absolute and relative paths. Absolute path requires an explicit reference beginning from the root folder (/) unless the current working directory is a part of the fully qualified path. While relative path requires a  reference to the target folder which is relative to the present working directory. For example, let's say our present working directory is **/Users/moc/sandbox** and we would like to create 3 directories (week1, week2, week3) in the **/Users/moc/training** folder. This is how we could achieve this using Absolute and Relative Paths.

![absolute-vs-relative-path](img/absolute-vs-relative-path.png "Absolute vs. Relative path")
### Using Absolute path
``` zsh
    mkdir /Users/moc/training/week1 /Users/moc/training/week2 /Users/moc/training/week3
```

### Using Relative path
``` zsh
    mkdir ../training/week1 ../training/week2 ../training/week3
``` 
