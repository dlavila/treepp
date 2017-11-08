
Modern C++ Challenge:
======

The purpose of this challenge is to write a small application to demonstrate the usage of Modern C++ features and libraries. What better to learn some of the concepts presented at [MeetingCpp] than solving a real problem? 

The challenge is to write a simple and portable version of the Linux command line tool [tree]:

tree
------

`tree` is a recursive directory listing program that produces a depth indented listing of files. With no arguments, `tree` lists the files in the current directory. When a directory argument is given, `tree` lists all the files and/or directories found in the given directory.
Upon completion of listing all files/directories found, `tree` returns the total number of files and/or directories listed.

The output takes a graphical form which will resemble the following example:

```
.
├── config.xml
├── config.json
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

2 directories, 11 files
```

By default folders and files are sorted in alphabetical order as shown in the example.
For simplicity you can assume only folders and files in the path.

Your implementation of `tree` should understands the following command line switches (one at the time):

```
-d: List directories only.
-t: Sort the output by last modification time.
--dirsfirst: List directories before files.
-L level: Max display depth of the directory tree.
```

You are free to use any C++17/14 feature, and open source library from this [list]. The solution should be limited to one source file and must include the command to compile (no make/ninja/etc files) in a comment. 

To submit your solution send us an [email](mailto:dlavila@uc.cl) with a link to a place where we can find your code (we recommend using something like [Wandbox], [Coliru] or doing a pull request direclty to the challenge repo). Anyone can participate but for strategic reasons winners will be selected among MeetingCpp attenders.

To encourage discussion and learning all the solutions are going to be made public after announcing the winner(s). 

[MeetingCpp]: https://www.meetingcpp.com
[Wandbox]: https://wandbox.org
[Coliru]: http://coliru.stacked-crooked.com
[tree]: https://linux.die.net/man/1/tree
[boost::hana]: http://www.boost.org/doc/libs/1_61_0/libs/hana/doc/html/index.html
[list]: https://github.com/mattgodbolt/compiler-explorer/wiki/Installed-libraries
