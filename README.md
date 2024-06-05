# Simple Gantt chart for LaTeX

![image](https://github.com/jjholt/latex-gantt-chart/assets/876097/e057112c-a53a-446c-bc28-5a2f4708d2d8)


## Adding to your project
There are a few ways to use this
1. Copy the `tikzpicture` environment in `gant-chart.tex` directly into your project.
2. Import the standalone file:
```tex
% main.tex
\documentclass{article}
\usepackage[mode=buildnew]{standalone}
\usepackage{tikz}
\begin{document}
    \includestandalone[width=\textwidth]{gantt-chart}
\end{document}
```

## Usage
A new task can be created using:
``` tex
\task{index}{name}{start-index}{length}  
```
Examples:
``` tex
\task{1}{Task 1}{0}{3}  % Task 1 starting at the 0th quarter (Q1 2024) lasting 3 quarters
\task{2}{Task 2}{5}{6}  % Task 2 starting at the 5th quarter (Q2 2025) lasting 6 quarters
```
