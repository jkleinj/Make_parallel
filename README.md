# Demo for parallel GU Make execution
Example taken from
* https://stackoverflow.com/questions/7668311/makefile-run-processes-in-background

Run the Makefile.parallel with:
```
make -j -f Makefile.parallel
```

From the GNU Make manual:
* https://www.gnu.org/software/make/manual/html_node/Parallel.html

If the ‘-j’ option is followed by an integer, this is the number
of recipes to execute at once; this is called the number of job slots.
If there is nothing looking like an integer after the ‘-j’ option,
there is no limit on the number of job slots.
The default number of job slots is one, which means serial execution
(one thing at a time).

You can use the ‘-l’ option to tell make to limit the number of jobs
to run at once, based on the load average. The ‘-l’ or ‘--max-load’
option is followed by a floating-point number. 


