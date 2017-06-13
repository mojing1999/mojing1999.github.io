---

layout: post
title: "Markdown Syntax"
description: "markdown syntax study"
category: "Other"
tags: [markdown, study]


---



---

[TOC]

---
### 1. 斜体和粗体
使用 * 和 ** 表示斜体和粗体。
实例: 
这是*斜体*, 这是**粗体**。

### 2. 分级标题
使用 === 表示一级标题， 使用 --- 表示二级标题。
示例:
```
这是一个一级标题
=======================================

这是一个二级标题
--------------------------------------

### 这是一个三级标题
```

### 3. 外部链接
使用\[描述](链接地址) 为文字增加外链接
示例:
这是去往[Bing](https://www.bing.com)的链接

### 4. 无序列表
使用 *， +， - 表示无序列表
示例:
- 无序列表项 一
- 无序列表项 二
- 无序列表项 三

### 5. 有序列表
使用数字和点表示有序列表
示例:
1. 有序列表项 一
2. 有序列表项 二
3. 有序列表项 三

### 6. 文字引用
使用 > 表示文字引用。
实例:
> 野火烧不尽，春风吹又生。

### 7. 行内代码块
使用\`代码\` 表示行内代码块。
示例:
让我们聊聊 `html` `HTML`

### 8. 代码块
使用 四个缩进空格 表示代码块
示例:
    这是一个代码块，此行左侧有四个不可见的空格
    
### 9. 插入图像
使用\!\[描述](图片链接) 插入图像
示例:
![我的头像](https://www.zybuluo.com/static/img/my_head.jpg)


# Cmd Markdown 高阶语法

### 1. 内容目录
在段落中填写`[TOC]` 以显示全文的内容的目录结构。

[TOC]

### 2. 标签分类
在编辑区任意行的列首位置输入以下代码给文稿标签:
标签： 数学 英语 Markdown
或者
Tags : 数学 英语 Markdown

### 3. 删除线
使用 ~~ 表示删除线。
~~这是一段错误的文本。~~

### 4. 注脚
使用 [^keyword] 表示注脚。

这是一个注脚[^footnote]的样例。

这个第二个注脚[^footnote]的样例。




---
## What is Markdown
Markdown is ....**粗体**, *斜体*
### 制作一份待办事宜[Todo 列表] ()

- [] 支持PDF
- [] 改进Cmd
- [x] 新增Todo 列表
- [x] 修复LaTex
- [x] 新增LaTex公式

### 2. 书写一个质能守恒公式[^LaTex]
质能守恒方程可以用一个很简洁的方程式 $E=mc^2$ 来表达

$$ 表示整行公式:
$$\sum_{i=1}^n a_i=0$$

$$f(x_1, x_x,\ldots,x_n) = x_1^2 + x_2^2 +\cdots + x_n^2 $$

$$\sum^{j-1}_{k=0}{\widehat{\gamma}_{kj} z_k}$$

访问 [MathJax](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference)参考更多使用方法。


---

### 6. 加强的代码块
支持四十一种编程语言的语法高亮显示， 行号显示。
非代码示例:
```
$ sudo apt-get install vim
```
### 7. 高亮一段代码

``` C
int main(int argc, char *argv)
{
return 0;
}
```

---

### 8. 高效绘制[流程图]()
示例1
```flow
st=>start: Start
op=>operation: Your Operatation
cond=>condition: Yes or No?
e=>end

st->op->cond
cond(yes)->e
cond(no)->op

```

---
示例2
```flow
st=>start: Start|past:>http://www.google.com[blank]
e=>end: End|future:>http://www.google.com
op1=>operation: My Operation|past
op2=>operation: Stuff|current
sub1=>subroutine: My Subroutine
cond=>condition: Yes or No?|approved:>http://www.google.com
c2=>condition: Good idea|rejected
io=>inputoutput: catch something...|futrue

st->op1(right)->cond
cond(yes,right)->c2
cond(no)->sub1(left)->op1
c2(yes)->io->e
c2(no)->op2->e

```

```flow
st=>start: Start
en=>end: End
op1=>operation: vision detection
cond=>condition: Result OK?
op2=>operation: send adjust param
op3=>operation: wait for adjust

st->op1->cond
cond(yes, right)->en
cond(no)->op2->op3(left)->op1

```







更多语法参考: [流程图语法参考](https://github.com/adrai/flowchart.js)


---

### 9. 高效绘制[序列图]
```seq
Alice->Bob: Hello Bob, how are you?
Note right of Bob: Bob thinks
Bob->Alice: I am good thanks!


```
示例2
```seq
Title: Here is a title
A->B: Normal line
B-->C: Dashed line
C->>D: Open arrow
D-->>A: Dashed open arrow
```
#### 更多语法参考：[序列图语法参考](http://bramp.github.io/js-sequence-diagrams/)
---

### 10. 高效绘制[甘特图]
```gantt
    title 项目开发流程
    section 项目确定
        需求分析    :a1, 2017-04-30, 3d
        可行性报告  :after a1, 5d
        概念验证    :5d
    section 项目实施
        概要设计    :2017-04-30, 5d
        详细设计    :2017-05-03, 10d
        编码        :2017-05-05, 20d
        测试        :2017-05-20, 10d
    section 发布验收
        发布        :2d
        验收        :3d
        
```
#### 更多语法参考: [甘特图语法参考](https://knsv.github.io/mermaid/#mermaid)
---

### 11. 绘制表格
| 项目   | 价格 | 数量 |
| ----  | ---: | :---: |
| 计算机 | \$1600 | 5 |
| 手机 | \$12 | 12 |
| 线 | \$1 | 234 |


### 12. 更详细语法说明
想要查看更详细的语法说明， 可以参考我们准备的[Markdown ][1] , 进阶用户可以参考[Cmd Markdown][2] 了解更多高级功能

---
### 13. 待办事宜 Todo 列表
使用带有[ ] 或 [x] (未完成或已完成) 项的列表语法撰写一个代办事宜列表， 并且支持子列表嵌套以及混用Markdown语法， 例如：

- [ ] **Cmd Markdown 开发**
    - [ ] 改进以PDF格式导出文稿
    - [x] 新增Todo列表功能 [语法参考](https://github.com/blog/1375-task-lists-in-gfm-issues-pulls-comments)
    - [x] 改进LaTex功能
        - [x] 修复LaTex公式渲染问题
        - [x] 新增LaTex公式编号功能 [语法参考](http://docs.mathjax.org/en/latest/tex.html#tex-eq-numbers)
- [ ] **七月旅行计划**

[^footnote]: 这是一个 *注脚* 的**文本**。
[^footnote2]: 这是另一个 *注脚* 的**文本**。


