
# The Never Ending List & FILO Notebook

Next up: Start Learning React Again.

# A Bad Reaction to React

I love JavaScript. It is my first programming language (unless you count an intro to BASIC on my Commodore 64 using spaghetti code aka GOTO statements). And like all first loves, every other encounter will be compared to it. I like HTML and CSS (with and without LESS and/or Flexbox). They are straight-forward, clean, and get the job done, but they lack the complexity of JavaScript. So, when I read about JSX merging JS and HTML, I was intrigued. 

However, this romance has gotten off to a rocky start. With the end in sight (since my React localhost sites are a mess), I am already grieving what could have been. I quickly traversed through Denial and I am now stuck in Anger. To take the first step into bargaining with JSX, I decided to simultaneously continue on this path while returning to the beginning and write about this experience.

## React 101


## AJAX & CRUD

### It Begins with a JS Promise

JS keeps it promises. Ask JS to log something 2 seconds after it was called and it does even while do other things. When asking for a new Promise, strings (no not those types of strings) can be attached (e.g., was the parameter less than 1000). If everything goes smoothly, resolve runs then; if not, reject is there to catch and throw and error. 

**In fancy terms, promises are a way to write asyncronous code using an established design pattern.**

`let bigBang = 0;

const bigBangTimer = timeValue => {
  return new Promise((resolve, reject) => {
    setTimeout(() => {
      bigBang = timeValue;
      return bigBang < 1000 ? reject(bigBang): resolve(bigBang);
    }, timeValue);
  })
}
console.log('before call')
bigBangTimer(2000)
    .then(response => console.log('Resolved in', bigBang/1000, 'second(s)'))
    .catch(error => console.log('Error:', error));
console.log('after call')


// before call
// after call
// Resolved in 2 second(s)`

### CRUD: Create, Read, Update, Delete


Get
Post
Put
Delete

HTTP / AJAX I
In this module we’ll learn how to perform asynchronous requests in order to retrieve, create, modify, or remove information that exist on external servers.

At the end of this module, you should be able to:
describe promises and demonstrate the use of the `.then` and `.catch` methods
explain what AJAX stands for, it's benefits and how to make AJAX requests from a React Application
explain what HTTP is and the methods used to perform CRUD operations
make GET requests to an external API using axios


# Gitting Started

This repository is for storing what I learn about Git/GitHub. I hope other Mac users will find it useful as well. 
Code and output are in `light grey boxes`. Sample output follows ==>.

## Setting Up Git on a Mac
+ Download Git from [Homebrew](https://brew.sh/)
+ Run commands from the command line using the built-in Terminal or iTerm2.
  + `git --version` (list current version on local computer)
  + `git config --global user.name "My Name"`
  + `git config --global user.email "myemail@gmail.com"`
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
