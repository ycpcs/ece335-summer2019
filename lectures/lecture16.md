---
restindex: |
    crumb: Lecture 16 format: rest page-title: Lecture 16: Proof by
    Induction encoding: utf-8 output-encoding: None initialheaderlevel: 2
    build: yes include: yes
---

/restindex

1. Induction Goals
==================

::: {.parsed-literal}
To prove a goal of the form ∀*n* ∈ ℕ *P(n)* where ℕ is the set of
natural numbers, i.e. ℕ = {0,1,2,3,\...}, first prove *P(0)*, known as
the *base case*, and then prove ∀*n* ∈ ℕ (*P(n)* → *P(n+1)*), known as
the *induction step*. Thus we show that the statement is true for some
*initial value* (typically 0) and then prove that if *P(n)* is true then
*P(n+1)* is true. Thus since *P(0)* gives *P(1)* which gives *P(2)* and
so on proving *P(n)* for all *n*.

The form of the formal proof will have the form:

*Base Case.* \[Proof of *P(0)* goes here.\] *Induction Step.* \[Proof of
∀*n* ∈ ℕ (*P(n)* → *P(n+1)*) goes here.\]
:::

**Example 1**

::: {.parsed-literal}
Prove that for every natural number *n*, 2^0^ + 2^1^ + \... + 2^n^ =
2^n+1^ - 1.
:::

First we can easily show the base case for *n* = 0 since

> 2^0^ = 1 and 2^1^ - 1 = 2 - 1 = 1.

Next we need to show the induction step which is that if 2^0^ + 2^1^ +
\... + 2^n^ = 2^n+1^ - 1, then 2^0^ + 2^1^ + \... + 2^n^ + 2^n+1^ =
2^n+2^ - 1.

Therefore we assume 2^0^ + 2^1^ + \... + 2^n^ = 2^n+1^ - 1 is true and
then try to show the conclusion.

Thus we compute 2^0^ + 2^1^ + \... + 2^n^ + 2^n+1^ which by our
assumption gives

> (2^0^ + 2^1^ + \... + 2^n^) + 2^n+1^ = (2^n+1^ - 1) + 2^n+1^
>
> = 2 ⋅ 2^n+1^ - 1
>
> = 2^n+2^ - 1

Thus we have proved the induction step.

Formally,

> **Theorem.** *Prove that for every natural number n*, 2^0^ + 2^1^ +
> \... + 2^n^ = 2^n+1^ - 1.
>
> *Proof.* Using induction:
>
> *Base Case:* Letting *n* = 0, we get 2^0^ = 1 = 2^1^ - 1.
>
> *Induction Step:* Let *n* be an arbitrary natural number and assume
> that 2^0^ + 2^1^ + \... + 2^n^ = 2^n+1^ - 1. Then
>
> > (2^0^ + 2^1^ + \... + 2^n^) + 2^n+1^ = (2^n+1^ - 1) + 2^n+1^
> >
> > > = 2 ⋅ 2^n+1^ - 1
> > >
> > > = 2^n+2^ - 1

**Example 2**

::: {.parsed-literal}
Prove that for all *n* ∈ ℕ, 0 + 1 + 2 + \... + *n* = *n*(*n* + 1)/2.
:::

First we show the base case for *n* = 0 which gives 0(1)/2 = 0.

Next we work on the induction step by assuming 0 + 1 + 2 + \... + *n* =
*n*(*n* + 1)/2 and trying to show 0 + 1 + 2 + \... + *n* + *n* + 1 =
(*n* + 1)((*n* + 1) + 1)/2 = (*n* + 1)((*n* + 2)/2. Thus

> 0 + 1 + 2 + \... + *n* + *n* + 1 = (0 + 1 + 2 + \... + *n*) + *n* + 1
>
> > = *n*(*n* + 1)/2 + *n* + 1
> >
> > = (*n* + 1)(*n*/2 + 1)
> >
> > = (*n* + 1)(*n* + 2)/2

Formally,

> **Theorem.** *Prove that for all n* ∈ ℕ, 0 + 1 + 2 + \... + *n* =
> *n*(*n* + 1)/2.
>
> *Proof.* Using induction:
>
> *Base Case:* Letting *n* = 0, we get 0(1)/2 = 0.
>
> *Induction Step:* Let *n* be an arbitrary natural number and assume
> that 0 + 1 + 2 + \... + *n* = *n*(*n* + 1)/2. Then
>
> > 0 + 1 + 2 + \... + *n* + *n* + 1 = (0 + 1 + 2 + \... + *n*) + *n* +
> > 1
> >
> > = *n*(*n* + 1)/2 + *n* + 1
> >
> > = (*n* + 1)(*n*/2 + 1)
> >
> > = (*n* + 1)(*n* + 2)/2

**Example 3**

::: {.parsed-literal}
Prove that for sufficiently large *n*, that 2^n^ \> *n*^2^.
:::

First we show a base case, but we *cannot* use *n* = 0 since for *n* =
3, 3^2^ = 9 but 2^3^ = 8. Likewise for *n* = 4, 4^2^ = 16 but 2^4^ = 16.
However for *n* = 5, 5^2^ = 25 and 2^5^ = 32 which we can use as a base
case. Thus while the theorem is *not* true *for all* *n* ∈ ℕ, it may be
true for *n* ≥ 5.

Now to show the induction step we need to prove that if 2^n^ \> *n*^2^
then 2^n+1^ \> (*n*+1)^2^. Thus assume 2^n^ \> *n*^2^, then

> 2^n+1^ = 2 ⋅ 2^n^

Applying the assumption for 2^n^ gives

> 2 ⋅ 2^n^ \> 2 ⋅ *n*^2^

At this point we now need to show 2 ⋅ *n*^2^ \> (*n*+1)^2^ = *n*^2^ +
2*n* + 1. Thus bringing *n*^2^ from the right hand side of the
inequality to the left reduces the proof to showing for *n* ≥ 5 that

> *n*^2^ \> 2*n* + 1

Now we observe that for *n* ≥ 5 it is clear that *n*^2^ = (*n*)(*n*) ≥
5*n* and thus

> *n*^2^ ≥ 5*n*
>
> > = 2*n* + 3*n*
> >
> > \> 2*n* + 1

Hence the theorem is true for \"sufficiently large\" *n* which in this
case is *n* ≥ 5.

Formally,

> **Theorem.** *Prove that for sufficiently large n, that 2*^n^ \>
> *n*^2^.
>
> *Proof.* Using induction:
>
> *Base Case:* Letting *n* = 5, clearly *n*^2^ = 5^2^ = 25 and 2^n^ =
> 2^5^ = 32. Thus 2^n^ \> *n*^2^ for *n* = 5.
>
> *Induction Step:* Let *n* be an arbitrary natural number greater than
> 5 and assume that 2^n^ \> *n*^2^. Since *n* \> 5, clearly *n*^2^ =
> (*n*)(*n*) \> 5*n*. Thus
>
> > 2^n+1^ = 2 ⋅ 2^n^
> >
> > > \> 2 ⋅ (*n*^2^)
> > >
> > > = *n*^2^ + *n*^2^
> > >
> > > ≥ *n*^2^ + 5*n*
> > >
> > > = *n*^2^ + 2*n* + 3*n*
> > >
> > > \> *n*^2^ + 2*n* + 1
> > >
> > > = (*n* + 1)^2^
>
> Therefore 2^n+1^ \> (*n* + 1)^2^ and hence 2^n^ \> *n*^2^ for *n* ≥ 5.
