This repository demonstrates a common error in Ada programming: accessing an array element outside its defined bounds. The `bug.ada` file contains code that reproduces this error, while `bugSolution.ada` provides a corrected version.

The error occurs when the loop exits prematurely without completing the iteration through the entire array. This leaves the loop variable pointing to an index beyond the array's valid range. Subseqently attempting to access the array at this index triggers a runtime `Constraint_Error`.

The solution involves ensuring that all array accesses are within the defined bounds. In the corrected version, we add checks to prevent accessing invalid elements.