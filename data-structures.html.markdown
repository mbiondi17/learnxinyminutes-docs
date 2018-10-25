---
category: Algorithms & Data Structures
name: Data Structures
contributors:
    - ["Matthew Biondi", "http://github.com/MBiondi17"]
---

# Data Structures

## What are they?

Data structures are exactly what they sound like -- objects in which data is
stored in some manner. The file system on your computer is a tree data
structure, where the nodes are directories and leaves are files. Data can be
stored in many ways, such as in arrays, lists, stacks, queues, and trees. 
Each of these methods has advantages and disadvatages. Some may be very fast at
getting a specific element, but be slow when it comes to inserting or deleting
elements. Knowledge of which data structure to use for a given set of data can
be critical in optimizing your program and making difficult tasks easier. 

## Basic Data Structures

In this section, we will give a brief overview of the most fundamental data 
structures, and give basic use cases for each of them. Many other data 
structures are extensions of these basic types, so an understanding of them
will take you far. We will present pseudocode for the implementation of each
of these simple data structures to help illuminate how each of them works.

### Array
### Binary Search Tree
### Hash Table
### Heap
### Queue
### Singly-Linked List
### Stack

## More Complex Data Structures

Here we will review some of the more complicated data structures, and once 
again give examples where each may be used. We will not present pseudocode for
these data structures, but will discuss how they may arise from simpler ones.

### AVL Tree
### B-Tree
### Cartesian Tree
### Doubly-Linked List
### Heap
### KD Tree
### Red-Black Tree
### Skip List
### Splay Tree


## Complexity of Basic Operations

In this section, we will compare the Algorithmic Complexity of the common data
operations (Access, Search, Insert, Delete) for each data structure. A more 
in-depth version of this information (and a cool poster) may be found at
[the Big-O cheatsheet website](http://bigocheatsheet.com/). 

In the below graph, average- and worst- case times are both presented for 
comparison in the form Θ(Avg) | O(worst). For instance, the Binary Search
Tree for each operation looks like Θ(log(n)) | O(n). This means that on 
average, BST operations scale like the log(n), but can scale as slowly as (n)
in some cases. For a more detailed analysis of time complexity, see the page
for Complexity Analysis on this site. 

| Data Structure     |   Access Complexity    | Find Complexity        | Insert Complexity      | Delete Complexity      |
|--------------------|:----------------------:|------------------------|------------------------|------------------------|
| Array              |      Θ(1) \| O(1)      |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |
| AVL Tree           | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) |
| Binary Search Tree |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |
| B-Tree             | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) |
| Cartesian Tree     |       N/A \| N/A       |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |
| Doubly-Linked List |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |      Θ(1) \| O(1)      |      Θ(1) \| O(1)      |
| Hash Table         |       N/A \| N/A       |      Θ(1) \| O(n)      |      Θ(1) \| O(n)      |      Θ(1) \| O(n)      |
| KD Tree            |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |
| Queue              |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |      Θ(1) \| O(1)      |      Θ(1) \| O(1)      |
| Red-Black Tree     | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) |
| Singly-Linked List |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |      Θ(1) \| O(1)      |      Θ(1) \| O(1)      |
| Skip List          |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |    Θ(log(n)) \| O(n)   |
| Splay Tree         |       N/A \| N/A       | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) | Θ(log(n)) \| O(log(n)) |
| Stack              |      Θ(n) \| O(n)      |      Θ(n) \| O(n)      |      Θ(1) \| O(1)      |      Θ(1) \| O(1)      |


## Closing Remarks

This overview does not cover all data structures -- indeed, there are many out
there, and more are still being invented. However, this article has hopefully
given you the understanding you need to pick the right data structure for your
problem. The field of data structures is large, and we heartily encourage you
to look through the extra resources, as there is much more depth to find. 

Happy diving!

## Resources

<!---
## Types of Asymptotic Notation

In the first section of this doc we described how an Asymptotic Notation 
identifies the behavior of an algorithm as the input size changes. Let us 
imagine an algorithm as a function f, n as the input size, and f(n) being 
the running time. So for a given algorithm f, with input size n you get 
some resultant run time f(n). This results in a graph where the Y axis is the 
runtime, X axis is the input size, and plot points are the resultants of the 
amount of time for a given input size.

You can label a function, or algorithm, with an Asymptotic Notation in many 
different ways. Some examples are, you can describe an algorithm by its best 
case, worse case, or equivalent case. The most common is to analyze an 
algorithm by its worst case. You typically don't evaluate by best case because 
those conditions aren't what you're planning for. A very good example of this 
is sorting algorithms; specifically, adding elements to a tree structure. Best 
case for most algorithms could be as low as a single operation. However, in 
most cases, the element you're adding will need to be sorted appropriately 
through the tree, which could mean examining an entire branch. This is the 
worst case, and this is what we plan for.

### Types of functions, limits, and simplification

```
Logarithmic Function - log n
Linear Function - an + b
Quadratic Function - an^2 + bn + c
Polynomial Function - an^z + . . . + an^2 + a*n^1 + a*n^0, where z is some 
constant
Exponential Function - a^n, where a is some constant
```

These are some basic function growth classifications used in various 
notations. The list starts at the slowest growing function (logarithmic, 
fastest execution time) and goes on to the fastest growing (exponential, 
slowest execution time). Notice that as 'n', or the input, increases in each 
of those functions, the result clearly increases much quicker in quadratic, 
polynomial, and exponential, compared to logarithmic and linear.

