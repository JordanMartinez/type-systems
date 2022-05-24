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

This is an inline LaTeX expression, "$y = x + 2$", in a paragraph.

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
&|& \textasciitilde &|& \textbackslash \text{textasciitilde} &|& \text{Tilde} &|\newline
&|& \textbackslash &|& \textbackslash \text{textbackslash} &|& \text{Backslash} &|\newline
&|& \textasciicircum &|& \textbackslash \text{textasciicircum} &|& \text{Caret} &|\newline
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

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \alpha &|& \textbackslash \text{alpha} &|& \text{a (short)} &|\newline
&|& \beta &|& \textbackslash \text{beta} &|& \text{b} &|\newline
&|& \gamma &|& \textbackslash \text{gamma} &|& \text{g} &|\newline
&|& \delta &|& \textbackslash \text{delta} &|& \text{d} &|\newline
&|& \epsilon &|& \textbackslash \text{epsilon} &|& \text{e} &|\newline
&|& \zeta &|& \textbackslash \text{zeta} &|& \text{z} &|\newline
&|& \eta &|& \textbackslash \text{eta} &|& \text{a (long)} &|\newline
&|& \theta &|& \textbackslash \text{theta} &|& \text{th} &|\newline
&|& \iota &|& \textbackslash \text{iota} &|& \text{i} &|\newline
&|& \kappa &|& \textbackslash \text{kappa} &|& \text{k} &|\newline
&|& \lambda &|& \textbackslash \text{lambda} &|& \text{l} &|\newline
&|& \mu &|& \textbackslash \text{mu} &|& \text{m} &|\newline
&|& \nu &|& \textbackslash \text{nu} &|& \text{n} &|\newline
&|& \xi &|& \textbackslash \text{xi} &|& \text{ks} &|\newline
&|& \omicron &|& \textbackslash \text{omicron} &|& \text{o (short)} &|\newline
&|& \pi &|& \textbackslash \text{pi} &|& \text{p} &|\newline
&|& \rho &|& \textbackslash \text{rho} &|& \text{r} &|\newline
&|& \sigma &|& \textbackslash \text{sigma} &|& \text{s} &|\newline
&|& \tau &|& \textbackslash \text{tau} &|& \text{t} &|\newline
&|& \upsilon &|& \textbackslash \text{upsilon} &|& \text{u} &|\newline
&|& \phi &|& \textbackslash \text{phi} &|& \text{ph} &|\newline
&|& \chi &|& \textbackslash \text{chi} &|& \text{kh} &|\newline
&|& \psi &|& \textbackslash \text{psi} &|& \text{ps} &|\newline
&|& \omega &|& \textbackslash \text{omega} &|& \text{o (long)} &|\newline
\end{align*}
$$
#### Uppercase

$$
\begin{align*}
&|& \mathrm{Symbol} &|& \mathrm{LaTeX} &|& \mathrm{English} &|\newline
&|& \mathrm{-} &|& \mathrm{-} &|& \mathrm{-} &|\newline
&|& \Alpha &|& \textbackslash \text{Alpha} &|& \text{a (short)} &|\newline
&|& \Beta &|& \textbackslash \text{Beta} &|& \text{b} &|\newline
&|& \Gamma &|& \textbackslash \text{Gamma} &|& \text{g} &|\newline
&|& \Delta &|& \textbackslash \text{Delta} &|& \text{d} &|\newline
&|& \Epsilon &|& \textbackslash \text{Epsilon} &|& \text{e} &|\newline
&|& \Zeta &|& \textbackslash \text{Zeta} &|& \text{z} &|\newline
&|& \Eta &|& \textbackslash \text{Eta} &|& \text{a (long)} &|\newline
&|& \Theta &|& \textbackslash \text{theta} &|& \text{th} &|\newline
&|& \Iota &|& \textbackslash \text{Iota} &|& \text{i} &|\newline
&|& \Kappa &|& \textbackslash \text{Kappa} &|& \text{k} &|\newline
&|& \Lambda &|& \textbackslash \text{Lambda} &|& \text{l} &|\newline
&|& \Mu &|& \textbackslash \text{Mu} &|& \text{m} &|\newline
&|& \Nu &|& \textbackslash \text{Nu} &|& \text{n} &|\newline
&|& \Xi &|& \textbackslash \text{Xi} &|& \text{ks} &|\newline
&|& \Omicron &|& \textbackslash \text{Omicron} &|& \text{o (short)} &|\newline
&|& \Pi &|& \textbackslash \text{Pi} &|& \text{p} &|\newline
&|& \Rho &|& \textbackslash \text{Rho} &|& \text{r} &|\newline
&|& \Sigma &|& \textbackslash \text{sigma} &|& \text{s} &|\newline
&|& \Tau &|& \textbackslash \text{Tau} &|& \text{t} &|\newline
&|& \Upsilon &|& \textbackslash \text{Upsilon} &|& \text{u} &|\newline
&|& \Phi &|& \textbackslash \text{Phi} &|& \text{ph} &|\newline
&|& \Chi &|& \textbackslash \text{Chi} &|& \text{kh} &|\newline
&|& \Ssi &|& \textbackslash \text{Psi} &|& \text{ps} &|\newline
&|& \Omega &|& \textbackslash \text{omega} &|& \text{o (long)} &|\newline
\end{align*}
$$

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
