---
date: 2022-10-05
---

# Computer Science Curriculum - discussion

_what classes are like the important core classes you should know about?_

- really depends on your goal
-  the highest leverage stuff cuts across classes
- (tips: understanding the difference between similar concepts is often more useful than mastering one of them)
- so whatever the way you'll get the explanation, it would be better to code a little bit

_JavaScript/typescript, shell, lua, AppleScript, (css)_


## Resources

- [Crash Course on Computer Science - YT](https://www.youtube.com/watch?v=tpIctyqH29Q&list=PL8dPuuaLjXtNlUrzyH5r6jN9ulIgZBpdo)
- [Harvard's CS50: Introduction to Computer Science](https://pll.harvard.edu/course/cs50-introduction-computer-science?delta=0) (free to learn, paid to be certified ?)

## Concepts

- manipulating various data structures (tree, graph, ..)
    having a deeper understanding of how data is structured at different levels of software is a huge boon, even as a pure end user
    understanding trees and graphs has probably a lot of everyday usages
- Computational complexity is also handy
    knowing how to estimate the big O of your code is good
    it's really easy to accidentally hit quadratic time when you could have it in linear or at least polynomial ( if you use a different data structure )
- Math field: set and graph theory
    Composition of those two tools can effectively model a huge swath of very important, very relevant systems
    Set theory is the **basis for typing in programming language**
    If you're using an SQL database, understanding what a trie actually is means you can make more informed choices about your indices
    - **SQL**
- some concepts about how network/internet works
  - learning about the [[networking_layers-OSI|OSI stack]] might be neat
      networking is importannt - TCP, UDP, BGP
- knowing a little bit about two coding languages with different concepts (object, functional, ..)
  - Pretty much all the popular languages do both [object and functional] nowadays so I feel like at a certain point the difference is more academic than anything else
  - Still important to know the difference between the two if you're programming at all
  - most of modern language do provide functions and object, but to do some real functional programming, or real object programming, or whatever the language paradigm
  - for coding in real life you don't need to follow one paradigm, but having some background in at least two of them makes you a better developer
  - Functional programming harnesses a lot of concepts that are just straight maths. So you might have encountered them before from other fields. Like first year university level maths, not school
- Code testing
  - Unit testing
- Programming language types (_typescript_ !!)
- Call by reference vs call by values
- exceptions handling
- Game development
  - it can be a good way to learn OO if you're interested in it, it's a domain that lends itself well to objects
  - And there's a bunch of good Lua game engines

### System Administration

- [Course about Shell](https://missing.csail.mit.edu/2020/course-shell/)

## More advanced concept of code/programming language design

_Don't worry too much about this yet_

### dependency injection

The basic principle is to take (as an argument or field or whatever) all external dependencies, so you can treat entire systems as black boxes
Like, don't import your logging class into your DB access layer, inject it when you instantiate, so you can switch out the logging mechanism without even touching the DB layer

**Also great for unit testing**

### language paradigms

#### tail recursion

python isn't a functional language, there's functions and you can do many functional style programming, but without a mechanism to optimize tail recursion at compilation time it's difficult to call it functional.

#### typing by prototype

I mean sure JS doesn't have real classes but it's enough to blur the distinction for new programmers
