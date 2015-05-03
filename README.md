sudoku-solver
=============
The great Sudoku solver challenge for Python Atlanta!

Use your skills to produce a sudoku solver.  Rules:

1. Pure python solution

2. Totally local solution (no call-outs to a CUDA powered AWS instance, for example).

3. Your solution should be self contained in a single file.  The python standard library fair to use.

4. Must be callable via 'python <your script> <81char sudoku puzzle>' (full example below)

5. Puzzle spec must be 81 characters string.  Accept 0 as unknown slots in the sudoku puzzle.

6. Output must be the solved puzzle presented as an 81 character string.  The 81 characters begin in the top left of the puzzle.  The first 9 characters are the top row of the puzzle, left to right.  The next 9 are the second row, etc.  Full example:
```
$ python ./sudoku1.py 048006102000300000009005006000001089000000000000900001006002900084100000002048003
348796152615324897279815436527461389891253674463987521136572948784139265952648713
```

7. Please name the file uniquely (sudoku1.py is a poor choice).

8. Contest will either run on my multi-core macbook, or a multi-core linux VM.  Default python is 2.7.8.  Python3 is available on request.  Submit your solution as a pull request into this github repo: https://github.com/zapman449/sudoku-solver.git   .  Please place your code either in the p2 directory (for python 2) or the p3 directory (for python 3).

9. The winner will need to discuss their solution and how it works in detail.  Other people should be willing to give a 'lightening talk' on their solution.

Other details:

The script 'sudoku-harness.sh' and 'compare.py' will compare the results of the tests.  An assortment of puzzles will
be attempted with your solution.  Absolute timeout is 60 seconds.  If you take that long, you've blown it.  Time will
measured via gnu time's 'elapsed' time.  Each puzzle will be attempted 3 times, and the best of those three times will
be used for scoring.  Note: the puzzles in puzzles.txt are NOT the puzzles you'll be judged on, but they are representative.
