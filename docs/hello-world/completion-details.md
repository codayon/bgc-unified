---
title: Compilation Details
description: A bit more about how to build C programs
sidebar_position: 3
---

Let's talk a bit more about how to build C programs, and what happens behind the scenes there.

Like other languages, C has _source code_. But, depending on what language you're coming from, you might never have had to _compile_ your source code into an _executable_.

Compilation is the process of taking your C source code and turning it into a program that your operating system can execute.

JavaScript and Python devs aren't used to a separate compilation step at all--though behind the scenes it's happening! Python compiles your source code into something called _bytecode_ that the Python virtual machine can execute. Java devs are used to compilation, but that produces bytecode for the Java Virtual Machine.

When compiling C, _machine code_ is generated. This is the 1s and 0s that can be executed directly and speedily by the CPU.

> Languages that typically aren't compiled are called _interpreted_
> languages. But as we mentioned with Java and Python, they also have a
> compilation step. And there's no rule saying that C can't be
> interpreted. (There are C interpreters out there!) In short, it's a
> bunch of gray areas. Compilation in general is just taking source code
> and turning it into another, more easily-executed form.

The C compiler is the program that does the compilation.

As we've already said, `gcc` is a compiler that's installed on a lot of Unix-like operating systems. And it's commonly run from the command line in a terminal, but not always. You can run it from your IDE, as well.

So how do we do command line builds?

## Building with `gcc`

If you have a source file called `hello.c` in the current directory, you can build that into a program called `hello` with this command typed in a terminal:

```sh
gcc -o hello hello.c
```

The `-o` means "output to this file". And there's `hello.c` at the end, the name of the file we want to compile.

If your source is broken up into multiple files, you can compile them all together (almost as if they were one file, but the rules are actually more complex than that) by putting all the `.c` files on the command line:

```sh
gcc -o awesomegame ui.c characters.c npc.c items.c
```

and they'll all get built together into a big executable.

That's enough to get started―later we'll talk details about multiple source files, object files, and all kinds of fun stuff.

## Building with `clang`

On Macs, the stock compiler isn't `gcc`―it's `clang`. But a wrapper is also installed so you can run `gcc` and have it still work.

You can also install the `gcc` properly through Homebrew or some other means.

## Building from IDEs

If you're using an _Integrated Development Environment_ (IDE), you probably don't have to build from the command line.

With Visual Studio, `CTRL-F7` will build, and `CTRL-F5` will run.

With VS Code, you can hit `F5` to run via the debugger. (You'll have to install the C/C++ Extension.)

With XCode, you can build with `COMMAND-B` and run with `COMMAND-R`. To get the command line tools, Google for "XCode command line tools" and you'll find instructions for installing them.

For getting started, I encourage you to also try to build from the command line―it's history!
