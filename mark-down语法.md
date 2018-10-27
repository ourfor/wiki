<!-- TITLE: MarkDown语法 -->
<!-- SUBTITLE: A quick summary of MarkDown语法 -->

# Markdown语法
一级标题: #
二级标题: ##
等等...

```markdown
# 算法概述
## 递归与分治策略
```

加粗: **第一个认识的人就是你**
```markdown
**第一个认识的人就是你**
```
倾斜: *很高兴*
```markdown
*很高兴*
```
加粗并倾斜: ***nice***
```markdown
***nice***
```
插入代码：
- 插入c语言代码：
```c
#include <iostream>
#include <stdio.h>
int main(){
    printf("Hello world\n");
    return 0;
}
```

```markdown
```c
#include <iostream>
#include <stdio.h>
int main(){
    printf("Hello world\n");
    return 0;
}
```   
```

- 插入shell命令
```bash
sudo dnf install git -y
sudo dnf update -y
```

```markdown
```bash
sudo dnf install git -y
sudo dnf update -y
```     
```

规则就是三个反引号+需要` 语法高亮 `的<strong>语言类型</strong>

引用书中的话或名人名言:

> 书籍是人类进步的阶梯 ---- 高尔基

```markdown
> 书籍是人类进步的阶梯 ---- 高尔基
```

小黑点:

- 你还是这么好看

```markdown
- 你还是这么好看
```

任务列表(有x显示为勾选，留空表示不勾选):
- [x] 高等数学
- [ ] 线性代数

```markdown
- [x] 高等数学
- [ ] 线性代数
```

反白:

```markdown
` root ` 在Unix/Linux操作系统中是指具有最高权限的用户
```

` root ` 在Unix/Linux操作系统中是指具有最高权限的用户

插入图片:
```markdown
![life](https://i.loli.net/2018/10/06/5bb815d8e14fd.jpg)
```

![life](https://i.loli.net/2018/10/06/5bb815d8e14fd.jpg)

- 方括号内部是对图片的描述，在github是不会显示出来的,也就是html中的alt
- 圆括号里面的网址可以是图片的绝对路径地址也可以是相对路径

添加超链接:
[GitHub](https://github.com)
```markdown
[GitHub](https://github.com)
```
表格:

```markdown
|这是表头|A|B|
|:-|-:|:-:|
|h|a|b|
```
实际效果:

|这是表头|A|B|
|:-|-:|:-:|
|h|a|b|

- ` :- ` 这是左对齐
- ` -: ` 这是右对齐
- ` :-: ` 这是居中对齐

显然这种表格是很简单的, 对于更加复杂的表格, markdown就有点心有余而力不足了, 还好兼容html, 我们就可以用html的方式插入表格:

<table class="table">
<th>
  <td align=center>星期一</td>
  <td align=center>星期二</td>
  <td align=center>星期三</td>
  <td align=center>星期四</td>
  <td align=center>星期五</td>
  </th>
  <tr>
  <td>第一节</td>
  <td align=center rowspan=2>高等数学A(理化214)</td>
  <td align=center rowspan=2>线性代数(理化327)</td>
  <td align=center rowspan=4>软件综合(一)(机房)</td>
  <td align=center rowspan=2>程序设计基础(理化327)</td>
  <td align=center rowspan=4>软件综合(一)(机房)</td>
  </tr>
  <tr>
  <td>第二节</td>
  </tr>
  <tr>
  <td>第三节</td>
  <td align=center rowspan=2>程序设计基础(理化327)</td>
  <td align=center rowspan=2>大学英语(至105)</td>
  <td align=center rowspan=2>大学体育(体育馆)</td>
  </tr>
  <tr>
  <td>第四节</td>
  </tr>
  <tr>
  <td align=center>午安</td>
  <td align=center colspan=5>我的课表居然这么满🍎🍏🍐🍑🍒🍓🥝🍅</td>
  </tr>
  <tr>
  <td>第五节</td>
  <td align=center rowspan=4>程序设计基础(机房)</td>
  <td align=center rowspan=3>面向对象软件方法学(至308)</td>
  <td align=center rowspan=3>算法分析与设计(至308)</td>
  <td></td>
  <td align=center rowspan=3>操作系统(至116)</td>
  </tr>
  <tr>
  <td>第六节</td>
  <td></td>
  
  </tr>
  <tr>
  <td>第七节</td>
  <td></td>
  </tr>
  <tr>
  <td>第八节</td>
  <td></td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
  <tr>
  <td align=center>傍晚</td>
  <td align=center colspan=5>认识你真好🍇🍈🍉🍊🍋🍌🍍</td>
  </tr>
  <tr>
  <td>第一节</td>
  <td align=center rowspan=3>Java校选课(至502)</td>
  <td></td>
  <td></td>
  <td></td>
  <td align=center rowspan=3>概率论与数理统计(至117)</td>
  </tr>
  <tr>
  <td>第二节</td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
  <tr>
  <td>第三节</td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
</table>

<details><summary><strong>HTML代码</strong></summary>
```html
<table>
<th>
  <td align=center>星期一</td>
  <td align=center>星期二</td>
  <td align=center>星期三</td>
  <td align=center>星期四</td>
  <td align=center>星期五</td>
  </th>
  <tr>
  <td>第一节</td>
  <td align=center rowspan=2>高等数学A(理化214)</td>
  <td align=center rowspan=2>线性代数(理化327)</td>
  <td align=center rowspan=4>软件综合(一)(机房)</td>
  <td align=center rowspan=2>程序设计基础(理化327)</td>
  <td align=center rowspan=4>软件综合(一)(机房)</td>
  </tr>
  <tr>
  <td>第二节</td>
  </tr>
  <tr>
  <td>第三节</td>
  <td align=center rowspan=2>程序设计基础(理化327)</td>
  <td align=center rowspan=2>大学英语(至105)</td>
  <td align=center rowspan=2>大学体育(体育馆)</td>
  </tr>
  <tr>
  <td>第四节</td>
  </tr>
  <tr>
  <td align=center>午安</td>
  <td align=center colspan=5>我的课表居然这么满🍎🍏🍐🍑🍒🍓🥝🍅</td>
  </tr>
  <tr>
  <td>第五节</td>
  <td align=center rowspan=4>程序设计基础(机房)</td>
  <td align=center rowspan=3>面向对象软件方法学(至308)</td>
  <td align=center rowspan=3>算法分析与设计(至308)</td>
  <td></td>
  <td align=center rowspan=3>操作系统(至116)</td>
  </tr>
  <tr>
  <td>第六节</td>
  <td></td>
  
  </tr>
  <tr>
  <td>第七节</td>
  <td></td>
  </tr>
  <tr>
  <td>第八节</td>
  <td></td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
  <tr>
  <td align=center>傍晚</td>
  <td align=center colspan=5>认识你真好🍇🍈🍉🍊🍋🍌🍍</td>
  </tr>
  <tr>
  <td>第一节</td>
  <td align=center rowspan=3>Java校选课(至502)</td>
  <td></td>
  <td></td>
  <td></td>
  <td align=center rowspan=3>概率论与数理统计(至117)</td>
  </tr>
  <tr>
  <td>第二节</td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
  <tr>
  <td>第三节</td>
  <td></td>
  <td></td>
  <td></td>
  </tr>
</table>
```
</details>


- 可以参考文档[MarkDown语法](https://docs-legacy.requarks.io/wiki/user-guide/markdown-syntax)