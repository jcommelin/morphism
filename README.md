morphism
========

Typesetting morphisms in LaTeX
------------------------------

This LaTeX package provides a command `\map` which should be used as follows:

    \map[f]{X}[hook]{Y}[x][y]

The arguments between `[]` are optional, the arguments between `{}` are
mandatory.

* The first argument (`[f]`) is the name of the map/morphism.
* The second argument (`{X}`) is the source of the morphism.
* The third argument (`[hook]`) provides an arrow modifier (in this case a
  hook, to indicate an injective map).
* The fourth argument (`{Y}`) is the target of the morphism.
* The fifth and sixth argument (`[x][y]`) are respectively an element of the
  source, and its image in the target.

The way this command typesets the morphism depends on whether it is used in
inline math or display math. This is also one of its great advantages, because
it allows for easy moving of morphism definitions from inline to display math,
and vice versa.

In inline math, it typesets roughly as f: X-> Y, x |-> y. In display math it
looks like
	f : X --> Y
	    x |-> y

Arrow modifiers
---------------

To be written.


