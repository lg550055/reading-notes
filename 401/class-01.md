# Intro to Big O notation and names and values in Python

Given the intensity of the Software Engineering program, it is worth a brief reflexion on pain an suffering before introducing Big O notation.

### Pain and Suffering

A high-quality, immersive program like Python Software Engineering repeatedly pushes students outside their comfort zone.  This is likely to cause pain but ideally not suffering.  The two following quotes summarize this vision:

> Pain plus reflexion equals growth. -*Ray Dalio*

> Suffering is pain without purpose; no higher goal, no dreams, no ambition, no aspiration. -*Code Fellows*

### Big O notation

Big O notation is used in computer science to assess the performance of an algorithm.  It describes how many steps (or space) the algortithm takes as a function of the size of the input.

Rather than a precise assessment of the numbers of steps to the size of the input data, Big O describes the order of magnitude of their relation.  Here are the most common categories:

- O(1) - constant
- O(N) - linear
- O(log N) - logarithmic
- O(N^2) - square
- O(2^N) - exponential

As you can imagine, our aim is to create efficient code.  Big O gives is a widely-used tool to measure it.

### Names and Values in Python

Python is a simple language.  When it comes to names and values is important to know:
> Names refer to values
> Assignments make names refer to a value
> Names are reassigned independently
> Assignment never copies data
> Changes are visible through all names
> Immutable values can't alias
> Anything on the left side of an assignment is a reference
> Lots of things are assignments: x= , for x in , class x() , def x() , def fn(x) , import x , except... as x, with ... as x

---

[Back to table of contents](../README.md)