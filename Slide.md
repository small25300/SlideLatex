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
\usepackage[skins, breakable, theorems,fitting,most]{tcolorbox}% 用来生成各式各样的框
%\usepackage[absolute ,overlay]{textpos}
%\usepackage{tikz}
%定义一些表示长度的命令
%\newlength{\boxw}
%\newlength{\boxh}
%\newlength{\boxroundness}%表示文本盒圆角的半径大小
%\newlength{\shadowsize}%表示文本盒阴影的宽度
%\newlength{\tmpa}%在带有阴影的文本盒的绘制过程中起到一个中间变量的作用。
\usepackage{xcolor}
%\includeonlyframes{current}
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
		
		\begin{centering}%将整个文本框居中
			\begin{frametitlebox}
				\centering\insertframetitle\par
			\end{frametitlebox}
		\end{centering}
		
	}
	%==============end====================%
	\newtcolorbox{frametitlebox}{width=5cm, colback = yellow!85!red,colframe=red!5!white}%设置文本框命令及其参数

	\begin{frame}\frametitle{目\quad 录}
		\tableofcontents		
	\end{frame}

	\section{第一部分}
	\begin{frame}\frametitle{FirstSection}
	\tableofcontents[currentsection, currentsubsection]
		\begin{tcolorbox}[title = {I Love Sophia}]
			This is a \textbf{tcolorbox} with title.
			\tcblower
			Here, you see the lower part of the box.
		\end{tcolorbox}
	\end{frame}

	\section{第二部分}
	\begin{frame}
		\begin{tcolorbox}[title=Lower separated] This is the upper part.
			\tcblower
			This is the lower part.
		\end{tcolorbox}
	
		\begin{tcolorbox}[sidebyside,title=Lower separated]
			This is the upper part.
			\tcblower
			This is the lower part.
		\end{tcolorbox}
	\end{frame}	

	\section{第三部分}
	\begin{frame}
		\begin{tcolorbox}[upperbox=invisible,colback=white]
			This is a \textbf{tcolorbox} (but invisible).
			\tcblower
			This is the lower part.\\
			sdkljk
		\end{tcolorbox}
	\end{frame}
	
	\frame{\frametitle{Outline}\tableofcontents[currentsection]}
	
	\AtBeginSection[]{
	\frame{\frametitle{Outline}\tableofcontents[currentsection]}
	}
\end{document}
```