One extremely important note is that for the notations about to be discussed 
you should do your best to use simplest terms. This means to disregard 
constants, and lower order terms, because as the input size (or n in our f(n) 
example) increases to infinity (mathematical limits), the lower order terms 
and constants are of little to no importance. That being said, if you have 
constants that are 2^9001, or some other ridiculous, unimaginable amount, 
realize that simplifying will skew your notation accuracy.

Since we want simplest form, lets modify our table a bit...

```
Logarithmic - log n
Linear - n
Quadratic - n^2
Polynomial - n^z, where z is some constant
Exponential - a^n, where a is some constant
```

### Big-O
Big-O, commonly written as **O**, is an Asymptotic Notation for the worst 
case, or ceiling of growth for a given function. It provides us with an 
_**asymptotic upper bound**_ for the growth rate of runtime of an algorithm.
Say `f(n)` is your algorithm runtime, and `g(n)` is an arbitrary time 
complexity you are trying to relate to your algorithm. `f(n)` is O(g(n)), if 
for some real constants c (c > 0) and n<sub>0</sub>, `f(n)` <= `c g(n)` for every input size 
n (n > n<sub>0</sub>).

*Example 1*

```
f(n) = 3log n + 100
g(n) = log n
```

Is `f(n)` O(g(n))?
Is `3 log n + 100` O(log n)?
Let's look to the definition of Big-O.

```
3log n + 100 <= c * log n
```

Is there some pair of constants c, n<sub>0</sub> that satisfies this for all n > <sub>0</sub>?

```
3log n + 100 <= 150 * log n, n > 2 (undefined at n = 1)
```

Yes! The definition of Big-O has been met therefore `f(n)` is O(g(n)).

*Example 2*

```
f(n) = 3*n^2
g(n) = n
```

Is `f(n)` O(g(n))?
Is `3 * n^2` O(n)?
Let's look at the definition of Big-O.

```
3 * n^2 <= c * n
```

Is there some pair of constants c, n<sub>0</sub> that satisfies this for all n > <sub>0</sub>?
No, there isn't. `f(n)` is NOT O(g(n)).

### Big-Omega
Big-Omega, commonly written as **Ω**, is an Asymptotic Notation for the best 
case, or a floor growth rate for a given function. It provides us with an 
_**asymptotic lower bound**_ for the growth rate of runtime of an algorithm.

`f(n)` is Ω(g(n)), if for some real constants c (c > 0) and n<sub>0</sub> (n<sub>0</sub> > 0), `f(n)` is >= `c g(n)` 
for every input size n (n > n<sub>0</sub>).

### Note

The asymptotic growth rates provided by big-O and big-omega notation may or 
may not be asymptotically tight. Thus we use small-o and small-omega notation 
to denote bounds that are not asymptotically tight. 

### Small-o
Small-o, commonly written as **o**, is an Asymptotic Notation to denote the 
upper bound (that is not asymptotically tight) on the growth rate of runtime 
of an algorithm.

`f(n)` is o(g(n)), if for all real constants c (c > 0) and n<sub>0</sub> (n<sub>0</sub> > 0), `f(n)` is < `c g(n)` 
for every input size n (n > n<sub>0</sub>).

The definitions of O-notation and o-notation are similar. The main difference 
is that in f(n) = O(g(n)), the bound f(n) <= g(n) holds for _**some**_ 
constant c > 0, but in f(n) = o(g(n)), the bound f(n) < c g(n) holds for 
_**all**_ constants c > 0.

### Small-omega
Small-omega, commonly written as **ω**, is an Asymptotic Notation to denote 
the lower bound (that is not asymptotically tight) on the growth rate of 
runtime of an algorithm.

`f(n)` is ω(g(n)), if for all real constants c (c > 0) and n<sub>0</sub> (n<sub>0</sub> > 0), `f(n)` is > `c g(n)` 
for every input size n (n > n<sub>0</sub>).

The definitions of Ω-notation and ω-notation are similar. The main difference 
is that in f(n) = Ω(g(n)), the bound f(n) >= g(n) holds for _**some**_ 
constant c > 0, but in f(n) = ω(g(n)), the bound f(n) > c g(n) holds for 
_**all**_ constants c > 0.

### Theta
Theta, commonly written as **Θ**, is an Asymptotic Notation to denote the 
_**asymptotically tight bound**_ on the growth rate of runtime of an algorithm. 

`f(n)` is Θ(g(n)), if for some real constants c1, c2 and n<sub>0</sub> (c1 > 0, c2 > 0, n<sub>0</sub> > 0), 
`c1 g(n)` is < `f(n)` is < `c2 g(n)` for every input size n (n > n<sub>0</sub>).

∴ `f(n)` is Θ(g(n)) implies `f(n)` is O(g(n)) as well as `f(n)` is Ω(g(n)).

Feel free to head over to additional resources for examples on this. Big-O 
is the primary notation use for general algorithm time complexity.

### Ending Notes
It's hard to keep this kind of topic short, and you should definitely go 
through the books and online resources listed. They go into much greater depth 
with definitions and examples. More where x='Algorithms & Data Structures' is 
on its way; we'll have a doc up on analyzing actual code examples soon.

## Books

* [Algorithms](http://www.amazon.com/Algorithms-4th-Robert-Sedgewick/dp/032157351X)
* [Algorithm Design](http://www.amazon.com/Algorithm-Design-Foundations-Analysis-Internet/dp/0471383651)

## Online Resources

* [MIT](http://web.mit.edu/16.070/www/lecture/big_o.pdf)
* [KhanAcademy](https://www.khanacademy.org/computing/computer-science/algorithms/asymptotic-notation/a/asymptotic-notation)
* [Big-O Cheatsheet](http://bigocheatsheet.com/) - common structures, operations, and algorithms, ranked by complexity.

--->