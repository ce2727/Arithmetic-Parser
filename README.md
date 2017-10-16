# Arithmetic-Parser
Creates a parse tree using a recursive decent parse algorithm, then evaluates it. As well, it runs a table based parse on the expression to see if it applies to the grammar.

Grammars derived from https://www.cs.rochester.edu/~nelson/courses/csc_173/grammars/parsing.html

-----

Recursive Decent Grammar:

    <E>→<T><A>

    <A>→+<T><A>|-<T><A>|e

    <T>→<F><B>

    <B>→*<F><B>|/<F><B>|e

    <F>→<E>|<N>

    <N>→<D><C>

    <C>→<N>|e

    <D>→0|1|2|3|4|5|6|7|8|9

-----

Table Based Grammar:

    <E>→<T><A>

    <A>→+<T><A>|-<T><A>|e

    <T>→<F><B>

    <B>→*<F><B>|/<F><B>|e

    <F>→<E>|<Number>
