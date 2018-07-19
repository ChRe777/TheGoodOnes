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

#### Why Plan9?

[https://www.mail-archive.com/9fans@9fans.net/msg17067.html]([9fans] So, why Plan 9?)

#### What people say

https://www.mail-archive.com/9fans@9fans.net/msg17073.html

Most of the people who can answer best are currently at the Plan 9 Workshop
(http://www.iwp9.org/), so they'll doubtless chip in a wee bit later.

Plan 9 is a research OS that has had a **quite amazing impact** on most other
Unix type OSes. For example: **UTF-8**, **process filesystem** (generalised to "use
a filesystem as a well defined abstraction mechanism"), **recursive window
systems** (ie. a full windowing system inside a window, not 100% sure who did
it first, but the Plan 9 one is **amazingly consistent** and so **easy to use** it
makes others look clunky), and **full historical filesystem** (**remember
everything you ever did using snapshots**).

Plan 9 is not a polished end user OS!

Robby

---

Oh, and most of the Plan 9 tools were first made available to use outside
the Plan 9 OS through Russ Cox's plan9 in user space effort (
http://swtch.com/plan9port/). And there's the virtualisation project vx32
that includes Plan 9 as an example. Not sure how they fit into a holistic
view. They're more like pragmatic ways forward when you can't (or don't want
to) run a stand alone OS.

One of the **great things** in Plan 9 is the **readability of the code**. You can
actually dive in and **see how it all works** without needing an augmented
brain. Although it may require adjusting your thinking to a "let's try to
**manage all this complexity** a bit better" mindframe. And that can take a bit
of time and effort. But it's well worth it.

Robby

---

> why anyone should care about Plan 9 anyway

Because: **getting things right the first time** around is much more of a
practical matter than you may at first realize.


Nick

---

Very succinct, and better than I could do 'til the coffee kicks in.

You could have **pointed out** that the **entire source tree is smaller than
the gcc manual.**


But as I say - do what you like. I know people who would rather spend
$5k on an Apple PC than $200 on a slicker plan9 box. I have my FS
(venti + fossil) on a USB wristband. Take that penguin heads.

Just the semi-delirious jots from early morning brucee.

---

**getting it right**:

- **less code** in plan 9 than in most configure scripts (hard to believe but true)
- plan 9 memory management code is 1 file, linux is 55
- almost no assembly in plan 9 ; # lines  assembly is GROWING in linux
- growth of linux code size is exponential (this is part of the
getting it right issue)


it's **always good to have a system** that gets closer to **getting it right**
around, as a **reminder if nothing else**.

ron

---

Well, I think it depends also on who one is and what one can afford to do at a 
point in time. And "afford" isn't necessarily only measured in dollars :)


I would much rather spend **$200 on a slick Plan9 box**, but I can't afford, given 
my current state of texpertise, to risk a government-funded project on a 
research O/S where support is more difficult. So an Apple it is, for the time 
being (for a lot less than $5000, btw...)

That's not to denigrate Plan9 by any means. I'm looking at it, like it, and 
hope to continue learning the ropes. But at the immediate moment, I don't 
really have a realistic choice, even given that the help I've got from people 
on this list has been **fantastic**. So for me, the short term solution is the 
Apple, and ideally, the **long-term solution will be Plan9**.

KarkJurgen

---

I'm probably not the best person to try to present the holistic
view, but I will anyway.  To understand where Plan 9 came
from, we first have to understand how UNIX developed.  In the
late '80s, UNIX was about 20 years old and had not aged too
gracefully.  In particular, as Sun said, the network had become
the computer, and UNIX networking was kind of bolted onto
the side of the system.  Similarly, graphical interaction had
become ubiquitous well after UNIX had originally been designed.
The way I like to describe it is that the Bell Labs guys at this
time decided to take **20 years of UNIX experience** and **start
over again** and **do it right**, applying that experience.  The
**result was Plan 9**.

There are 5 main approaches to having the Plan 9 experience.
First, the "real" Plan 9 experience requires a network of machines
including file servers, CPU servers, and terminals.  Of course,
the original Plan 9 systems ran natively on bare hardware,
and it still happily runs on a lot of hardware.  The biggest
problem with just grabbing a bunch of random hardware
and running Plan 9 on it is the problem of drivers for random
PC hardware.  But a lot of us do run Plan 9 on bare hardware
and it's a refreshing experience after years of UNIces.  I
should also point out that Plan 9 has from the very beginning
been built around running on a variety of hardware and
today runs on everything from tiny gumstix machines to
Blue Gene/P.

The second major approach is **running Plan 9 on** simulators
and **virtual machines**.  Most of us have had varying degrees
of success running Plan 9 "networks" on instances of qemu
or vmware or xen or...  This is a pretty good way to mitigate
the hardware support issues.  It's also a nice way to set up
and test distributed things while sitting with a single laptop
in a hotel room.

If you have a real Plan 9 cpu server, but don't have a
Plan 9 terminal for accessing it, you can use the application
drawterm.  It is an interesting modification of the Plan 9
kernel running as an X11 application.  Unlike a real terminal,
it doesn't run any Plan 9 applications locally on the terminal,
but it does give you an interface to a real Plan 9 system.

Over time, many people who at one time used Plan 9 as
their main systems, were pulled away and found themselves
back on UNIX-like systems.  For a period of time, there were
several projects that implemented Plan 9 inspired tools for
UNIX and X11.  This is where P9P (aka Plan 9 from User Space)
comes in.  Russ Cox ported the bulk of the Plan 9 application
set to UNIX-based systems.  With these, you can have a user
environment that looks a lot like Plan 9, complete acme and
sam.

Later, Russ also developed the vx32 virtualization and the
implementation of Plan 9 on it.  This is 9vx which allows you
to run an instance of Plan 9 as user application.  9vx is
essentially a port of the Plan 9 kernel to the vx32 platform.
It's great as it allows you to run a "real" Plan 9 terminal as
an application on a more traditional system.  You can run it
stand-alone with the root taken from your host system, or
you can run it as a terminal that takes its root from a Plan 9
file server.

As I sit here at IWP9, I am typing this in acme in 9vx running
on FreeBSD, using the rio port in P9P for my window manager.
Because I'm away from my home network, I'm running 9vx
with the the root on my local machine.  When I'm at home, I
use 9vx booting with its root taken from a real Plan 9 file
server.  I also run it on qemu fairly often.  The bottom line
is that there are quite a **variety of ways to work with Plan 9**
and they **are all useful** in their own ways.

I've been too long-winded as it is, so I'll stop now.  Hopefully,
I haven't said anything that's too far off base.

BLS

---

Why Plan 9?

Because on one of these days some big company (hint: where are the ex Bell
Labsers working with a very much Plan 9 / inferno / Limbo insipired new
programming language) adopts the Plan 9 / Inferno in a a more or less varied
incarnation. I could imagine Android having a new kernel not tied to Java
only, and supporting a **rich ecosystem of distributed 9P objects**...


 It is going to be big. It does not have to be **Google**. Someone will do it. I
hope. *Wish. Dream.*

In the end I can't make up my mind, about what is the *single greatest idea*
in the Plan 9 culture. But if pressed I suggest it is **9P** and the idea, that
we really **do not need protocols** above the network layer, but HTTP, SMTP,
DNS, SOAP, IIOP, IMAP, IRC, SSH, SSL, TP, SNMP and hundred others can *all be
replaced by "remote file access"*. And at the same time with file system
union directories you can also "inherit" and "augment" any of the
"services". This essentially gioves you distributed objects (with natural
persistence option). And this all can be done *securely with authenticator*
handles and the Factotum agent. **It is safe enough** to be run over the **public
internet**.

Anssi

---

the **twitter example** you gave is perhaps too simple, could the tweets
not just be text written to a **publicly writable file**. the users could connect
with 9p but as the user none son they will need no auth.


**better examples** of the everything is a **file aproach are wikifs** (a file server 
which
prvides **virtual files** for the httpd server (or any normal 9p file client)
to access and stores a database of wiki pages.
http://plan9.bell-labs.com/magic/man2html/4/wikifs

the cassic example is using a **plan9 server** as a **gateway machine across a 
firewall**.
This machine is dual homed and all machines inside the firewall are isolated.
when one of these machines wants to connect to somone outside the firewall they
can just import the gateway's /net.alt over the top of their own. (by tradition
the primary interface is mounted on /net and the seccondary at /net.alt)

Now any DNS lookup and  socket connection will be made using the gateway's 
internet
facing NIC. This is all done using the **9p protocol**, no clever IP routing etc.
if the 9p connection to the hateway happens to come over an ssh session,
ppp, or pigeon, it doesn't matter, you are sharing files, and these particular
files give you access to that machines network interface.

there is also a really neat trick you can use do a similar thing with a unix
machine as the gateway - sshnet provides a /net like interface to plan9 but uses
ssh's remote port forwarding to speak to unix:
http://plan9.bell-labs.com/magic/man2html/1/ssh

-Steve

---

For any use-case I personally care about (and probably any
workstation/server use case you care about as well,) the Linux kernel
with the GNU userspace will blow anything out of the water, both in
performance and usability. If you don't recognize this you're sticking
your head in the sand. I know **P9 is faster** in many ways, but have you
tried comparing performance figures with, say, browser rendering times,
Doom 3, or some video transcoder? Exactly.


However, projects like Linux and P9 can and should coexist, because
they complement each other. The developers of research OSs get a lot
more freedom to do research advance the state of the art. In fact, I'd
say P9 has contributed at least as much to the state of open-source OS
development as Linux has. Certainly, the Linux kernel uses a lot of
techniques that could **only** have been **incubated within a research OS**.
(/proc... what a wacky idea! But a good one.)

So, there are two reasons to use (and port your software to) Plan 9.
-First of all, you get a preview of what Unix development is probably
going to look like in a few years-- increased depreciation of ASCII for
Unicode, resource shared between computers, and so on. 
-Second of all, Plan 9 is just **SO DAMN FUN to play with**.

-Max

---

2010/10/12 Max E <maxxed...@comcast.net>:
> For any use-case I personally care about (and probably any
> workstation/server use case you care about as well,) the Linux kernel
> with the GNU userspace will blow anything out of the water, both in
> performance and usability.


I don't think the GNU userspace is more usable. Compare the bash and
rc man pages and tell me which one you find easier to use. From my
point of view **consistency and simplicity** **increase usability**. Both of
these **qualities are difficult to find** in *GNU software*.. If you don't
recognize this *you're sticking your head in the sand*.

-- 
- yiyus || JGL . 4l77.com

#### Design of Plan9

[http://doc.cat-v.org/plan_9/1st_edition/designing_plan_9] (DESIGNING PLAN 9)

#### History (see Wiki)

Plan 9 from Bell Labs was originally developed, starting mid-1980s, by members of the Computing Science Research Center at Bell Labs, the same group that originally developed Unix and C.[8] The Plan 9 team was initially led by *Rob Pike*, *Ken Thompson*, *Dave Presotto* and Phil Winterbottom, with support from *Dennis Ritchie* as head of the Computing Techniques Research Department. Over the years, many notable developers have contributed to the project including Brian Kernighan, Tom Duff, *Doug McIlroy*, *Bjarne Stroustrup* and Bruce Ellis.[9]

#### Useful Links

[http://www.iwp9.org/](Papers and Slides from *8th International Workshop on Plan 9*)

### Fuchsia OS (Google)

Fuchsia is a capability-based operating system currently being developed by Google. It first became known to the public when the project appeared on GitHub in August 2016 without any official announcement. In contrast to prior Google-developed operating systems such as Chrome OS and Android, which are based on Linux kernels, Fuchsia is based on a new microkernel called **"Zircon"**, derived from **"Little Kernel"**,[1][2] a small operating system intended for embedded systems, which was developed by *Travis Geiselbrecht*, a creator of the *NewOS* kernel used by *Haiku OS*.

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






