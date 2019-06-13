```
\documentclass[slidestop,compress,mathserif]{beamer}
\usepackage[UTF8]{ctexcap}
%\usepackage{xcolor}%用于混合颜色
%\xdefinecolor{lavendar}{rgb}{0.8,0.6,1}
\xdefinecolor{olive}{cmyk}{0.64,0,0.95,0.4}
\colorlet{olive}{red!60!black}
%\colorlet{structure}{red!60!black}中的structure指的是预先定义的颜色，用后面的新配的颜色替换，如上面这一句将自己之前预先定义的olive导航颜色用red!60!black替换
\usecolortheme[named=olive]{structure}

%\usepackage[bars]{beamerthemetree} % Beamer主题样式v 2.2
\usetheme{Antibes} % Beamer主题样式v 3.0
\usecolortheme{lily} % Beamer颜色主题样式
%\useoutertheme[subsection=false,footline=authortitle]{miniframes}

%\beamertemplateshadingbackground{yellow!5!white}{blue!5}
%\beamertemplategridbackground[1cm]

\usestructuretemplate{\color{structure}}{} 
%\beamertemplateshadingbackground{yellow!50}{magenta!50}
\title{我的Beamer学习}
\author{王小龙}
\institute{兰州交通大学}
%\colorlet{structure}{red!60!black}
\begin{document}
	\begin{frame} % Cover slide
		\titlepage
	\end{frame}
	\begin{frame}%{First Slide}{副标题}
		\frametitle{First Slide}
		\framesubtitle{副标题}
		手机的肌肤设计的就是打飞机了空间
	\end{frame}
	\begin{frame}
	空白帧，没有标题
	\end{frame}
	
	
	\begin{frame}
	
	\begin{enumerate}
	
	\item 第一项
	\item 第而项
	\item 第三项
	\end{enumerate}
	\end{frame}
	
	\begin{frame}
	\begin{itemize}
	\item 第一项
	\item 第而项
	\item 第三项
	\end{itemize}
	\end{frame}
	
	\begin{frame}
	\begin{description}
	\item [红色：]热情、活泼
	\item [蓝泽：]蓝猫、大家法律框架
	\item [审理：]三等奖、是大家分开了
	\end{description}
	\end{frame}
	\section{FourthSection}
	\begin{frame}
	\begin{block}{重要内容}
	今天答辩顺利通过
	\end{block}
	\end{frame}
	
	\begin{frame}
	\begin{alertblock}{提醒重要内容}
	今天答辩顺利通过
	\end{alertblock}
	\end{frame}
	
	\begin{frame}
	\begin{exampleblock}{重要案例}
	今天答辩顺利通过\\
	今天工作很多
	\end{exampleblock}
	\end{frame}
	
	\begin{frame}
	\begin{theorem}
	微积分基本公式：$\int_{a}^{b}f(x)\mathrm{d}x=F(b)-F(a)$
	\end{theorem}
	\end{frame}
\end{document}%也可以用 \frame{\titlepage}}代替 (在Beamer v 2.2 宏包中) 
```
```
\documentclass{beamer}
\usepackage[UTF8]{ctexcap}
\usetheme{AnnArbor}
%\usebeameroutertheme{split}
\title{我的第一张幻灯片}
\subtitle{小试牛刀}
\author{王小龙}
\institute{西北师范大学知行学院}
\date{2019年6月4日}
%\useoutertheme{infolines}
%\useinnertheme{rectangles}
\begin{document}
	\begin{frame}
		\titlepage
	\end{frame}
	%========设置frametitle剧中============%
	\setbeamercolor{frametitle}{fg=red}
	\setbeamerfont{frametitle}{series=\bfseries}
	\setbeamertemplate{frametitle}
	{
%		\fbox{%
%			\parbox{\textwidth}{%
%				\begin{centering}
%					\vspace*{5ex}\insertframetitle\par
%				\end{centering}
%			}%
%		}
		\begin{textblock}[1]
			\color{blue}{\insertframetitle}
		\end{textblock}
	}
	%==============end====================%
	\begin{frame}{目\quad 录}
		\tableofcontents
	\end{frame}
\end{document}
```
