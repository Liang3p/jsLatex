# jsLatex
jsLaTeX is a jQuery plugin that lets you embed LaTeX directly into your website or blog.

This branch is forked from [dreasgrech/jsLatex](https://github.com/dreasgrech/jsLatex). 

## Diff from the master branch:
1. Only replace the escape character in equations.
2. Align inline equations.
3. Set SVG by default.

## Usage
Here's an example in this demo page:
![](http://ww1.sinaimg.cn/large/a92183f7gy1fqlaxgirnxj20p00k0gmh.jpg)

## Knownbugs:
Some Multi-line equations can't rendered correctly such as the Maxwell's equations , the API can't handdle double dollar `$$` syntax. But It's acceptable in single-line equation.

It's Highly Suggested to test on [this site](http://www.codecogs.com/latex/eqneditor.php) first.

For example:
The single-line equation `$$x=\frac{-b \pm \sqrt{\Delta }}{2a}=\frac{-b \pm \sqrt{b^{2}-4ac }}{2a}$$` can be rendered .
It will faild when you try to convert the multi-line equations:
```
$$
\begin{eqnarray}
\nabla\cdot\vec{E} &=& \frac{\rho}{\epsilon_0} \\
\nabla\cdot\vec{B} &=& 0 \\
\nabla\times\vec{E} &=& -\frac{\partial B}{\partial t} \\
\nabla\times\vec{B} &=& \mu_0\left(\vec{J}+\epsilon_0\frac{\partial E}{\partial t} \right)
\end{eqnarray}
$$
```
![](http://ww1.sinaimg.cn/large/a92183f7gy1fqlajt1j0kj20yu0cojtq.jpg)

Use single dollar is OK.
```
$
\begin{eqnarray}
\nabla\cdot\vec{E} &=& \frac{\rho}{\epsilon_0} \\
\nabla\cdot\vec{B} &=& 0 \\
\nabla\times\vec{E} &=& -\frac{\partial B}{\partial t} \\
\nabla\times\vec{B} &=& \mu_0\left(\vec{J}+\epsilon_0\frac{\partial E}{\partial t} \right)
\end{eqnarray}
$
```
![](http://ww1.sinaimg.cn/large/a92183f7gy1fqlak7kkd8j20ys0h7q5f.jpg)
