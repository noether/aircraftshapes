# aircraftshapes
Aircraft shapes for use with the [PGF/TikZ](https://www.ctan.org/pkg/pgf?lang=en) LaTeX package. It currently defines shapes for `aircraft side` and `aircraft top` corresponding to the side and top views of aircraft, respectively.

## Example

```latex
\documentclass{article}

\usepackage{tikz}
\usepackage{aircraftshapes}

\begin{document}

\begin{figure}
	\begin{tikzpicture}
	\node [aircraft side,fill=black,minimum width=1cm,rotate=10] at (0,0) {};
	\node [aircraft side,fill=black,minimum width=1cm,xscale=-1] at (5,1) {}; 
	\end{tikzpicture}
	\caption{Aircraft side.}
\end{figure}

\begin{figure}
	\begin{tikzpicture}
	\node [aircraft top,fill=black,minimum width=1cm,rotate=30] at (0,0) {};
	\node [aircraft top,fill=black,minimum width=1cm,xscale=-1] at (5,1) {}; 
	\end{tikzpicture}
	\caption{Aircraft top.}
\end{figure}

\begin{figure}
	\centering
	\begin{tikzpicture}
	\node [quadcopter top,minimum width=1cm] at (0,0) {};
	\node [quadcopter top,minimum width=1cm,rotate=20] at (5,1) {}; 
	\end{tikzpicture}
	\caption{Quadcopter top.}
\end{figure}

\end{document}
```
