---
title: What to Expect from C
description: C is a low-level language
sidebar_position: 1
---

> _"Where do these stairs go?"_ \
> _"They go up."_
>
> ― Ray Stantz and Peter Venkman, Ghostbusters

C is a low-level language.

It didn't use to be. Back in the day when people carved punch cards out of granite, C was an incredible way to be free of the drudgery of lower-level languages like assembly.

But now in these modern times, current-generation languages offer all kinds of features that didn't exist in 1972 when C was invented. This means C is a pretty basic language with not a lot of features. It can do _anything_, but it can make you work for it.

So why would we even use it today?

- As a learning tool: not only is C a venerable piece of computing history, but it is connected to the [flw[bare metal|Bare_machine in a way that present-day languages are not. When you learn C, you learn about how software interfaces with computer memory at a low level. There are no seatbelts. You'll write software that crashes, I assure you. And that's all part of the fun!

- As a useful tool: C still is used for certain applications, such as building operating systems or in embedded systems. (Though the Rust programming language is eyeing both these fields!)

If you're familiar with another language, a lot of things about C are easy. C inspired many other languages, and you'll see bits of it in Go, Rust, Swift, Python, JavaScript, Java, and all kinds of other languages. Those parts will be familiar.

The one thing about C that hangs people up is _pointers_. Virtually everything else is familiar, but pointers are the weird one. The concept behind pointers is likely one you already know, but C forces you to be explicit about it, using operators you've likely never seen before.

It's especially insidious because once you _grok_ pointers, they're suddenly easy. But up until that moment, they're slippery eels.

Everything else in C is just memorizing another way (or sometimes the same way!) of doing something you've done already. Pointers are the weird bit. And, arguably, even pointers are variations on a theme you're probably familiar with.

So get ready for a rollicking adventure as close to the core of the computer as you can get without assembly, in the most influential computer language of all time^[I know someone will fight me on that, but it's gotta be at least in the top three, right?. Hang on!
