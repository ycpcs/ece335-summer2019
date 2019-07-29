---
layout: default
title: "Assignment 7"
---

**Due: Wednesday, Aug 7th in class** Late assignments will be penalized 20% per day.

Book Questions from *How To Prove It - 2nd ed.*
===============================================

6.3.12 (pg. 286), 4.1.8 (pg. 171)

4.3.17 (pg. 188), 5.1.11 (pg. 234)

5.3.2 (pg. 253), 5.3.6 (pg. 253)


*Hints:*

> 6.3.12 - (a) Rather than proving that 2<sup>n</sup> \> *n* by induction, try proving that 2<sup>n</sup> \> *n* + 1 using induction (then clearly since *n* + 1 \> *n* for all *n* this proves the original theorem).

> > (b) Note that for *n* \> 9, (*n*+1) \> 10 \> 2<sup>2</sup>
	
> > (c) Use the fact that 2<sup>n+1</sup> \> *n* + 1 which was proven in part (a).
	
> 4.1.8 - To prove the theorem we must show that each side is a *subset* of the other, i.e. that equality means if and only if. Thus choose an arbitrary element from the *Cartesian product* of one side and show it is an element of the *Cartesian product* of the other side. Note that one direction will simply be the reverse reasoning of the other.

> 4.3.17 - Use the definition of *symmetric* and *composition* to prove the equality (again using if and only if reasoning to show each side is a subset of the other since the composition of relations is itself a relation). Make sure to use the proper sets in the Cartesian products of each part.

> 5.1.11 - (a) Start by letting *x* be an arbitrary element of *A* and *b* = *f(x)*. Then use the fact that *S* is reflexive to deduce a fact about (*x*,*x*). 

> > (b) Start by letting *x*, *y* be arbitrary elements of *A* such that *a* = *f(x)* and *b* = *f(y)*. Use the fact that *S* is symmetric to deduce a fact about (*x*,*y*) and (*y*,*x*). 

> > (c) Start by letting *x*, *y*, *z* be arbitrary elements of *A* such that *a* = *f(x)*, *b* = *f(y)*, and *c* = *f(z)*. Use the fact that *S* is transitive to deduce a fact about (*x*,*y*), (*y*,*z*), and (*x*,*z*).

> 5.3.2 - Note the function for this problem is *A* = {1,2,3}, *B* = ℘(*A*) and *F*: *B* → *B* *F(X)* = *A* \\ *X*. First show that *F* is *one-to-one* and *onto* then determine *F* <sup>-1</sup>. It might help to write out the elements of *B* and construct *F*. See if you can prove that *F* is one-to-one and onto using set properties rather than simply inspecting the ordered pairs. One helpful equivalence is *A* \\ (*A* \\ *B*) = *A* ∩ *B*.

> 5.3.6 - Start by sketching a graph for *f*. Then consider what the *range* of *f* needs to be in order for the function to be *one-to-one*, i.e. so that no two *x* values produce the same *f(x)*. Then consider any further restrictions required to make *f* *onto*, i.e. so that *every* value of *B* has a corresponding *x*. With this restricted domain, determine *f* <sup>-1</sup>.
