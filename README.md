# Latex_learn
展示一张效果图
![](./Tex/latex.png)
---

## 一、LaTeX简介

专业排版工具，尤其是文字中插入复杂的数学符号，有些导师直接要求论文必须用它来写。离线下载安装包2个多G,链接在这里[传送门](https://pan.baidu.com/s/1lCNotdcchx-97FME8AXgsQ)，提取码：dpzf

## 二、学习内容

1.10月20日和21日开始安装和学习，主要学习了目录结构和图片插入，索引部分还没学会。效果图在下面

![效果](http://p6hlch5jf.bkt.clouddn.com/pic.png) 

- 最简单的文字结构

```

%\documentclass{article}  %调用的宏，只支持英文
\documentclass[UTF8]{ctexart}%与上面功能相同，但支持汉语
\author{lijie}
\title{test}
\begin{document}%这块儿是主体，有begin，有end
\maketitle
hello,我想写中文，但那个texmaker真垃圾，还是vim好用！
\end{document}


```

- 文档、图片、标题结构

```

%\documentclass{article} %注意需要导包 \usepackage{caption} \usepackage{graphicx, subfig} \begin{document} \begin{figure} \centering %\includegraphics[width=.8\textwidth]{1.png} %1.png是图片文件的相对路径 \caption{best} %caption是图片的标题 \label{img} %此处的label相当于一个图片的专属标志，目的是方便上下文的引用 \end{figure} \end{document}
%\documentclass[•]{article}
\documentclass[UTF8]{ctexart}
\usepackage{caption}
\usepackage{float,amsmath,amsfonts,amssymb,eufrak,eucal }
\usepackage{graphicx,subfig}
\usepackage[superscript]{cite}%引用
\author{李杰}
\title{插入图片}
\begin{document}
	\maketitle
	\section{归途也还可爱，琴弦少了磁带}
		\begin{enumerate}
			\item 很喜欢陈鸿宇，声音沙哑，歌词沧桑，全是故事		
			\item 除此之外还有花粥，最初是通过《二十岁的某一天》认识她的，从里面听到了她的故事，从此一发不可收拾
			\item 还有比如朴树、张悬、宋冬野、赵雷等等，很多名字一时想不起
		\end{enumerate}
	\section{就老去吧！孤独别醒来}
		喜欢的武打明星首先是龙叔，从小看到大，如今苍老了很多，他的角色虽没有李连杰的正派，但是更喜欢他，因为真实。还有就是星爷，陪我度过青春岁月，小时候笑，现在完全笑不出来了，你演的就是人生。
	\begin{figure}
		\centering
		%\caption{uncle long}
		%\includegraphics[width=.8\textwidth]{long.jpg}%图片为本行宽的80%
		\includegraphics [width=3cm] {long.jpg}
		%将 file.eps 插入文档并且它的宽度被缩放到 3 英寸，高度也会 按相应的比例缩放
		\caption{龙叔啊，终于找到你了}%标题
		%\caption{uncle long}
		\label{img}%专属标题，方便上下文引用
	\end{figure}
	\section{随便写写}
	写一句我喜欢的歌词吧：我看见眼前的一马平川，和我身后的山花烂漫，眼前的周遭都与我无关，只留你的呻吟在我耳畔！
	\section{尝试一下插入公式}
	先从积分开始把，让我们来看看：\begin{equation*}\int_{-X}^{Y} \exp(z)\, dz\end{equation*}
	真是牛逼呀，代码里异常的丑！	\begin{equation*}\iint_{-X}^{Y} \exp(z)\, dx\,dy\end{equation*}
	其他就稍微举几个例子，如闭合曲线积分 ：\begin{equation*}\oint_{C} x^3\, dx + 4y^2\, dy\end{equation*}
	
	上括号：\begin{matrix} 5050 \\ \overbrace{ 1+2+\cdots+100 } \end{matrix}    下括号： $\underbrace{a+b+\cdots+z}$
	\\ 幂(我说的话怎么不见了)：$a^{2+2}$        求和公式也很牛：$\sum_{k=1}^N k^2$
	
	

\end{document}
```
代码后半部分效果展示
![](http://p6hlch5jf.bkt.clouddn.com/biaoti.png)

## 三、下一步打算

1. 准备尽快掌握如何调用dib文件，使文章更加灵活
2. 找到一个适合自己的模板，然后认真学习主要语法，或者直接找本书，专门突击，感觉学会后帮助很大，可以做别人做不了的事
3. 再花2个左右通宵，认真学习，不要花费太多时间，最多一周。了解需要用的主要语法

