# dhvar

## Background

This is a non-empty program that takes no input, and produces an exact copy of its source code on the standard output.

## Approach

One approach is to create some data: a string or array of strings. This data contains all or most of the characters or lines that appear in the source code . Output the strings or substrings with some of them more than once. As the code developed, the data need to be updated since it has to match.

Want to avoid the use of quoted strings or character literals, except in that one place where you specify the data.

One of the tricky parts is to figure out how to deal with special characters like quotation marks, newlines, and other punctuation. For example, in Python, one way to get a double-quote mark is to use something like `'"'`.

Perhaps, create a program whose output differs from the source only by non relevant spacing. If the ouptut compile and produce itself, use that intead.

Use `diff` to do the comparison. If the following produces no output, then the program and its output are identical.
```
python3 dhvar.py | diff - dhvar.py
```

The program should be minimal, i.e. no comments and unnecessary spaces. Style is out of the window. Lines can be as long as desired. If the program is essentially unreadable, you may have done it right. The program can be written in just two or three lines. However, you may write more. Though a smaller program would be more readable than most.

## How to run

```
python3 dhvar.py | diff - dhvar.py
```

## Author

Truong Pham


