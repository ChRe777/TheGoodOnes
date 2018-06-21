# The Good Ones

Today it is hard to find some good ones. Because everyone had their opinions 
(and opinions are often like noses) how to develop software.

A collection of the good ones. 

A try to collect the good stuff I found over past the years (since 2000)

I believe that good product could not be mass product.

Good vegetables you will find on a small vegetables market of farmers.

I believe in the lego principe And keep it simple. 
Most projects I saw with high level of complexity. 
That means you have no simple lego stones, but very complex one.

## Design

Design a software like building a house. First you need to know what to build.
Make a plan and build if up layer by layer. Do not build the house from the roof.
But always have the overview of the end result. Most do not know the end result, build something and change it and change it.
If you change to often you get in a total mess which needs a lot of energy to keep it alive.

## APIs

I believe that it much better not to be bride and get a hacker, but rather look
at good apis and look how they made it then to create your own one's.

### Maya API

http://docs.autodesk.com/MAYAUL/2014/ENU/Maya-API-Documentation/

### MSDN - Examples lead to Bad Code

I believe that the examples in MSDN leads to bad programer pratice we all face of our colleagues.
If a example writer writes an example of for instance loading something from the db and
put into a dataview. He leads people to do this is production code. 
The purpose was to give a simple example. But in reality you should not do that.
A good programer would do this in the event handler. But write a command and has different
layers in the code. Would have an api. Would a MVP Pattern or some layers of abstractions. Whatever.

## Programming Languages

### Go

Go (often referred to as Golang) is a programming language created at Google[11] in 2009 by *Robert Griesemer*, *Rob Pike*, and *Ken Thompson*.[9] Go is a statically typed compiled language in the tradition of C, with memory safety, garbage collection, structural typing,[2] and CSP-style concurrent programming features added.[12] The compiler, tools and source code are all free and open source.[13]

Go is recognizably in the tradition of C, but makes many changes to improve brevity, simplicity, and safety. The language consists of:

A syntax and environment adopting patterns more common in dynamic languages:[27]
* Optional concise variable declaration and initialization through type inference (x := 0 not int x = 0; or var x = 0;).
   * Fast compilation times.[28]
   * Remote package management (go get)[29] and online package documentation.[30]
* Distinctive approaches to particular problems:
  * Built-in concurrency primitives: light-weight processes (goroutines), channels, and the select statement.
  * An interface system in place of virtual inheritance, and type embedding instead of non-virtual inheritance.
  * A toolchain that, by default, produces **statically linked native binaries** **without external dependencies.**
  * A desire to keep the language specification simple enough to hold in a programmer's head,[31] in part by omitting features which are common in similar languages.

### Oberon 2

