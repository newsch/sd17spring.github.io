---
date: '2016-12-29T18:26:01'
description: ''
title: Pickling
toc: true
---

In this project toolbox exercise you will be learning how to write Python data
to disk and retrieve them later. This structure will be very useful for any
situation where your program needs to have access to persistent data that it
then modifies periodically. One way this can be used is to make a quick and
dirty database.

## Get Set

The starter code contains the function you should be implementing. The
function has a descriptive docstring that explains what you will be doing
along with a few unit tests. If you run the Python script without any
arguments you will execute the doctests.

Grab the starter code for this toolbox exercise via the normal fork-and-clone
method from <https://github.com//{{site.course.github_owner}}/ToolBox-Pickling>.The starter code
will be in `counter.py`.

## Learn About File Input and Output

There are many good resources to use to learn about files. Check out some of
these resources:

* [The Python documentation](https://docs.python.org/2/tutorial/inputoutput.html)
* [Think Python Chapter 14](http://www.greenteapress.com/thinkpython/html/thinkpython015.html)
* [This tutorial](http://www.tutorialspoint.com/python/python_files_ io.htm) at TutorialsPoint

## Learn About Pickle

There are many good resources to use to learn about pickling. Check out some
of these resources:

* [The Python documentation](https://docs.python.org/2/library/pickle.html)
* [Think Python Chapter 14](http://www.greenteapress.com/thinkpython/html/thinkpython015.html)
* [The Python wiki](https://wiki.python.org/moin/UsingPickle)

## Implement the function update_counter

The basic idea is to open the counter file in **r+**  (reading plus) mode if it
exists and you are not resetting the counter, and in **w**  (writing) mode
otherwise. Once the file is open you can either initialize the counter to 0
(if appropriate) or read the counter value (using `load`) and then increment
it. To finish your implementation, use the `dump` function to store the
resultant counter value to the disk.

Hints:

  * To see if the file already exists, you can use `os.path.exists` function which we have already imported for you as `exists`
  * To move the file handle back to the beginning of the file (for instance after reading), use the command `f.seek(0,0)` (assuming you called your open file **f** )

## Turning in your toolbox assignment

To turn in your assignment, push your code to GitHub and submit a pull request
to notify the NINJAs to check you off!