# List Comprehension
This directory is here to show the Speed Difference between using 
List Comprehension vs. calling append() in a For Loop to create a list

## Executing
In a UNIX terminal, run:

```
time python list-append-loop.py
```
real	0m11.381s
user	0m10.553s
sys		0m0.824s

```
time python list-comp.py
```
real	0m4.228s
user	0m3.428s
sys		0m0.800s


Here we see that the list comprehension was almost 3x as fast
as the `list.append()` for loop. This is because everytime the
append() method is called, it has to be looked up by the Interpreter,
whereas the list comprehension can do it all at once.

### Disclaimer
Since this is a very simple example where we are just creating a list of
numbers with the range() function, we can actually just cast the result
of the range() function to a list and get even faster speed than the
list comprehension. 

To show a more practical example where you can't just cast it:

```
time python list-append-loop2.py
```

real	0m29.756s
user	0m28.875s
sys		0m0.880s


```
time python list-comp2.py
```

real	0m21.932s
user	0m21.031s
sys		0m0.900s

In this practical example, we see that the list comprehension finished
in about 2/3 of the time it took the for loop append() method, still
significantly faster!

All in all, it depends on the example, but list comprehensions are often
faster than using a loop.
