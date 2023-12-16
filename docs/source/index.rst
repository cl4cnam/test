.. _topics-index:

===================================
FuncSug documentation
===================================

**FuncSug** is a programming language for facilitating GUI programming (in client-side web programming) loosely based on `SugarCubes`_ of Jean-Ferdy Susini. It adheres to `structured concurrency`_ principles.

**Advantages:**

- It avoids "callback hell"
- and enables you to program as if you make a console application
- without losing the multiple possibilities of interaction
- and without freezing the user interface.
- It **eliminates** the need to manage **all the combinations** of component states.

The goal of the language is to enable a better structure of code, that is, a more natural and more readable structure.

For this aim, it uses the "**concurrent way**" or more exactly the "**logically parallel way**". That is, it introduces explicit concurrency where no concurrency seems present or mandatory. The concurrency is reputed to be very difficult. However, amazingly, many cases are simpler with explicit concurrency!

With this style, you can program **as you program for the console** without users losing the multiple possibilities of interaction (Indeed, this style suppresses the *inversion of control* of the callback style of event-driven programming).

This "**concurrent way**" is expressed thanks to additional control flow instructions (beyond ``if``, ``while``, ``for``,...):

- ``parallel`` / ``parallel exitAfter ... finished`` / ``parallel(select ...)`` / ``parallel(for ... in ...)``,
- ``select``,
- ``spawn``,
- ``whileTrue_dependsOn`` / ``whileTrueAwaitFrame_js`` / ``whileTrueAwaitDom_js``,
- ...
- ``repeat``,
- ``sequence``

and with new modifiers (beyond ``break``, ``return``): ``restart``, ``pause``, ``resume``.

.. _structured concurrency: https://en.wikipedia.org/wiki/Structured_concurrency
.. _SugarCubes: https://github.com/LordManta/SugarCubesJS

.. note::

	This project is under active development.
 
