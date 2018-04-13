# List Comprehension
This directory is here to show the Speed Difference between using 
Dictionary Comprehension vs. a For Loop to create a dictionary

## Executing
In a UNIX terminal, run:


```
time python dict-loop.py

real	0m3.087s
user	0m2.762s
sys	0m0.324s
```

```
time python dict-comp.py

real	0m2.581s
user	0m2.252s
sys	0m0.328s
```


Here we see that the dictionary comprehension is about 20% faster
than the for loop method. Again, this is a case-by-case scenario,
but generally the Dictionary comprehension will probably be faster.
There are probably cases where dictionary comprehension is slower, 
but at the end of the day, comprehensions are generally used for
more concise code rather than for speed.
