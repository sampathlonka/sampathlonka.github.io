
\section{Introduction}
In this chapter we discuss, how to find optimal points for given function either in 
one variable or several variables. This is often called \emph{classical optimization}, 
even though many of the techniques are of recent origin. Occasionally these techniques can be used to solve real-world problems. These techniques frequently used to optimize the cost function in Machine Learning and Deep Learning algorithms.

\section{Optimization of Unconstrained Functions}
\subsection{Optimization of Unconstrained Functions of One Variable}
We start with some definitions:

\begin{Definition}\label{def1} Consider a continuous function $f:I=(a,b)\rightarrow \mathbb{R}.$
	\begin{enumerate} 
	\item   We say that $f$ has a global minimum/ absolute minimum at $x_1\in I$ if 
	\[f(x_1)\le f(x) \ \forall x\in I\]
	\item  We say that $f$ has a global maximum/ absolute maximum at $x_1\in I$ if 
	\[f(x_1)\ge f(x) \ \forall x\in I\]
	\item We say that $f$ has a global extremum/ absolute extremum at $x_1\in I$ if $f$ has either a global minimum or a global maximum at $x_1.$
	\item We say that $f$ has a local minimum/ relative minimum at $x_1\in I$ if there exists a real number $\delta>0$ such that 
	\[f(x_1)\le f(x)\ \forall x\in(x_1-\delta,x_1+\delta)\]
	\item We say that $f$ has a local maximum/ relative maximum at $x_1\in I$ if there exists a real number $\delta>0$ such that 
	\[f(x_1)\ge f(x)\ \forall x\in(x_1-\delta,x_1+\delta)\]
	\item We say that $f$ has a local extremum/ relative extremum at $x_1\in I$ if $f$ has either a local minimum or a local maximum at $x_1.$
	\item We say that $f$ has a stationary/ critical point at $x_1\in I$ if 
	$f$ is differentiable at $x_1$ and $f'(x_1)=0.$
	\end{enumerate}	