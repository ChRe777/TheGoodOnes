# Unix

## Tags

- Plan 9
- Dennis Ritchie
- ...

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
