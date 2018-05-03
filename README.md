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

Haiku OS is the open source project of BeOS. Build on NewOS Kernel.

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

## Books/Articles

Several ways to increase the [bus factor](https://en.wikipedia.org/wiki/Bus_factor) have been proposed:

* Reduce complexity
* Document all processes and keep that documentation up-to-date
* Encourage cross-training.

### Subject: Simplicity (Reduce Complexity)

- Eric S. Raymond - [The Art of Unix Programming](http://nakamotoinstitute.org/static/docs/taoup.pdf)
- Niklaus Wirth - [The School of Niklaus Wirth: The Art of Simplicity](https://www.amazon.de/School-Niklaus-Wirth-Art-Simplicity/dp/1558607234)
- Donald A. Norman - [Living with Complexity - Chapter 1](https://www.jnd.org/dn.mss/LWCChapter1.pdf)


#### Some interesting Rules 

Some interesting Rules from the book [The Art of Unix Programming](http://nakamotoinstitute.org/static/docs/taoup.pdf).

1. **Rule of Modularity**: Write simple parts connected by clean interfaces.
2. **Rule of Clarity**: Clarity is better than cleverness.
3. **Rule of Composition**: Design programs to be connected to other programs.
4. **Rule of Separation**: Separate policy from mechanism; separate interfaces from engines.
5. **Rule of Simplicity**: Design for simplicity; add complexity only where you must.
6. **Rule of Parsimony**: Write a big program only when it is clear by demonstration that nothing else will do.
7. **Rule of Transparency**: Design for visibility to make inspection and debugging easier.
8. **Rule of Robustness**: Robustness is the child of transparency and simplicity.

#### Complexity vs. complicated

Some interesting from the book [Living with Complexity - Chapter 1](https://www.jnd.org/dn.mss/LWCChapter1.pdf)

I distinguish between **complexity** and **complicated**. I use the 
word “complexity” to *describe a state of the world*. The word 
“complicated” describes a *state of mind*. The dictionary defini-
tion for “complexity” suggests things with many intricate and in-
terrelated parts, which is just how I use the term. The definition 
for “complicated” includes as a secondary meaning “confusing,” 
which is what I am concerned with in my definition of that word. 
I use the word “complex” to describe the state of the world, the
tasks we do, and the tools we use to deal with them. I use the 
word “complicated” or “confused” to describe the psychological 
state of a person in attempting to understand, use, or interact with 
something in the world. Princeton University’s WordNet program 
makes this point by suggesting that “complicated” means “puz-
zling complexity.” 
