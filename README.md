LaTeX Snippets for Sublime Text
===============================

Feel free to add your own snippets and send a pull request.

As LaTeX is, in Sublime's interpretation, rather text than code, one has to trigger auto-completion manually when typing. Alternatively, change the auto-completion mode in order to make the menu show when typing LaTeX.

chapter
-------

`\chapter{$content}`

commenttitle
------------

Inserts a headline in the comments.

```
%%--------------------------------------------------------------------------
%% ${1:TITLE}
%%--------------------------------------------------------------------------
```

emph
----

`\emph{$content}`

footnote
--------

`\footnote{$content}`

fraction
--------

`\frac{$numerator}{$denominator}`

label
-----

`\label{$name}`

nthroot
-------

`\sqrt[$n]{$radicand}`

paragraph
---------

`\paragraph{$content}`

quotes
------

`\glqq{}$content\grqq{}`

section
-------

`\section{$content}`

sqrt
----

`\sqrt{$radicand}`

ssection
--------

`\subsection{$content}`

sssection
---------

`\subsubsection{$content}`

sum
---

`\sum_{$k=$1}^$n`

titlepage
---------

```
\begin{titlepage}
    \author{$author} 
    \title{$title} 
    \date{$date} 
    \maketitle
\end{titlepage}
```
