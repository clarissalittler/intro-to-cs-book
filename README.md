<div id="table-of-contents">
<h2>Table of Contents</h2>
<div id="text-table-of-contents">
<ul>
<li><a href="#orgheadline1">1. The Point of This Book</a></li>
<li><a href="#orgheadline2">2. What Should Be Included</a></li>
<li><a href="#orgheadline3">3. A Revised Approach</a></li>
</ul>
</div>
</div>

# The Point of This Book<a id="orgheadline1"></a>

What I really want is for there to be a book that teaches introductory programming with an eye towards actually giving a decent introduction to the more formal concepts in computer science, at least the ones relevant to understanding how programming-in-and-of-itself works.

Basically, I'm trying to write the book I wanted years ago when I thought, as someone who cut my teeth in the math department, that I just was wired wrong for learning how to code.

The problem I had those years ago was that I wanted to find *meaning* in the syntax of languages themselves. Fortran 77 and C++ were probably not good first languages to see if one wanted principled algebraic meaning, I suppose. 

The reality, though, is that syntax is syntax and semantics is semantics. I don't mean to say that syntax can't and shouldn't convey meaning, but that sometimes syntax is convention or aesthetic or this-would-have-made-the-parser-twice-as-long. If I had had a book that explained the distinction between syntax and semantics and, in particular, the meaning of a program can be understood apart from the mysterious implementation running it, I think I would have started enjoying myself a lot more quickly.

That's the kind of thing I want to write. I want to write a book that ultimately leaves the reader, even without any real programming or mathematics background to speak of, with an understanding of the distinction between the parts of a language and their meaning, the distinction between describing a computation and performing one. I want anyone who makes it through the text to have the ability to quickly understand how to learn other languages by knowing how to break a new language down into familiar computational idioms.

# What Should Be Included<a id="orgheadline2"></a>

-   a description of how to evaluate each piece of syntax by hand
    -   exercises to demonstrate doing just that
    -   a plethora of examples
        -   (this is one place where I currently fall down in my existant rough text)
-   give a language independent idea of What Programming Is
    -   iteration
    -   recursion
    -   data types
    -   branching
    -   these are all topics that should be related to how we describe directions in general
        -   what do I mean by this? I mean that we should appeal to how we specify instructions in the first place.
        -   we know how to follow orders of "if this then that"
            -   branching
        -   we know how to follow directions that say repeat something n-times
            -   iteration
        -   we know how to break a problem into sub-problems
            -   recursion
        -   we know how to learn to associate words or phrases with procedures
            -   function definitions
-   explanation and exercises for learning to **read** code
    -   this is something I've never seen in an intro-to-computer science text
        -   but a skill that's very important
    -   this would include small programs and a series of questions to answer about
        -   what the code does
        -   how it works
        -   its (rough) efficiency on its input
        -   any critiques for the style and possible errors
    -   exercises on how to read code should start with small functions and progress into entire programs
-   intro topics in cs
    -   adts
        -   lists
        -   trees
        -   graphs
        -   heaps
        -   &#x2026;
    -   sorting
    -   searching
    -   all of these are topics that are like learning your arithmetic skills
        -   they're not the be-all-end-all
        -   but they're good to know and good practice
-   strategies for writing correct code
    -   tests
    -   types
    -   writing specifications
    -   simple correctness proofs
        -   does this belong in an introductory book? I'd argue it does. If you're going to teach calculational reasoning I think you should also have a way of describing how to use calculations to gain confidence in your code

# A Revised Approach<a id="orgheadline3"></a>

I was thinking about why I keep getting stuck with this text and I realized that one of the problems is that of *narrative* and organizing the text. One of my frustrations with texts and tutorials on programming is that they either

-   introduce programming constructs with a monkey-see-monkey-do approach
-   introduce programming with a syntax-first approach

I'm somewhat guilty of the latter in early attacks on this book, but I think they're both very wrong approaches.
I think what I've been missing is a need to focus on *informal description*, on how to conceptualize how to solve problems in programming with words rather than just saying "for loops do this" or "if statments do that". Instead, we can start each section of the text with a problem to be solved and a description of how to solve the problem informally, building up each of the pieces we need to solve the problem in the formal syntax and explaining a connection between how we describe the problem in natural language and how the formal syntax works.
