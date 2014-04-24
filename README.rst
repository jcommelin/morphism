morphism
========

This package is heavily inspired by and builds upon Pieter Belmans ideas: http://pbelmans.wordpress.com/2010/12/24/an-extension-to-our-function-macro-injective-and-surjective-functions/.

Typesetting morphisms in LaTeX
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

This LaTeX package provides a command ``\map`` which should be used as
follows::

    \map[f]{X}[hook]{Y}[x][y]

The arguments between ``[]`` are optional, the arguments between ``{}`` are
mandatory.

* The first argument (``[f]``) is the name of the map/morphism.
* The second argument (``{X}``) is the source of the morphism.
* The third argument (``[hook]``) provides an arrow modifier (in this case a
  hook, to indicate an injective map).
* The fourth argument (``{Y}``) is the target of the morphism.
* The fifth and sixth argument (``[x][y]``) are respectively an element of the
  source, and its image in the target.

The way this command typesets the morphism depends on whether it is used in
inline math or display math. This is also one of its great advantages, because
it allows for easy moving of morphism definitions from inline to display math,
and vice versa.

In inline math, it (rougly) typesets as :math:`f : X \hookrightarrow Y, x
\mapsto y`. (In LaTeX: ``f \colon X \hookrightarrow Y, x \mapsto y``.) In
display math it looks approximately like

.. math::
	\begin{array}{crll}
                f : & X & \hookrightarrow & Y \\
                & x & \mapsto & y
	\end{array}

which, in LaTeX code looks like::

	\arraycolsep=1.4pt
	\begin{array}{crll}
		f \colon & X & \longhookrightarrow & Y \\
                & x & \longmapsto & y
	\end{array}

Arrow modifiers
---------------

To be written.


