LaTeX Snippets for Sublime Text
===============================

Feel free to add your own snippets and send a pull request.

As LaTeX is, in Sublime's interpretation, rather text than code, one has to trigger auto-completion manually when typing. Alternatively, change the auto-completion mode in order to make the menu show when typing.

* _Note about using `turn_on_number.sublime-snippet` and `turn_off_number.sublime-snippet`_

Suppose you have written an unnumbered equation
```
\[
  Y = X.
\]
 ```
Latter, you want to change this unnumbered equation to be a numbered one.
```
\begin{equation}
  Y = X.
\end{equation}
 ```
Or you want to do the reverse (change numbered one to be unnumbered).

`turn_on_number.sublime-snippet` and `turn_off_number.sublime-snippet` are prepared to do the above conversion. `turn_on_number.sublime-snippet` is to convert the _selected_ unnumbered equation to be a numbered one. `turn_off_number.sublime-snippet` is to do reverse.

To use them, first save these two snippets, and second define key bindings to implement them. For example, let `Packages/User/My Snippets/LaTeX/turn_on_number.sublime-snippet` be path of the first snippet. One can define `cmd + shift + 1` and `cmd + shift + 0` (in Mac) as the short cut for "turning the equation number on" and "off", respectively, by adding the following to your sublime text key bindings.

```
{
    "keys": ["super+shift+1"],
    "command": "insert_snippet", 
    "args": { "name": "Packages/User/My Snippets/LaTeX/turn_on_number.sublime-snippet"}
},
{
    "keys": ["super+shift+0"],
    "command": "insert_snippet", 
    "args": { "name": "Packages/User/My Snippets/LaTeX/turn_off_number.sublime-snippet"}
},
```

![equ_number](switching_equation_number.gif)
