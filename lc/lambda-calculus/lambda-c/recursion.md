# Recursion in lambda calculus

To achieve recursion in lambda calculus, a fixed-point function is required.
**Fixed-point function** or **Y-combinator** must satisfy *Yf=f(Yf)*

The function used is   
Y: `λf.(λg.f(gg))(λg.f(gg))`

`Yf` can be beta reduced to 
`(λg.f(gg))(λg.f(gg))`  which in turn can be beta reduced to 
`f(λg.f(gg))(λg.f(gg))` satisfying *Yf=f(Yf)*

Using Y, a function has access to a bound copy of itself.

If lambda expressions were named, you might want to write 
`f=λx1...xnE`, where E is some expresion refering to f.

With the Y combinator, the function on the right becomes `Yλfx1...xnE`.


## Partial recursive functions in lambda calculus

Partial recursive functions are a functional model of universal computation developed by Kleene, Gödel and Herbrand.

Partial recursive functions are built from a set of basic functions: **projection**, **zero** and **successor**, which apply to tuples of integers, using the operations of *composition*, *primitive recursion* and *minimisation*.


