- Oberon Compilers and Language reference material [http://www.ethoberon.ethz.ch/compiler](http://www.ethoberon.ethz.ch/compiler/index.html#report)

### Arc

Arc is Lisp. Paul Graham tried to get back in time and make a fresh start.

Lisp basically work with 7 primitives. Basic building stones:

1. car  
2. cdr
3. cons
4. atom
5. quote
6. eq
7. cond

The rest of the language can be written in the language itself by using this stones.
I call it the [Lego](https://en.wikipedia.org/wiki/Lego) principle. 
The 7 primitives of Lisp remembers me on a set of basic bricks in Lego. 

Graham added 3 new primitives to the core:

8. rep
9. tag
10. type

For instance with tag it is possible to "tag" a function as macro and use this 
information in eval to do a macex.

Read the Article ('Some Work on Arc') (http://www.paulgraham.com/ilc03.html)

- Arc Language Homepage of Paul Graham [http://arclanguage.org/](http://arclanguage.org/)

## Operation Systems

### Oberon

It is a small elegant operating system. It was ahead of his time and still is.

- ETH Oberon Home Page [http://www.ethoberon.ethz.ch/](http://www.ethoberon.ethz.ch/)

### Minix

Minix has a small stable kernel. 

A kernel is like the heart of the body it should never stop working.

The kernel could be overseen by one person.

Minix drivers for instance run like programms. If a driver crash, the driver will be restarted. 

- Minix 3 Homepage [http://www.minix3.org/](http://www.minix3.org/)

### BeOS / Haiku OS

Haiku OS is the open source project of BeOS. Build on NewOS Kernel 

### Plan9

#### History (see Wiki)

Plan 9 from Bell Labs was originally developed, starting mid-1980s, by members of the Computing Science Research Center at Bell Labs, the same group that originally developed Unix and C.[8] The Plan 9 team was initially led by *Rob Pike*, *Ken Thompson*, *Dave Presotto* and Phil Winterbottom, with support from *Dennis Ritchie* as head of the Computing Techniques Research Department. Over the years, many notable developers have contributed to the project including Brian Kernighan, Tom Duff, *Doug McIlroy*, *Bjarne Stroustrup* and Bruce Ellis.[9]

### Fuchsia OS (Google)

### Little Kernel

LK (Little Kernel) is a tiny operating system suited for small embedded devices, bootloaders, and other environments where OS primitives like threads, mutexes, and timers are needed, but there’s a desire to keep things small and lightweight. On embedded ARM platforms the core of LK is typically 15-20 KB.

LK was made by [Travis Geiselbrecht](https://github.com/travisg) see [Github](https://github.com/littlekernel/lk/)

## User Interface

### The Humane Interface

The ideas is this book are still ahead of time and will be. All current interface could not
changed because it would cause to make a fresh start. That no big company will do.

- The Humane User Interface Book in Wiki (https://en.wikipedia.org/wiki/The_Humane_Interface)

## Others

The basic idea of this book is to think in patterns. Keep thing simples and bring you code in order.
The humane brain for instance is a rule (pattern) extraction machine. Kids learn a language by
extract the pattern of the language by listen all day long to the parents. 
Read [Lernen-Gehirnforschung-die-Schule-Lebens](https://www.amazon.de/Lernen-Gehirnforschung-die-Schule-Lebens/dp/3827413966)

- Design Patterns - The Gang of Four

## Persons

- Jef Raskin [https://en.wikipedia.org/wiki/Jef_Raskin](https://en.wikipedia.org/wiki/Jef_Raskin)
- Donald E. Knuth [https://de.wikipedia.org/wiki/Donald_E._Knuth](https://de.wikipedia.org/wiki/Donald_E._Knuth)
- Niklaus Wirth [https://en.wikipedia.org/wiki/Niklaus_Wirth](https://en.wikipedia.org/wiki/Niklaus_Wirth)
- Paul Graham - [http://www.paulgraham.com/](http://www.paulgraham.com/)

- Ken Tompson
- Dennis Ritchie


## Books/Articles

Several ways to increase the [bus factor](https://en.wikipedia.org/wiki/Bus_factor) have been proposed:

* Reduce complexity
* Document all processes and keep that documentation up-to-date
* Encourage cross-training.

### Subject: Simplicity (Reduce Complexity)

- Eric S. Raymond - [The Art of Unix Programming](http://nakamotoinstitute.org/static/docs/taoup.pdf)
- Niklaus Wirth - [The School of Niklaus Wirth: The Art of Simplicity](https://www.amazon.de/School-Niklaus-Wirth-Art-Simplicity/dp/1558607234)
- Donald A. Norman - [Living with Complexity - Chapter 1](https://www.jnd.org/dn.mss/LWCChapter1.pdf)

### The Art of Unix Programming - Eric S. Raymond

Book [The Art of Unix Programming](http://nakamotoinstitute.org/static/docs/taoup.pdf).

#### Basics of the Unix Philosophy ####

The *Unix philosophy* originated with *Ken Thompson’s* early meditations on how to **design a small**
but capable operating system with a **clean service interface**. It grew as the Unix culture learned
things about how to get maximum leverage out of Thompson’s design. It absorbed lessons from
many sources along the way.
The Unix philosophy is not a formal design method. It wasn’t handed down from the high fastnesses
of theoretical computer science as a way to produce theoretically perfect software. Nor is it that
perennial executive’s mirage, some way to magically extract innovative but reliable software on too
short a deadline from unmotivated, badly managed, and underpaid programmers.
The Unix philosophy (like successful folk traditions in other **engineering disciplines**) is **bottom-up**,
not top-down. It is pragmatic and grounded in experience. It is not to be found in official methods
and standards, but rather in the implicit half-reflexive knowledge, the expertise that the Unix culture
transmits. It encourages a sense of proportion and skepticism — and shows both by having a sense
of (often subversive) humor.
*Doug McIlroy*, the inventor of **Unix pipes** and one of the founders of the Unix tradition, had this to
say at the time [McIlroy78]:

**(i)** Make each program do one thing well. To do a new job, build afresh rather
than complicate old programs by adding new features.

**(ii)** Expect the output of every program to become the input to another, as yet
unknown, program. Don’t clutter output with extraneous information. Avoid
stringently columnar or binary input formats. Don’t insist on interactive input.

**(iii)** Design and build software, even operating systems, to be tried early, ideally
within weeks. Don’t hesitate to throw away the clumsy parts and rebuild them.

**(iv)** Use tools in preference to unskilled help to lighten a programming task, even
if you have to detour to build the tools and expect to throw some of them out after
you’ve finished using them.

He later summarized it this way (quoted in A Quarter Century of Unix [Salus]):

  This is the Unix philosophy: Write programs that **do one thing** and **do it well**.
Write programs to **work together**. Write programs to handle **text streams**, because
that is a **universal interface**.

*Rob Pike*, who became one of the great masters of C, offers a slightly different angle in Notes on C
Programming [Pike]:

* *Rule 1.* You can’t tell where a program is going to spend its time. Bottlenecks
occur in surprising places, so don’t try to second guess and put in a speed hack
until you’ve proven that’s where the bottleneck is.

* *Rule 2.* Measure. Don’t tune for speed until you’ve measured, and even then don’t
unless one part of the code overwhelms the rest.

* *Rule 3.* Fancy algorithms are slow when n is small, and n is usually small. Fancy
algorithms have big constants. Until you know that n is frequently going to be
big, don’t get fancy. (Even if n does get big, use Rule 2 first.)

* *Rule 4.* Fancy algorithms are buggier than simple ones, and they’re much harder
to implement. Use **simple algorithms** as well as **simple data structures**.

* *Rule 5.* Data dominates. If you’ve chosen the **right data structures** and **organized
things well**, the algorithms will almost always be self-evident. Data structures,
not algorithms, are central to programming.

* *Rule 6.* There is no Rule 6.
  
*Ken Thompson*, the man who designed and implemented the first Unix, reinforced Pike’s rule 4 with
a gnomic maxim worthy of a Zen patriarch:
  
  When in doubt, use brute force.

More of the Unix philosophy was implied not by what these elders said but by what they did and the
example Unix itself set. Looking at the whole, we can abstract the following ideas:

1. **Rule of Modularity**: Write simple parts connected by clean interfaces.
2. **Rule of Clarity**: Clarity is better than cleverness.
3. **Rule of Composition**: Design programs to be connected to other programs.
4. **Rule of Separation**: Separate policy from mechanism; separate interfaces from engines.
5. **Rule of Simplicity**: Design for simplicity; add complexity only where you must.
6. **Rule of Parsimony**: Write a big program only when it is clear by demonstration that nothing else will do.
7. **Rule of Transparency**: Design for visibility to make inspection and debugging easier.
8. **Rule of Robustness**: Robustness is the child of transparency and simplicity.


#### Rule of Modularity: Write simple parts connected by cleaninterfaces.

As Brian Kernighan once observed, “Controlling complexity is the essence of computer programming”
[Kernighan-Plauger]. Debugging dominates development time, and getting a working system
out the door is usually less a result of brilliant design than it is of managing not to trip over your
own feet too many times.
Assemblers, compilers, flowcharting, procedural programming, structured programming, “artificial
intelligence”, fourth-generation languages, *object orientation*, and software-development methodologies
without number have been touted and *sold as a cure for this problem*. **All have failed** as
cures, if only because they ‘succeeded’ by escalating the normal level of program complexity to
the point where (once again) human brains could barely cope. As Fred Brooks famously observed
[Brooks], there is no silver bullet.
The **only way to write complex software** that won’t fall on its face is to hold its global complexity
down — to build it out of **simple parts connected by well-defined interfaces**, so that most **problems
are local** and you can have some hope of **upgrading a part without breaking the whole.**

#### Rule of Clarity: Clarity is better than cleverness.

Because **maintenance is so important and so expensive**, write programs as if the most important
communication they do is not to the computer that executes them but to the **human** beings who will
**read** and **maintain** the source code in the future (including yourself).
In the Unix tradition, the implications of this advice go beyond just **commenting your code**. Good
Unix practice also embraces choosing your algorithms and implementations for future maintainability.
Buying a small increase in performance with a **large increase** in the **complexity and obscurity**
of your technique is a bad trade — not merely because complex code is more likely to harbor bugs,
but also because complex code will be harder to read for future maintainers.
Code that is graceful and clear, on the other hand, is less likely to break — and more likely to be
instantly comprehended by the **next person to have to change it**. This is important, especially when
that next person might be yourself some years down the road.

  Never struggle to decipher subtle code three times. Once might be a one-shot
  fluke, but if you find yourself having to figure it out a second time — because the
  first was too long ago and you’ve forgotten details — it is **time to comment the
  code** so that the **third time** will be relatively **painless**.
  —
  HenrySpencer

#### Complexity vs. complicated

Some interesting from the book [Living with Complexity - Chapter 1](https://www.jnd.org/dn.mss/LWCChapter1.pdf)

> I distinguish between **complexity** and **complicated**. 
> I use the word “complexity” to *describe a state of the world*. 
> The word “complicated” describes a *state of mind*. 
> The dictionary **definition for “complexity”** suggests things with many intricate and interrelated parts, which is just how I use the term. 
> The **definition for “complicated”** includes as a secondary meaning “confusing,* which is what I am concerned with in my definition of that word. 
> I use the word “complex” to describe the state of the world, the tasks we do, and the tools we use to deal with them. I use the word “complicated” or “confused” to describe the psychological state of a person in attempting to understand, use, or interact with  something in the world. Princeton University’s WordNet program makes this point by suggesting that “complicated” means “puzzling complexity.” 

### Subject: Technical Documentation

I had a one day class about **technial Writing** documents held by Dr. Klaus Hofer from [usabilitymapping.com](http://usabilitymapping.com/what-is-usability-mapping/)

[Klaus Hofer Linked In](https://ca.linkedin.com/in/klaus-hofer-0547a41)

# Personal Experience 

## Good advice is expensive

* Never build huge monolith software system.

You will after years always end with a [Leaning Tower of Pisa](https://en.wikipedia.org/wiki/Leaning_Tower_of_Pisa)
In beginning you do not see that you build a leaning tower that will fall down. You will see it when it is to late.

* Build small modular components

Better is to build small components. Like small leaning towers. 
But if you see that one (of many) tower is going to become oblique then stop.
Never build a tower with 54 levels if the tower is oblique on the first level.

A Software goes into production and the leaning towers is full of people
you can not easy get refactor this building. This is the same with software.
Never build monotlith. They will get monsters sooner or later. And then it is
to late.

For example I believe Linux is a monolith compared to Minix Os. Which is a much better approach.






