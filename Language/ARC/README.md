# ARC

## Tags

- Lisp
- Paul Graham

## New Approach

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
