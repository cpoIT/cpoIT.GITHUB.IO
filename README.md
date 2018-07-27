# Gitting Started

This repository is for storing what I learn about Git/GitHub. I hope others will find it useful as well. Jekyll automatically converts double dashes into single dashes. Triple dashes are converted into em dashes.

## Setting Up Git on a Mac
+ Download Git from [Homebrew](https://brew.sh/)
+ Run commands from the command line using the built-in Terminal or iTerm2.
  + `git --version` (list current version on local computer)
  + `git config --global user.name "Kat Fries"`
  + `git config --global user.email katherynejf@gmail.com`
  + `git config –list` lists all Git settings
  + `git config user.name` will provide user's name
  + `man git` (full Git manual)


## Command Line Basics
### Moving around the Command Line
+	**(*tab button*)**: complete the name of the directory/file
+	**clear**: clears the bash screen

### High-Level User Commands aka *Porcelain Commands*
+	**pwd (Print Working Directory)**: returns current path directory e.g.: 
      `pwd`
  ==> `/Users/katsmac`
+	**ls (List)**: lists files and directories, e.g.:

Applications	Desktop
Downloads		README.md
+	**cd (Change Directory)**:
  +	**cd ..**					move up one directory
  +	**cd Desktop/**			takes a directory name as an argument
  +	**cd Downloads/git_tutorial**	moves to a directory within a directory
+	**touch**: creates a new empty file inside the working directory or updates the access date of the file without opening, saving and closing the file. 
+	**mkdir**: create a new empty folder



+	**add**: 
+	**commit**: 
+	**push**: 
+	**pull**: 
+	**branch**: 
+	**checkout**: 
+	**merge**: 

### Low-Level Commands aka *Plumbing Commands*
+	**cat-file**: 
+	**hash-object**: 




# TO DO LIST
git --help
usage: git [--version] [--help] [-C <path>] [-c name=value]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial)
   clone      Clone a repository into a new directory
   init       Create an empty Git repository or reinitialize an existing one

work on the current change (see also: git help everyday)
   add        Add file contents to the index
   mv         Move or rename a file, a directory, or a symlink
   reset      Reset current HEAD to the specified state
   rm         Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect     Use binary search to find the commit that introduced a bug
   grep       Print lines matching a pattern
   log        Show commit logs
   show       Show various types of objects
   status     Show the working tree status

grow, mark and tweak your common history
   branch     List, create, or delete branches
   checkout   Switch branches or restore working tree files
   commit     Record changes to the repository
   diff       Show changes between commits, commit and working tree, etc
   merge      Join two or more development histories together
   rebase     Reapply commits on top of another base tip
   tag        Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch      Download objects and refs from another repository
   pull       Fetch from and integrate with another repository or a local branch
   push       Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
  
  GIT(1)                            Git Manual                            GIT(1)

NAME
       git - the stupid content tracker

SYNOPSIS
       git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p|--paginate|--no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>]
           <command> [<args>]

DESCRIPTION
       Git is a fast, scalable, distributed revision control system with an
       unusually rich command set that provides both high-level operations and
       full access to internals.

       See gittutorial(7) to get started, then see giteveryday(7) for a useful
       minimum set of commands. The Git User's Manual[1] has a more in-depth
       introduction.

       After you mastered the basic concepts, you can come back to this page
       to learn what commands Git offers. You can learn more about individual
Git commands with "git help command". gitcli(7) manual page gives you
       an overview of the command-line command syntax.

       A formatted and hyperlinked copy of the latest Git documentation can be
       viewed at https://git.github.io/htmldocs/git.html.

OPTIONS
       --version
           Prints the Git suite version that the git program came from.

       --help
           Prints the synopsis and a list of the most commonly used commands.
           If the option --all or -a is given then all available commands are
           printed. If a Git command is named this option will bring up the
           manual page for that command.

           Other options are available to control how the manual page is
           displayed. See git-help(1) for more information, because git --help
           ...  is converted internally into git help ....
           


