---
title: I Started Learning C/C++
date: 2017-12-19 00:00:00 Z
categories:
- code
tags:
- c
- cpp
- emacs
- c++
layout: article
author: Me
---

I actually used to learn C back in the days when I thought I needed to run a lot of simulatinos on the local computer(s), which is difficult to do with Matlab. I am doing it through Coursera and the course is provided by Duke University. I am also taking Introduction to C++ through EdX Microsoft. The C++ course runs faster as they target students who already know some programming.

I like the fact that the Coursera course use gcc to compile and emacs for the editor. I will use the same enviornment for the C++ course while they of course use Visual Studio in the video lessons. Not only it would be good to use those simplest tools to learn programming to get to become familar with the process of transitioning the code you write to the executable, but also that's the exact development environment I used back in the days when those fancy IDEs like Xcode wasn't avaiable and the Visual Studio was difficlt to figure out how to use with the limited resources freely available and without being in the coding community. 

Given you wrote a .c program (source code) in Emacs, say hello.c, you go back to the terminal by suspending Emacs with `ctr` + `z`, and there type
```terminal
gcc hello.c
``` 
This command produces `a.out` which is actually executable by typing `./a.out` where `./` indicates to run the executable located in the current directory. I believe the common mistake is to type `a.out`. Don't ask me why the system doesn't let it work.

You can name the executable file and do some fancy things that the gcc complier provides by giving some options in the commond line:
```terminal
gcc -Wall -o hello hello.c
```
where `-o hello` indicates that the [o]utput is named `hello` instead of the default name `a.out`. `-Wall` option has something to do with warnings that the complier may or may not issue. Its detail of what it helps you is relegated to some google search. You can run the program by typing `./hello` on the terminal.

The course suggests to use more optional arguments as
```
gcc -o hello -Wall -Werror -pedantic -std=gnu99 hello.c
```
At this moment, I don't worry about thoes extra options.

Now, I make a note of Emacs tutorials.

| What you want        | Command  |
| ------------- |:-------------:| -----:|
| save file      | `ctr` + `x` and `s` |
| suspend emacs to come back to the console     | `ctr` + `z`  |
| get back to emasc where you were  | `fg` in the terminal |