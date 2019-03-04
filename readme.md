![banner](http://lc-jOYHMCEn.cn-n1.lcfile.com/728c17816cf608b50d17.jpeg)

正则表达式（Regular Expression）是很多程序员，甚至是一些有了十多年经验的开发者薄弱的一项技能。大家都很多时候都会觉得正则表达式难记、难学、难用，但不可否认的是正则表达式是一项很重要的技能，所有我将学习和使用正则表达式时的关键点整理如下，供大家参考。

语言：

不同语言中的正则表达式写法有少许差异，本文将使用Javascript的写法。

工具：

本文使用在线正则表达式调试工具 [regex101](https://regex101.com/) 

# 开始

在Javascript中，一个正则表达式以 `/` 开头和结尾，所以简单至 `/hello regexp/` 就是一个正则表达式。在regex101中的样子（regex101支持在不同语言之间切换、解释你的正则表达式、显示匹配信息、提供常用语法参考等功能）：

![1](http://lc-jOYHMCEn.cn-n1.lcfile.com/b0fd70f342fe3e7b6a33.png)

# Flags（标志符或修饰符）

Flags可以影响正则表达式的匹配方式。

## g（global/全局匹配）

正则表达式默认只会返回第一个匹配结果，使用标志符`g`则可以返回所有匹配：

![flags-g](http://lc-jOYHMCEn.cn-n1.lcfile.com/fd92dcfa555f1d120980.png)

## i（case-insensitive/忽略大小写）

使用标志符`i`可以在匹配时忽略英文字母的大小写：

![flags-i](http://lc-jOYHMCEn.cn-n1.lcfile.com/4a2cd746bb876b89d063.png)

## ToDo Other Flags

# Character Sets（字符集合）

用于匹配字符集合中的任意一个字符，比如：

![Character Set](http://lc-jOYHMCEn.cn-n1.lcfile.com/c6bbc59ba0f200888c78.png)

或者匹配字符集的补集（任意不在集合中的字符），使用 `[^xxx]`表示补集，如：

![Negated Character Set](http://lc-jOYHMCEn.cn-n1.lcfile.com/e58dcbf07e1a64c89908.png)

集合或者补集也可以用一个范围表示，语法为 `[x-y]或[^x-y] `比如：

![Range Char Set](http://lc-jOYHMCEn.cn-n1.lcfile.com/faf09c4968045a365a6b.png)