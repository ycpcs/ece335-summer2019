---
layout: default
title: "Assignment 5"
---

**Due: Wednesday, July 17th in class** Late assignments will be penalized 20% per day.

Book Questions from *How To Prove It - 2nd ed.*
===============================================

3.2.3 (pg. 106), 3.2.12 (pg. 107)

3.3.2 (pg. 122), 3.3.12 (pg. 122)

3.4.3 (pg. 133), 3.4.7 (pg. 133)


*Hints:*

> 3.2.3 - Consider applying the conditional proof strategy for the original goal and then prove by contradiction.
>
> 3.2.12 - Carefully consider each step of the proof and determine where the error is introduced. Using this error, you should be able to easily create a counterexample.
>
> 3.3.2 - Recall what it means for two sets to be disjoint, i.e. *there does not exist* an element that is in both sets. Rewrite the goal using quantifiers and apply the techniques for handling quantifiers in both the givens (disjoint) and goal (subset).
>
> 3.3.12 - Remember that families contain *sets* but family union contains *elements*. So writing the goal using a universal quantifier (since it is subset), select an arbitrary element *x* ∈ ∪*F*. Then to show that *x* ∈ ∪*G* means that ∃ *A* ∈ *G* (*x* ∈ *A*), i.e. there is a set in the family *G* that contains the element *x*. Then interpret the quantifiers in the givens to find a set *A* ∈ *G* that contains *x*. Since *x* was arbitrary, this will prove the theorem.
>
> 3.4.3 - Write out what it means for *C* \\ *B* ⊆ *C* \\ *A* and then apply the conditional strategy which will give a conjunction given and a conjunction goal. Then prove both goals separately.
>
> 3.4.7 - DO NOT show this equivalency using logical equivalencies. Instead prove it by
> interpreting the = as ↔. Thus prove
> 
> > ℘(*A* ∩ *B*) ↔ ℘(*A*) ∩ ℘(*B*)
>
> Break the biconditional up into separate parts (recall *P* ↔ *Q* = (*P* → *Q*) ∧ (*Q* → *P*) and show 
>
> > ℘(*A* ∩ *B*) → ℘(*A*) ∩ ℘(*B*)
> 
> and separately
> 
> > ℘(*A*) ∩ ℘(*B*) → ℘(*A* ∩ *B*)
> 
> Since powersets imply subsets, use universal instantiation to construct the proof.
