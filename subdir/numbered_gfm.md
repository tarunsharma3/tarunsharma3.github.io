# Numbered List

1.  Computer Science Enthusiast
2.  Enjoy *trekking*, reading books on latest technology
    1.  Many other hobbies include **cycling**
        1.  Cycling is a fuel efficient way of commuting

# Numbered list with a Special Marker

1)  Asia continent


2)  North America continent


3)  Europe continent


4)  …Rest to be Filled Later…


I can refer to the above point of Europe (3). Only, if using pandoc I
convert this .md file to another .md file with output type -t as gfm.

# Quotes

## Block-quotes

> We want to refer to this text so putting it into block quote

This is a good example

## Inline-quotes

This is an `inline-quote`

# Programming Language Syntax Highlighting

``` python
a = [1, 2, 3]
squaring = [x * x for x in a]
```

``` java
System.out.println("Hello World");
```

``` cpp
int var = 10, sum = 0;
for (int i=0 ; i<var; i++) {
    sum += i;
}
```

# Tables

| Feature or package name | Examples                                 |
| :---------------------- | :--------------------------------------- |
| list comprehension      | `outL = [x*x for x in xrange(0,10,2)]`   |
| dict comprehension      | `outD = {x:x*x for x in xrange(0,10,2)`} |
