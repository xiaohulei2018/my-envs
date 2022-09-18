# Bash Overview

## What is Bash

- Shell: A (possibly interactive) command interpreter, acting as a layer between the user and the system.
  - Interactive mode: A mode of operation where a prompt asks you for one command at a time.
  - Script: A file that contains a sequence of commands to execute one after the other.
- BASH is an acronym for Bourne Again Shell. It is based on the Bourne shell and is mostly compatible with its features.
- Shells are command interpreters.
  - They are applications that provide users with the ability to give commands to their operating system interactively, or to execute batches of commands quickly.
  - In no way are they required for the execution of programs; they are merely a layer between system function calls and the user.
- Think of a shell as a way for you to speak to your system.
  - our system doesn't need it for most of its work, but it is an excellent interface between you and what your system can offer.
  - It allows you to perform basic math, run basic tests and execute applications.
  - More importantly, it allows you to combine these operations and connect applications to each other to perform complex and automated tasks.
- BASH is not your operating system.
  - It is not your window manager.
  - It is not your terminal (but it oftens runs inside your terminal). 
  - It does not control your mouse or keyboard. It does not configure your system, activate your screensaver, or open your files when you double-click them.
  - It is generally not involved in launching applications from your window manager or desktop environment.
  - It's important to understand that BASH is only an interface for you to execute statements (using BASH syntax), either at the interactive BASH prompt or via BASH scripts.

## Types of Commands

- Aliases
  - Only used interactive shells, not in scripts
  - Only useful as simple textual shortcut
  - To have more flexibility, use a function
- Functions
  - Can be used on scripts
  - Contains shell commands
  - Act very much like a small script
  - They can even take arguments and create local vars
- Builtins
  - Some basic commands builtin the shell itsell, rather than a executable on the file system
  - Example: cd, echo, …
  - To get a list of builtins: $help
- Keywords
  - Keywords are like builtins, with the main difference being that special parsing rules apply to them.
- Executables
  - Executables may also be called external commands or applications.
  - A Program
  - PATH
- Question: How to find out the type of a command?
  - $type

### Review

- Alias — a word that is mapped to a string. Whenever that word is used as a command, it is replaced by the string it has mapped.
- Function — a name that is mapped to a set of commands. Whenever the function is used as a command, it is called with the arguments following it. Functions are the basic method of making new commands.
- Builtin — certain commands have been built into Bash. These are handled directly by the Bash executable and do not create a new process.
- Executable — a program that can be executed by referring to its file path (e.g. /bin/ls), or simply by its name if its location is in the PATH variable.
