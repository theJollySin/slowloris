## Slow Loris

> A clone of DIY-LISP. The goal is to learn.

### What Slow Loris will be

It will be a relatively simple, but neat language. Initial features include:

- A handful of datatypes (integers, booleans and symbols)
- Variables
- First class functions with lexical scoping
- A nice, homemade-quality feeling

Initially, it will *not* have:

- A proper type system
- Error handling
- Good performance
- And much, much more

The language should be able to interpret the following code by the time we are done:

```lisp
(define fact 
    ;; Factorial function
    (lambda (n) 
        (if (eq n 0) 
            1 ; Factorial of 0 is 1
            (* n (fact (- n 1))))))

;; When parsing the file, the last statement is returned
(fact 5)
```

The syntax is that of the languages in the Lisp family. [Here is a more detailed description of the language.](parts/language.md)

### Prerequisites

Before we get started, make sure you have installed [Python](http://www.python.org/), [Pip](https://pypi.python.org/pypi/pip), and Nose (pip install nose). 
*For long-term stabilibility, the language is based on Python 2.7, as the Python 3.x flavors are being continuously improved.*

### Getting started!

Initial development is split up into seven parts:

- [Part 1: parsing](parts/1.md)
- [Part 2: evaluating simple expressions](parts/2.md)
- [Part 3: evaluating complex expressions](parts/3.md)
- [Part 4: working with variables](parts/4.md)
- [Part 5: functions](parts/5.md)
- [Part 6: working with lists](parts/6.md)
- [Part 7: using your language](parts/7.md)
