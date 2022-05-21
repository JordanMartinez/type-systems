# LaTeX

Throughout this work, LaTeX will be used, especialy since GitHub markdown now renders it automatically. Below is a LaTeX cheatsheet. Symbols are mapped to their definition in LaTeX and their meaning in English. I use this also to verify that GitHub renders content correctly.

Sources used:
- [Using LaTeX in Markdown](https://ashki23.github.io/markdown-latex.html#latex)
- [List of LaTeX Symbols](https://latex.wikia.org/wiki/List_of_LaTeX_symbols)

## Markdown Test

$Inline LaTeX Expression$

$$
Multi
Line
LaTeX
Expresion
$$

## Symbols

### Math operators

| Symbol | LaTeX | English |
| - | - | - |
| $$+$$ | `+` | Plus |
| $-$ | `-` | Minus |
| $\times$ | `\times` | Times |
| $\div$ | `\div` | Divide |

### Equality

| Symbol | LaTeX | English |
| - | - | - |
| $=$ | `=` | Equals |
| $\ne$ | `\ne` | Not Equals |
| $<$ | `<` | Less than |
| $\le$ | `\le` | Less than or equal to |
| $>$ | `>` | Greater than |
| $\ge$ | `\ge` | Greater than or equal to |


### Common Mathematical Symbols/Constants

| Symbol | LaTeX | English |
| - | - | - |
| $\infty$ | `\infty` | Infinity
| $\sum$ | `\sum` | Sum
| $\prod$ | `\prod` | Product

### Boundary Characters

| Symbol | LaTeX | English |
| - | - | - |
| $\{$ | `\}` | Left brace
| $\}$ | `\}` | Right brace
| $($ | `(` | Left parenthesis
| $)$ | `)` | Right parenthesis
| $[$ | `[` | Left bracket
| $]$ | `]` | Right bracket

### Sets/Collections

| Symbol | LaTeX | English |
| - | - | - |
| $\varnothing$ | `\varnothing` | Empty set
| $\{1, 2\}$ | `\{1, 2\}` | A set of two elements: 1 and 2
| $\mathbb{N}$ | `\mathbb{N}` | Natural numbers: $i \in \{ 1, 2, ..., \infty\}$
| $\mathbb{Z}$ | `\mathbb{Z}` | Integers: $i \in \{ -\infty, ..., -1, 0, 1, ..., \infty\}$
| $\in$ | `\in` | In / is a member of |
| $\notin$ | `\notin` | Not in / is not a member of |
| $\subset$ | `\subset` | Subset |
| $\subseteq$ | `\subseteq` | Subset or equals |
| $\nsubseteq$ | `\nsubseteq` | Not subset or equals |
| $\cup$ | `\cup` | Set Union |
| $\cap$ | `\cap` | Set Intersection |

### Logic

| Symbol | LaTeX | English |
| - | - | - |
| $\forall$ | `\forall` | Forall. Universal quantification. For every 'thing', something is true |
| $\exists$ | `\exists` | Exists. Existential quantification. For at least one 'thing', something is true |
| $\nexists$ | `\nexists` | Not Exists |
| $\lnot$ | `\lnot` | Not
| $\lor$ | `\lor` | Or
| $\land$ | `\land` | And
| $\bot$ | `\bot` | Bottom / false
| $\top$ | `\top` | Top / true
| $.$ | `.` | Dot
| $\vdash$ | `\vdash` | Turnstile

## Arrows

| Symbol | LaTeX | English |
| - | - | - |
| $\implies$ | `\implies` | Implies |
| $\impliedby$ | `\impliedby` | Implied by |
| $\to$ | `\to` | To / short thin right arrow |
| $\rightarrow$ | `\rightarrow` | short thin right arrow
| $\longrightarrow$ | `\longrightarrow` | long thin right arrow |
| $\Rightarrow$ | `\Rightarrow` | short fat right arrow
| $\Longrightarrow$ | `\Longrightarrow` | long fat right arrow |
| $\gg$ | `\gg` | Two arrowhead (?)
| $\ggg$ | `\ggg` | Three arrowhead (?).

### Greek Letters

#### Lowercase

| Symbol | LaTeX | English |
| - | - | - |
| $\alpha$ | `\alpha` | a (short)
| $\beta$ | `\beta` | b
| $\gamma$ | `\gamma` | g
| $\delta$ | `\delta` | d
| $\epsilon$ | `\epsiolon` | e
| $\zeta$ | `\zeta` | z
| $\eta$ | `\eta` | a (long)
| $\theta$ | `\theta` | th
| $\iota$ | `\iota` | i
| $\kappa$ | `\kappa` | k
| $\lambda$ | `\lambda` | l
| $\mu$ | `\mu` | m
| $\nu$ | `\nu` | n
| $\xi$ | `\xi` | ks
| $\omicron$ | `\omicron` | o (short)
| $\pi$ | `\pi` | p
| $\rho$ | `\rho` | r
| $\sigma$ | `\sigma` | s
| $\tau$ | `\tau` | t
| $\upsilon$ | `\upsilon` | u
| $\phi$ | `\phi` | ph
| $\chi$ | `\chi` | kh
| $\psi$ | `\psi` | ps
| $\omega$ | `\omega` | o (long)

#### Uppercase

| Symbol | LaTeX | English |
| - | - | - |
| $\Alpha$ | `\Alpha` | a (short)
| $\Beta$ | `\Beta` | b
| $\Gamma$ | `\Gamma` | g
| $\Delta$ | `\Delta` | d
| $\Epsilon$ | `\Epsiolon` | e
| $\Zeta$ | `\Zeta` | z
| $\Eta$ | `\Eta` | a (long)
| $\Theta$ | `\Theta` | th
| $\Iota$ | `\Iota` | i
| $\Kappa$ | `\Kappa` | k
| $\Lambda$ | `\Lambda` | l
| $\Mu$ | `\Mu` | m
| $\Nu$ | `\Nu` | n
| $\Xi$ | `\Xi` | ks
| $\Omicron$ | `\Omicron` | o (short)
| $\Pi$ | `\Pi` | p
| $\Rho$ | `\Rho` | r
| $\Sigma$ | `\Sigma` | s
| $\Tau$ | `\Tau` | t
| $\Upsilon$ | `\Upsilon` | u
| $\Phi$ | `\Phi` | ph
| $\Chi$ | `\Chi` | kh
| $\Psi$ | `\Psi` | ps
| $\Omega$ | `\Omega` | o (long)

### Inserting text in an expression

$$\text{text, then expression $x$}$$

```
$$\text{text, then expression $x$}$$
```

### Functions

$$
f(x)=
\begin{cases}
case1\newline
case2
\end{cases}
$$

```
$$
f(x)=
\begin{cases}
case1\newline
case2
\end{cases}
$$
```

### Formatting Symbols

#### Spacing

| Symbol | LaTeX | English |
| - | - | - |
| $a \! a$ | `\!` | Negative space
| $a a$ | `a a` | no space
| $a \, a$ | `\,` | Small space
| $a \: a$ | `\:` | Medium space
| $a \; a$ | `\;` | Large space
| $a\quad a$ | `\quad` | horizontal space
| $a \qquad a$ | `\qquad` | large horizontal space

#### Superscript / Subscript

| Symbol | LaTeX | English |
| - | - | - |
| $x^2$ | `x^2` | Superscript |
| $x^{n+2}$ | `x^{n+2}` | Superscript expression |
| $x_1$ | `x_1` | Subscript |
| $x_{n-1}$ | `x_{n-1}` | Subscript expression |

#### Font Colors

See [LaTeX Colors](https://latexcolor.com/)

| Symbol | LaTeX | English |
| - | - | - |
| $\color{red}{x}$ | `\color{red}{x}` | Color font with named color
| $\color{#FEFE33}{x}$ | `\color{#FEFE33}{x}` | Color font with hex color

#### Font Sizes

| Symbol | LaTeX | English |
| - | - | - |
| $\Huge M$ | `\Huge` | +5
| $\huge M$ | `\huge` | +4
| $\LARGE M$ | `\LARGE` | +3
| $\Large M$ | `\Large` | +2
| $\large M$ | `\large` | +1
| $\normalsize M$ | `\normalsize` | 0
| $M$ | - | 0
| $\small M$ | `small` | -1
| $\scriptsize M$ | `scriptsize` | -2
| $\tiny M$ | `tiny` | -3
