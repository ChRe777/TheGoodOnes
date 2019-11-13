# Plan 9

## Tags

- Everything is a file
- Microkernel
- Clean

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
[https://en.wikipedia.org/wiki/Fossil_(file_system)](Fossil)
https://en.wikipedia.org/wiki/Fossil_(file_system)

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
