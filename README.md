# Magma code to find generating vectors for groups acting on Riemann surfaces
This repository hosts Magma code used to determine generating vectors given a group and signature.

The original GAP code this code is based on has the following copyright:

*Copyright (C)  1997,  Lehrstuhl D fuer Mathematik,  RWTH Aachen,  Germany*


We are grateful to Thomas Breuer for permission to post the Magma version of this code.


To determine generating vectors, first type in Magma<br>
`load "genvectors.mag"`

The command `RepresentativesEpimorphisms(signature,G)` will output record(s) in Magma corresponding to one representative of each action for that group and signature up to *simultaneous conjugation*. Each record will consist of 4 fields:
* `signature` - the signature <br>
* `Con` - the conjugacy classes where this particular generating vector comes from, numbered as in Magma<br>
* `Gro`  - the group<br>
* `genimages` - the generating vectors as elements of G<br>


WARNING: If the group G is not already a permutation group, the program will convert it to one.  The records outputted, then, will give generating vectors as permutations for that permutation group.


More information about this project, and data run up to genus 48 may be found here:
http://www.math.grinnell.edu/~paulhusj/monodromy.html

