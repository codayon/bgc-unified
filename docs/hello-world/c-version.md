---
title: C Version
description: C has come a long way over the years
sidebar_position: 4
---

C has come a long way over the years, and it had many named version numbers to describe which dialect of the language you're using.

These generally refer to the year of the specification.

The most famous are C89, C99, C11, and C23. We'll focus on the last one in this book.

But here's a more complete table:

| Version              | Description                                                                                                                                                                                                                                                                        |
| -------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| K&R C                | 1978, the original. Named after Brian Kernighan and Dennis Ritchie. Ritchie designed and coded the language, and Kernighan co-authored the book on it. You rarely see original K&R code today. If you do, it'll look odd, like Middle English looks odd to modern English readers. |
| **C89**, ANSI C, C90 | In 1989, the American National Standards Institute (ANSI) produced a C language specification that set the tone for C that persists to this day. A year later, the reins were handed to the International Organization for Standardization (ISO) that produced the identical C90.  |
| C95                  | A rarely-mentioned addition to C89 that included wide character support.                                                                                                                                                                                                           |
| **C99**              | The first big overhaul with lots of language additions. The thing most people remember is the addition of `//`-style comments. This is the most popular version of C in use as of this writing.                                                                                    |
| **C11**              | This major version update includes Unicode support and multi-threading. Be advised that if you start using these language features, you might be sacrificing portability with places that are stuck in C99 land. But, honestly, 1999 is getting to be a while back now.            |
| C17, C18             | Bugfix update to C11. C17 seems to be the official name, but the publication was delayed until 2018. As far as I can tell, these two are interchangeable, with C17 being preferred.                                                                                                |
| C23                  | The most recent specification.                                                                                                                                                                                                                                                     |

You can force GCC to use one of these standards with the
`-std=` command line argument. If you want it to be picky about the
standard, add `-pedantic`.

For example:

```sh
gcc -std=c11 -pedantic foo.c
```

For this book, I compile programs for C23 with all warnings set:

```sh
gcc -Wall -Wextra -std=c23 -pedantic foo.c
```
