This is a prototypical implementation exemplifying the concept of local 
higher-order fixpoint iteration. It is written in OCaml. 

Make sure that the executable `ocamlc' is available, and possibly set the
path to it in Makefile. Then execute

> make all

to create executable.. These show the evaluation of a (possibly nested)
higher-order fixpoint formula over particular structures. The examples
are described in the paper "Local Higher-Order Fixpoint Iteration" by
F. Bruse, M. Lange, M. Sälzer of the University of Kassel, Germany, and
J. Kreiker of the University of Applied Sciences Fulda, Germany. 

- Example 1 formalises a non-context-free reachability problem. Usage:

    example1 <n>

   with n a natural number. Default is n=2.

- Example 2 formalises a context-sensitive parsing problem as it occurs
   in programming languages with indentation. Usage:

    example2 <s>

   where <s> is a string interepreted as a sequence of tokens for a grammar
   that recognizes words over the alphabet {'b','c','s'} (for 'block', 'code',
   'space'). Default is 
