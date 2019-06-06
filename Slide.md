```
\documentclass{beamer}
\usepackage[UTF8]{ctexcap}
\usebeamercolor{beaver}
\usetheme{AnnArbor}

\title{我的第一张幻灯片}
\subtitle{小试牛刀}
\author{王小龙}
\institute{西北师范大学知行学院}
\date{2019年6月4日}
\begin{document}
	% First Slide
	\frame{\titlepage}
	\section*{Outlines}
	\subsection{Part I: Review of Previous Lecture}
	\frame
	{
		\frametitle{Outline of Part I}
		\tableofcontents[part=1]
	}
	\subsection{Part II: Today’s Lecture}
	\frame{
		\frametitle{Outline of Part II}
		\tableofcontents[part=2]
	}
	\part{Review of Previous Lecture}
	\frame{\partpage}
	\section[Previous Lecture]{Summary of the Previous Lecture}
	\subsection{Topics}
	\frame{...}
	\subsection{Learning Objectives}
	\frame{...}
	\part{Today’s Lecture}
	\frame{\partpage}
	\section{Topic A}
	\frame{\tableofcontents[currentsection]}
	\subsection{Foo}
	\frame{...}
	\section{Topic B}
	\frame{\tableofcontents[currentsection]}
	\subsection{bar}
	\frame{...}
	
	

%	\begin{frame}
%	\titlepage
%	\end{frame}
%	\section{Android简介}
%	\begin{frame}[allowframebreaks,allowdisplaybreaks]{A Long Equation}
%	\begin{align}
%	\zeta(2) &= 1 + 1/4 + 1/9 + \cdots \\
%	&= ... \\
%	...
%	&= \pi^2/6.
%	\end{align}
%	\end{frame}
%	
%	\begin{frame}
%		\begin{itemize}
%			\item
%			Shown from first slide on.
%			\pause
%			\item
%			Shown from second slide on.
%			\begin{itemize}
%				\item
%				Shown from second slide on.
%				\pause
%				\item
%				Shown from third slide on.
%			\end{itemize}
%			\item
%			Shown from third slide on.
%			\pause
%			\item
%			Shown from fourth slide on.
%		\end{itemize}
%		%Shown from fourth slide on.
%		\begin{itemize}
%			\onslide
%			\item
%			Shown from first slide on.
%			\pause
%			\item
%			Shown from fifth slide on.
%		\end{itemize}
%	\end{frame}
%	\begin{frame}
%	\textbf{This line is bold on all three slides.}
%	\textbf<2>{This line is bold only on the second slide.}
%	\textbf<3>{This line is bold only on the third slide.}
%	\end{frame}
%	\begin{frame}
%	\only<1>{Initial text.}
%	\only<2>{Replaced by this on second slide.}
%	\only<3>{Replaced again by this on third slide.}
%	\end{frame}
%
%	\begin{frame}
%	Shown on first slide.
%	\onslide<2-3>
%	Shown on second and third slide.
%	\begin{itemize}
%		\item
%		Still shown on the second and third slide.
%		\onslide+<4->
%		\item
%		Shown from slide 4 on.
%	\end{itemize}
%	Shown from slide 4 on.
%	\onslide
%	Shown on all slides.
%	\end{frame}
%	
%	\begin{frame}{目录}
%	\tableofcontents
%	\end{frame}
%	\section{总结}
%	\begin{frame}{Slide two}{测试2}
%	现在才53
%	\end{frame}
\end{document}
```
