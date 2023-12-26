# llpnatded.sty

LLP-style natural deduction with LaTeX3

* Made for typesetting homework of the course _Logic, Language and Philosophy_ at Tsinghua University.
* Matching the natural deduction style used in the textbook manuscript.

## Example

```latex
\begin{nd}{3}
    \ndopen
    \ndstep{1}{p \to q}{\mathtt{A}}
    \ndopen
    \ndstep{2}{\neg q}{\mathtt{A}}
    \ndopen
    \ndstep{3}{p}{\mathtt{A}}
    \ndstep{4}{q}{E_\to, 1, 3}
    \ndstep{5}{\bot}{E_\neg, 2, 4}
    \ndclose
    \ndstep{6}{\neg p}{I_\neg}
    \ndclose
    \ndstep{7}{\neg q \to \neg p}{I_\to}
    \ndclose
    \ndstep{8}{(p \to q) \to (\neg q \to \neg p)}{I_\to}
\end{nd}
```

![image](https://github.com/skylee03/llpnatded/assets/24489025/f4c884c1-63c7-460d-8164-8c8a89303be9)


## License

This work may be distributed and/or modified under the conditions of the LaTeX Project Public License, either version 1.3 of this license or (at your option) any later version. The latest version of this license is in

https://www.latex-project.org/lppl.txt

and version 1.3c or later is part of all distributions of LaTeX version 2008 or later.
