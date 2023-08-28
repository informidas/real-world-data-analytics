# Navigating Nested Folders in Terminal 
Once you master the basic commands of terminal, the remaining challenege is traversing the tree-like hierarchy of the storage volume. This is faciliated by using absolute and relative paths.

## Absolute Paths
Absolute path requires an explicit reference to a directory or file using a fully qualified path inclusive of the root of the file.

BENEFIT: The path to the directory or file being references is fully qualified and avoids reliance on being in a special folder whne executing the command.

## Relative Paths
Relative path requires a reference to a directory or file based on the current location from which the command is being made.

BENEFIT: The path to the directory often requires less typing.  

## Special Folder reference  (Relative Paths)
To navigate to a directory one level up from the current path use teh following command:

``` zsh
    cd ..
```

see example below
![one-directory-up](img/one-directory-up.png "One Directory Up")

To navigate 2 levels up from the current path use the following command:

``` zsh
    cd ../..
```

see example below
![2-directories-up](img/[two-directories-up.png "Two Directories Up")
