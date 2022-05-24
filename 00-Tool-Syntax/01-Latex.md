# LaTeX

Throughout this work, LaTeX will be used, especialy since GitHub markdown now renders it automatically via Mathjax. Below is a LaTeX cheatsheet. Symbols are mapped to their definition in LaTeX and their meaning in English. I use this also to verify that GitHub renders content correctly.

Sources used:
- [Using LaTeX in Markdown](https://ashki23.github.io/markdown-latex.html#latex)
- [List of LaTeX Symbols](https://latex.wikia.org/wiki/List_of_LaTeX_symbols)
- [TEX Commands available in MathJax](https://www.onemathematicalcat.org/MathJaxDocumentation/TeXSyntax.htm)

**Note:** You can right-click the rendered expression to get a Mathjax context menu. The following menu options may be helpful:
- `Show Math As > Tex Commands`: See what the underlying LaTeX is that produces that expression
- `Copy to Clipboard > Tex Commands`: Copy the underlying LaTeX to your clipboard

## LaTeX Tables

Since GitHub doesn't render LaTeX correctly when it's used in a table...
```markdown
| Symbol | LaTeX |
| - | - |
| $$\times$$ | `\times` |
| $\div$ | `\div` |
```

| Symbol | LaTeX |
| - | - |
| $$\times$$ | `\times` |
| $\div$ | `\div` |

... we'll use LaTeX to define a table-like view instead.

```markdown
$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& + &|& \text{+} &|& \mathrm{Add} &|\newline
&|& - &|& \text{-} &|& \mathrm{Subtract} &|\newline
&|& \times &|& \textbackslash \text{times} &|& \mathrm{Mutiply} &|\newline
&|& \div &|& \textbackslash \text{div} &|& \mathrm{Divide} &|\newline
\end{align*}
$$
```

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& + &|& \text{+} &|& \mathrm{Add} &|\newline
&|& - &|& \text{-} &|& \mathrm{Subtract} &|\newline
&|& \times &|& \textbackslash \text{times} &|& \mathrm{Mutiply} &|\newline
&|& \div &|& \textbackslash \text{div} &|& \mathrm{Divide} &|\newline
\end{align*}
$$

## Markdown Test

$Inline LaTeX Expression$

$$
Multi
Line
LaTeX
Expresion
$$

## Symbols

### Escaping Characters

See https://tex.stackexchange.com/questions/34580/escape-character-in-latex but note that such characters must be `\`-escaped **twice** (e.g. `\\{`, not `\{`).

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \\& &|& \textbackslash \textbackslash \\& &|& \text{Ampersand} &|\newline
&|& \\% &|& \textbackslash \textbackslash \\% &|& \text{Percentage} &|\newline
&|& \\$ &|& \textbackslash \textbackslash \\$ &|& \text{Dollar} &|\newline
&|& \\# &|& \textbackslash \textbackslash \\# &|& \text{Hash} &|\newline
&|& \\_ &|& \textbackslash \textbackslash \\_ &|& \text{Underscore} &|\newline
&|& \\{ &|& \textbackslash \textbackslash \\{ &|& \text{Left Brace} &|\newline
&|& \\} &|& \textbackslash \textbackslash \\} &|& \text{Right Brace} &|\newline
&|& \textasciitilde \quad &|& \textbackslash \text{textasciitilde} \quad &|& \text{Tilde} &|\newline
&|& \textbackslash \quad &|& \textbackslash \text{textbackslash} \quad &|& \text{Backslash} &|\newline
&|& \textasciicircum \quad &|& \textbackslash \text{textasciicircum} \quad &|& \text{Caret} &|\newline
\end{align*}
$$

### Boundary Characters

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \\{ \quad &|& \textbackslash \textbackslash \\{ \quad &|& \text{Left Brace} &|\newline
&|& \\} \quad &|& \textbackslash \textbackslash \\} \quad &|& \text{Right Brace} &|\newline
&|& ( \quad &|& \text{(} \quad &|& \text{Left parenthesis} &|\newline
&|& ) \quad &|& \text{)} \quad &|& \text{Right parenthesis} &|\newline
&|& [ \quad &|& \text{[} \quad &|& \text{Left bracket} &|\newline
&|& ] \quad &|& \text{]} \quad &|& \text{Right bracket} &|\newline
\end{align*}
$$

### Math operators

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX}      &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& + &|& \text{+} &|& \text{Add} &|\newline
&|& - &|& \text{-} &|& \text{Subtract} &|\newline
&|& \times &|& \textbackslash \text{times} &|& \text{Mutiply} &|\newline
&|& \div &|& \textbackslash \text{div} &|& \text{Divide} &|\newline
\end{align*}
$$

### Equality

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX}      &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& = &|& \text{=} &|& \text{Equals} &|\newline
&|& \ne &|& \textbackslash \text{ne} &|& \text{Not equals} &|\newline
&|& < &|& \text{<} &|& \text{Less than} &|\newline
&|& \le &|& \textbackslash \text{le} &|& \text{Less than or equal to} &|\newline
&|& > &|& \text{>} &|& \text{Greater than} &|\newline
&|& \ge &|& \textbackslash \text{ge} &|& \text{Greater than or equal to} &|\newline
\end{align*}
$$

### Common Mathematical Symbols/Constants

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \infty &|& \textbackslash \text{infty} &|& \text{Infinity} &|\newline
&|& \sum &|& \textbackslash \text{sum} &|& \text{Sum} &|\newline
&|& \prod &|& \textbackslash \text{prod} &|& \text{Product} &|\newline
\end{align*}
$$

### Sets/Collections

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \varnothing &|& \textbackslash \text{varnothing} &|& \text{Empty set} &|\newline
&|& \\{ 1, 2 \\} &|& \textbackslash \textbackslash \\{ \text{1, 2} \textbackslash \textbackslash \\} &|& \text{A set of two elements: 1 and 2} &|\newline
&|& \mathbb{N} &|& \textbackslash \text{mathbb} \\{ \text{N} \\} &|& \text{Natural numbers: } i \in \\{ 1, 2 ..., \infty \\} &|\newline
&|& \mathbb{Z} &|& \textbackslash \text{mathbb} \\{ \text{Z} \\}  &|& \text{Integers: } i \in \\{ -\infty, -1, 0, 1 ..., \infty \\} &|\newline
&|& \in &|& \textbackslash \text{in} &|& \text{In / is a member of} &|\newline
&|& \notin &|& \textbackslash \text{notin} &|& \text{Not in / is not a member of} &|\newline
&|& \subset &|& \textbackslash \text{subset} &|& \text{Subset} &|\newline
&|& \subseteq &|& \textbackslash \text{subseteq} &|& \text{Subset or equal to} &|\newline
&|& nsubseteq &|& \textbackslash \text{nsubseteq} &|& \text{Not subset or equal to} &|\newline
&|& \cup &|& \textbackslash \text{cup} &|& \text{Set union} &|\newline
&|& \cap &|& \textbackslash \text{cap} &|& \text{Set intersection} &|\newline
\end{align*}
$$

### Logic

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \forall &|& \textbackslash \text{forall} &|& \text{Forall. Universal quantification. For every 'thing', something is true.} &|\newline
&|& \exists &|& \textbackslash \text{exists} &|& \text{Exists. Existential quantification. For at least one 'thing', something is true.} &|\newline
&|& \nexists &|& \textbackslash \text{nexists} &|& \text{Not exists} &|\newline
&|& \lnot &|& \textbackslash \text{lnot} &|& \text{Logical Not} &|\newline
&|& \lor &|& \textbackslash \text{lor} &|& \text{Logical Or} &|\newline
&|& \land &|& \textbackslash \text{land} &|& \text{Logical And} &|\newline
&|& \bot &|& \textbackslash \text{bot} &|& \text{Bottom / false} &|\newline
&|& \top &|& \textbackslash \text{top} &|& \text{Top / true} &|\newline
&|& . &|& \text{.} &|& \text{Dot} &|\newline
&|& \vdash &|& \textbackslash \text{vdash} &|& \text{Turnstile} &|\newline
\end{align*}
$$

## Arrows

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \implies &|& \textbackslash \text{implies} &|& \text{Implies} &|\newline
&|& \impliedby &|& \textbackslash \text{impliedby} &|& \text{Implied by} &|\newline
&|& \to &|& \textbackslash \text{to} &|& \text{To / short thin right arrow} &|\newline
&|& \rightarrow &|& \textbackslash \text{rightarrow} &|& \text{short thin right arrow} &|\newline
&|& \longrightarrow &|& \textbackslash \text{longrightarrow} &|& \text{long thin right arrow} &|\newline
&|& \Rightarrow &|& \textbackslash \text{Rightarrow} &|& \text{short fat right arrow} &|\newline
&|& \Longrightarrow &|& \textbackslash \text{Longrightarrow} &|& \text{long fat right arrow} &|\newline
&|& \gg &|& \textbackslash \text{gg} &|& \text{Two arrowhead (?)} &|\newline
&|& \ggg &|& \textbackslash \text{ggg} &|& \text{Three arrowhead (?)} &|\newline
\end{align*}
$$

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

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& a \\! a &|& \textbackslash \textbackslash \text{!} &|& \text{Negative space} &|\newline
&|& a a &|& \text{a a} &|& \text{No space} &|\newline
&|& a \\, a &|& \textbackslash \textbackslash \text{,} &|& \text{Small space} &|\newline
&|& a \\: a &|& \textbackslash \textbackslash \text{:} &|& \text{Medium space} &|\newline
&|& a \\; a &|& \textbackslash \textbackslash \text{;} &|& \text{Large space} &|\newline
&|& a \quad a &|& \textbackslash \text{quad} &|& \text{Horizontal space} &|\newline
&|& a \qquad a &|& \textbackslash \text{qquad} &|& \text{Large horizontal space} &|\newline
\end{align*}
$$


#### Superscript / Subscript

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& x^2 &|& \text{x} \textasciicircum \text{2} &|& \text{Superscript} &|\newline
&|& x^{n+2} &|& \text{x} \textasciicircum \\{ \text{n+2} \\} &|& \text{Superscript expression} &|\newline
&|& x2 &|& \text{x2} &|& \text{No super/sub script} &|\newline
&|& x_2 &|& \text{x} \\_ \text{2} &|& \text{Subscript} &|\newline
&|& x_{n+2} &|& \text{x} \\_ \\{ \text{n+2} \\} &|& \text{Subscript expression} &|\newline
\end{align*}
$$

#### Font Colors

See [LaTeX Colors](https://latexcolor.com/)

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \color{red}{x} &|& \textbackslash \text{color} \\{ \text{red} \\} \\{ \text{x} \\} &|& \text{Set font color to named color} &|\newline
&|& \color{#FEFE33}{x} &|& \textbackslash \text{color} \\{ \\# \text{FEFE33} \\} \\{ \text{x} \\} &|& \text{Set font color to hex color} &|\newline
\end{align*}
$$

#### Font Sizes

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \Huge M &|& \textbackslash \text{Huge M} &|& \text{+5} &|\newline
&|& \huge M &|& \textbackslash \text{huge M} &|& \text{+4} &|\newline
&|& \LARGE M &|& \textbackslash \text{LARGE M} &|& \text{+3} &|\newline
&|& \Large M &|& \textbackslash \text{Large M} &|& \text{+2} &|\newline
&|& \large M &|& \textbackslash \text{large M} &|& \text{+1} &|\newline
&|& \normalsize M &|& \textbackslash \text{normalsize M} &|& \text{0} &|\newline
&|& M &|& \text{M} &|& \text{0} &|\newline
&|& \small M &|& \textbackslash \text{small M} &|& \text{-1} &|\newline
&|& \scriptsize M &|& \textbackslash \text{scriptsize M} &|& \text{-2} &|\newline
&|& \tiny M &|& \textbackslash \text{tiny M} &|& \text{-3} &|\newline
\end{align*}
$$
