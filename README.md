
The purpose of this challenge is to write a small application to demonstrate the usage of modern C++ features and libraries. 

The challange is to write a simple and portable version of the linux command line tool tree:

Tree is a recursive directory listing program that produces a depth indented listing of files. With no arguments, tree lists the files in the current directory. When a directory argument is given, tree lists all the files and/or directories found in the given directory.
Upon completion of listing all files/directories found, tree returns the total number of files and/or directories listed.

The output takes a graphical form which will resemble the following example:

```
.
├── config.xml
├── data
│   ├── data1.bin
│   ├── data2.sql
│   └── data3.inf
├── code
│   ├── templates.h
│   ├── nullptr.rs
│   └── monad.hs
├── program.exe
├── lib1.so
└── lib2.dll

2 directories, 10 files
```

By default folders and files are sorted in alphabetical order as depicted in the previous example.
For simplicity you can assume only folders and files in the path.

The program should handle the following options (one at the time):

```
-d: List directories only.
-t: Sort the output by last modification time.
--dirsfirst: List directories before files.
-L level: Max display depth of the directory tree.
```

You are free to use any C++17/14 feature or open source library(1). The solution should be limited to one source file. To encourage discussion and learning all the solutions are going to be made public after announcing the winner(s).

(1) The library should be portable or quasi-portable (complies with the standard but is limited by some compilers, think hana), some ideas: ranges v3, gsl, absl.
