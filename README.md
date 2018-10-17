# Gitting Started

This repository is for storing what I learn about Git/GitHub. I hope other Mac users will find it useful as well. 
Code and output are in `light grey boxes`. Sample output follows ==>.

## Setting Up Git on a Mac
+ Download Git from [Homebrew](https://brew.sh/)
+ Run commands from the command line using the built-in Terminal or iTerm2.
  + `git --version` (list current version on local computer)
  + `git config --global user.name "My Name"`
  + `git config --global user.email myemail@gmail.com`
  + `git config –list` lists all Git settings
  + `git config user.name` will provide user's name
  + `man git` (full Git manual)


## Command Line Basics
### Moving around the Command Line
+	**(*tab button*)**: complete the name of the directory/file
+	**clear**: clears the bash screen

### High-Level User Commands aka *Porcelain Commands*
+	**pwd (Print Working Directory)**: returns current path directory e.g.:  
```pwd```  
  ==> ```/Users/katsmac```
+	**ls (List)**: lists files and directories, e.g.:  
```ls```
==>
```Applications	Desktop```  
```Downloads		JStodo.txt```

+	**cd (Change Directory)**:
  +	**cd ..** moves up one directory
  + **cd ~** moves to root directory
  +	**cd Desktop/**	takes a directory name as an argument (great place to use the tab button to complete the directory name).
  +	**cd Downloads/git_tutorial**	moves to a directory within a directory
+	**touch**: creates a new empty file inside the working directory or updates the access date of the file without opening, saving and closing the file. 
+	**mkdir**: create a new empty folder

#### Add, Commit, Push, Pull: Rinse & Repeat

+	**add**: once in the current directory to add all files: ```git add .```
+	**commit**: commit the add with a meaningful message: ```git commit -m "Finished component X. Next up, component Y."```
+	**push**: push the committed and added files with ```git push```
+	**pull**: go to get hub and create a pull request.
+	**branch**: 
+	**checkout**: 
+	**merge**: 

### Low-Level Commands aka *Plumbing Commands*
+	**cat-file**: 
+	**hash-object**: 

# A Bad Reaction to React




# TO DO LIST



