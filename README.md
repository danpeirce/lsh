# LSH

## Changes

1. Added the new built-in 'quit'. It is only an alias for 'exit' and uses the same 
   function lsh_exit() that was already implemented.
2. Replaced lsh_read_line() with simpler version that uses the stdio function
   getline(). This possibility was already described in the tutorial 
   at <http://stephen-brennan.com/2015/01/16/write-a-shell-in-c/>. I am
   happy to use the standard function here.

## Original Description

LSH is a simple implementation of a shell in C.  It demonstrates the basics of
how a shell works.  That is: read, parse, fork, exec, and wait.  So I think it's
pretty cool.  Since it's a simple implementation, it has some limitations.

* Commands must be on a single line.
* Arguments must be separated by whitespace.
* No quoting arguments or escaping whitespace.
* No piping or redirection.
* Only builtins are: `cd`, `help`, `exit` and now `quit`.
