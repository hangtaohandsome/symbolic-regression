CHARLIE - A symbolic regression system using genetic programming
================================================================

A very simple implementation of genetic programming in Racket.

The user can define elementary functions. Generated functions are
evaluated in a sandbox memory- and time-limited.

Default parameters are set in file genetic-programming.rkt and can be
changed by using Racket parameter system.
 * function-set - set of functions to be used in gp (a assoc list mapping symbols to actual functions)
 * mutation-percent - what percent of chromosomes should be mutated
 * stop-percent - stop probab. at creating function
 * subexp-percen - stop probab. at fetching subexpression
 * crossover-percent - stop probab. at crossover
 * initial-complexity - max initial depth of exp
 * allowed-complexity - max overall depth of exp (Koza. 17)
 * symbol/constant - ratio between symbols and constants
 * variables - list of free variables

For further reference check the source code.

This is an old (2010) project migrated from Google Code.

Revision history:
-----------------
 * 0.0.0 Sun Aug 15 2010 - initial implementation
 * 0.1.0 Tue Aug 24 2010 - removed globals, added parameters instead
 * 0.1.1 Sun Sep  5 2010 - added simplify (expression simplifier.
 * 0.1.2 Wed Sep  8 2010 - moved simplify to a separate module, added sandboxed evaluation
 * 0.2.0 Mon Dec 13 2010 - added Gauss-Newton algorithm for fixing the coefficients


