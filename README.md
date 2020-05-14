# contextual
What if you could invent a new programming language, designed purely to simplify your life as a programmer, without *any* of the constraints of existing languages? 

This is a proposal for a new programming language, or meta-language, designed for radical brevity plus human-readability. Think CoffeScript or Clojure without all the cruft. 

This project is bold enough to propose coding practice which some people might find scary. The radical goals of this project will not be comfortable for everyone, and we're OK with that. We're not trying to please everyone. We're trying to please programmers who are tired of having to over-explain themselves to the computer. 


# example
Which one do YOU find easier to read? Be honest. 

**Javascript**

105 chars

(each indent counts as one char)
```
greetByName('Jack')

function greetByName(sName) {
    if (!sName) {
        console.log ('Hi');
        }
    else {
        console.log ('Hello, ' + sName);
        };
    };
```

**contextual, proposed:** 

36 chars
````
greetByName'Jack'

greetByName
    ! Say
        'Hello ' sName
        'Hi'    
````
The contextual version has strong typing and locally-scoped variables. 

[Full explanation](https://github.com/contextual-contribs/contextual/wiki/Snip:-Function-With-Conditional)


# philosophy
The core philosophies of this meta-language are:
- Eliminate "machinery" in code. That is, most (all?) code today is packed with instructions to the parser[1], which aren't necessarily useful to the programmer, and often reduce readability. For example, punctuation. 
- Make the parser smarter. Exploit parser-intelligence to radically reduce programmer effort. 
- Exploit whitespace. Imply structure with whitespace. 
- Eliminate the obvious. Depend on context and implication. 
- Eliminate redundancy. 
- Eliminate variables whenever possible. 
- Make the most common coding patterns part of the language, so the programmer doesn't have to spell them out every time. 
- Enable programmer to customize language-keywords. 
- Strongly-typed.

[1]: (Using the word "parser" to refer to IDE, linters, parsers, transpilers, and compilers. Anything that interprets the code.)


# goals
1. Define the language. Resolve all ambiguities. 
2. Build a Javascript transpiler. 


# progress
Current phase is **brainstorming phase.** The only activity right now is for the community to dream up better, briefer ways to write code. No work will be done on a parser, transpiler, or compiler at this time. 
