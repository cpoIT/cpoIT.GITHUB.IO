
# The Never Ending List & FILO Notebook

Next up: Start Learning React Again.

# A Bad Reaction to React

I love JavaScript. It is my first programming language (unless you count an intro to BASIC on my Commodore 64 using spaghetti code aka GOTO statements). And like all first loves, every other encounter will be compared to it. I like HTML and CSS (with and without LESS and/or Flexbox). They are straight-forward, clean, and get the job done, but they lack the complexity of JavaScript. So, when I read about JSX merging JS and HTML, I was intrigued. 

However, this romance has gotten off to a rocky start. With the end in sight (since my React localhost sites are a mess), I am already grieving what could have been. I quickly traversed through Denial and I am now stuck in Anger. To take the first step into bargaining with JSX, I decided to simultaneously continue on this path while returning to the beginning and write about this experience.

## React 101
**Add to never ending list**

## AJAX, CRUD, & JS Promises

What is the fastest way to get things done? One could spend a lot of time creating a Gannt chart to figure out the best order or you can wing it knowing that multitasking shorter tasks between longer tasks will be fastest. Sometimes you may want to set a timer (or [pomodoro](https://francescocirillo.com/pages/pomodoro-technique)) to help track when to do something.

**In JS, asynchronous code is a way to stagger tasks and add timers. Promises are a way to write asyncronous code using established design patterns.**

### It Begins with a JS Promise Primer

JS keeps it promises. Ask JS to log something 2 seconds after it was called and it does even while do other things even if things have changed in the Greenwich Mean Time. When asking for a new Promise, strings (no not those types of strings) can be attached (e.g., was the parameter less than 1000). If everything goes smoothly, resolve runs then; if not, reject is there to catch and throw and error. 

```
let bigBang = 0;

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
```

### AJAX: Asynchronous Javascript and XML

AJAX is not a new language, method, library, etc. It is a playbook of asynchronous best-methods.

1. Open a new React codesandbox;
2. Convert the App component to a class;
3. Add the following componentDidMount (CDM):
```
    componentDidMount() {
      console.log("inside CDM");
      fetch('https://dog.ceo/api/breed/husky/images')
        .then(res => res.json())
        .then(dogs => console.log("fetch completed");)
        .catch(err => console.log(err));
      console.log("below fetch");
    }
```
4. Open the project in a new browser, inspect it, click on newtork tab, then click on Headers, Preview, Response & Timing. 

### HTTP: Hypertext Transfer Protocol

Simplistically, the Chrome browser is the client communicationg to an application on a server. The client requests info and the server responds. HTTP is a set of rules to ensure clear and quick communication between the client and server during these request-respond communiques. 

Easiest way to increase speed? Lighten the load. But how can you increase speed and keep the fancy accouterment? Lighten the initial load and behind the scenes add more functionality as needed and/or between other tasks, which brings us back to asyncronous code.

### CRUD: Create, Read, Update, Delete

CRUD is a way to store information. Information is created, read, updated (as necessary), and eventually deleted. HTTP follows this method, with a slight deviation and different names. 

**Get**: Request to retrieve information.
**Post**: Add or update resources; server names URL object.
**Put**: Add or modify resources; client can name, multiply puts for the same object URL will not throw an error.
**Delete**: Remove information.


#### HTTP Status Code: I'm a Little Teapot

Everyone has seen a 404 code. Yesterday, I got a 500 HTTP Error code from Youtube with a code monkey. But have you heard of a 418 I'm a Little Teapot error code? Yeah, me neither, but it existed. Want to improve UI? Be like [Lego](https://www.lego.com/404) or [Pixar](https://www.pixar.com/404) and create a 404 page to have the user laughing instead of being irritated by your incompetence.

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
