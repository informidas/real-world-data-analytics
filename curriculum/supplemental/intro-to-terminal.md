# Terminal Commands 
The following provides a basic introduction into the world of Terminal (on Windows) and the Terminal Emulator on Mac OS, both of which provide text-based command line interaction with the respective operating system. This is designed to introduce users to the core commands needed to navigate files and directories as well as communicate and execute commands against the operating systems.
## Launching the Command Terminal.
The Terminal program can be launched graphically or with a text-based command both on Windows and Mac.

### Graphically on Windows
In Windows, we can launch the Terminal graphically by typing terminal in the search box on the task bar, then clicking on the terminal icon as shown below:

![terminal-app-windows](img/launch-terminal-graphically-windows.png "How to launch terminal on Windows")

### Via the run command 
Alternately, we could also type **cmd** in the search field on the taskbar and press ENTER to launch the terminal window.

![run-cmd-command](img/run-cmd-command.png "How to launch terminal on Windows using CMD command")

### Graphically on Mac
From your Mac Desktop, click the spotlight icon among the list of icons displayedin the top right corner. Type the word terminal as shown below and press Enter key.

![terminal-app-mac](img/terminal-app-mac.png "How to launch terminal on Mac")

## How does the terminal work?
The terminal is an interactive shell which accepts user input as text-base inputs as commands instructing the computer's operating system to perform some action. While the commands can seem terse and cryptic at first, you really need to learn a handful of commands to be functional as a Data Analytics professional.

## Root Directory (\ on Windows, / MAC and Unix / Linux based systems)


### Present working directory (pwd)
When working in a terminal environment, it is important to have awareness of where you are executing commands from. Just like a house or a building, you need to know where you are starting from to be able to navigate to the room, floor or section of the house or building that you need to get to. Use the following command to determine your current location:
``` zsh
    pwd
```

![pwd-sample-output](img/pwd-sample-output.png "sample output on Mac for pwd terminal command")

### List files and directories in the current working directory (ls)
It is also important to view the contents of the current directory you are in. We achieve this using the list command

``` zsh
    ls
```
![sample-output-for-ls-command](img/ls-sample-output.png "Sample output for ls command")

### Make a Directory (i.e. folder) in the current working directory (mkdir)
On Unix-like terminals (Mac, Linux) and modern versions of Windows we have the ability to create a new folder using the **mkdir** command. While legacy versions of Windows operating systems used **md** to make a directory, I think it is pretty safe to use the mkdir command in terminal environments for all of the above OS's.  

``` zsh
    mkdir {name_of_directy}
```

![make-directory-training](img/make-directory-training.png "Make Directory Training")

### Change directory to the newly created trainig directory (cd)
Once a directory has been created, a user has the option to switch to that directory to view its contents or add additional files or folders to the directory.

![changing-directories](img/changing-directories.png "Changing into a Directory")

## Understanding Absolute (/) and Relative (./) Paths
Terminal offers great flexibility and timesaving features by allow users to give commands using absolute and relative paths. Absolute path requires an explicit reference beginning from the root folder (/) unless the current working directory is a part of the fully qualified path. While relative path requires a  reference to the target folder which is relative to the present working directory. For example, let's say our present working directory is **/Users/moc/sandbox** and we would like to create 3 directories (week1, week2, week3) in the **/Users/moc/training** folder. This is how we could achieve this using Absolute and Relative Paths.

### First confirm our current location
![absolute-vs-relative-path](img/absolute-vs-relative-path.png "Absolute vs. Relative path")

### Using Absolute path (/)
``` zsh
    mkdir /Users/moc/training/week1 /Users/moc/training/week2 /Users/moc/training/week3
```

![new-folders-created](img/new-folders-created.png "New Folders Created")

### Using Relative path (./)
``` zsh
    mkdir ../training/week1 ../training/week2 ../training/week3
```

![new-folders-created](img/new-folders-created.png "New Folders Created")

### Creating Files (touch)
The real benefit of creating folders is to allow us to organize and contain additional folders (i.e. sub-folders) and files. We already know the command to create a folder and creating a file is just as simple.

``` zsh
    touch {name_of_file_including_extension}
```

In the *example* below, we create three files (Dashboard.xlsw, jobs.csv, and manual.pdf) in the Week1 folder using the **touch** command
![create-file](img/create-file.png "Create Files")

### Removing Files (rm) and Directories (rmdir)
We have two commands that can be used to remove files and folders respectively. First, we will look at the simple case for both before introducing additional scenarios which create the need for modifiers which are more commonly referred to as flags.

**removing a file**
``` zsh
    rm {file_name_including_extension}
```

**removing an empty directory**
``` zsh
    rmdir {name_of_directory}
```

## Using Flags as Command modifiers in Terminal
Often times, using a terminal command by itself is not enough to achieve the output or outcome that we need. To use flags, we list the command then add a dash then the particular modifier:
``` zsh
    command -flag
```

### Using Flags with List command (-al | la)
One of the most useful flags used is for listing details about a file including:
- file permission
- file owner
- creation date
- file size

``` zsh
    ls -al
```

![ls-al-flag](img/ls-al-flag.png "Flag Modifier")

Note that the modifiers can be listed in any order

``` zsh
    ls -la
```

![ls-la-flag](img/ls-la-flag.png "Alternate Flag Modifier")
