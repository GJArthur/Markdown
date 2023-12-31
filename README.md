# Markdown 学习笔记

---

## 1. 标题

方式 1: 文字下一行加 ' === '（一级标题） 或者 ' --- '（二级标题）

> # 一级标题
>
> ## 二级标题
>
> > ```
> >  一级标题
> >  =================
> >
> >  二级标题
> >  -----------------
> > ```

方式 2: 文字前面加 ' # ' ，数量越多字体越小，' # ' 和文字之间空一格，才有效

> # 第一级
>
> ## 第二级
>
> ### 第三级
>
> #### 第四级
>
> ##### 第五级
>
> ###### 第六级
>
> > ```
> >  # 一级标题
> >  ## 二级标题
> >  ### 三级标题
> >  #### 四级标题
> >  ##### 五级标题
> >  ###### 六级标题
> > ```

---

## 2. 换行

方法 1：句子后面加两个及以上的空格然后换一行开始写
方法 2：空一行继续写

```
  这是第一行
  这是第二行

  这是第三行
```

---

## 3. 斜体

使用一对' \* '或者一对' _ '
如果前面文字紧挨着' _ ',前面加空格
例：这是第一 _行_

```
  *斜体文本*
  _斜体文本_

  例：这是第一 _行_
```

---

## 4. 粗体

使用两对' \* ' 或者 ' \_ '
**粗体文本**

```
  **粗体文本**
  __粗体文本__
```

---

## 5. 斜粗体

使用三对' \* '或者' \_ '
**_斜粗体_**

```
  ***斜粗体文本***
  ___斜粗体文本___
```

---

## 6. 分割线

```
  ***

  * * *

  *****

  - - -

  ----------
```

---

## 7. 删除线

使用两对' ~ '
使用英文符号
~~删除线~~

```
  ~~删除线~~
```

---

## 8. 下划线

<u> 下划线使用 HTML 里的</u> `<u> </u>`标签

```
  <u>下划线使用 HTML 里的</u>
```

---

## 9. 注脚

方式 1: 第一注脚 ^[RUNOOB]。

```
  第一注脚 ^[RUNOOB]。
```

方式 2: 第二注脚[^小羊]。
[^小羊]: 菜鸟教程

```
  第二注脚[^小羊]
  [^小羊]: 菜鸟教程
```

---

## 10. 无序列表

在列表选项前面加 ' \* ' , ' + '或者' - '
字符和字之间空一格

- 第一项

* 第二项

- 第三项

```
  * 第一项
  * 第二项
  * 第三项

  + 第一项
  + 第二项
  + 第三项


  - 第一项
  - 第二项
  - 第三项
```

---

## 11. 有序列表

在列表选项前面加数字和点，空一格

1. 第一项
2. 第二项
3. 第三项

**同级别下前面的序号数字可以为任何数，系统会自动进行排序**

```
  1. 第一项
  4. 第二项
  3. 第三项
```

---

## 12. 嵌套列表

1. 第一项
   - 元素一
   - 元素二
   3. 元素三
   4. 元素四
      - 元素五
      - 元素六
        - 元素七
2. 第二项

```
  1. 第一项
	- 元素一
	- 元素二
	3. 元素三
	5. 元素四
		- 元素五
		- 元素六
			- 元素七
  3. 第二项
```

#### 有序嵌套无序

```
  1. 第一项：
      - 第一项嵌套的第一个元素
      - 第一项嵌套的第二个元素
  2. 第二项：
      - 第二项嵌套的第一个元素
      - 第二项嵌套的第二个元素
```

---

## 13. 区块引用

使用' > '空一格，后面加区块里的内容

> 第一区 - 第一层
> 第一层里面
>
> > 第二层
> > 第二层里面
> >
> > > 第三层
> > > 第三层里面

> 第二区

```
> 最外层
> > 第一层嵌套
> > > 第二层嵌套
```

#### 区块中使用列表

> 区块中使用列表
>
> 1. 第一项
>    - 第一项
>    - 第二项
>    - 第三项
> 2. 第二项

```
> 区块中使用列表
> 1. 第一项
>     + 第一项
>     + 第二项
>     + 第三项
> 2. 第二项
```

#### 列表中使用区块

如果要在列表项目内放进区块，那么就需要在 ' > ' 前添加四个空格的缩进。

- 第一项
  > markdown
  > python
- 第二项

```
  * 第一项
      > markdown
      > python
  * 第二项
```

---

## 14. 写段落上的一个函数或片段的代码``

使用英文 esc 下面反引号\` \` , `printf()`函数

> \`printf()\`函数

#### 代码区块：一个 tab 键或者四个空格

    int x=4
    int y=7
    int z=x+y

```
    int x=4
    int y=7
    int z=x+y
```

#### 用\``` \```包裹代码可以指定语言

```c++
    int x=4
    int y=7
    int z=x+y
```

    ```c++
    int x=4
    int y=7
    int z=x+y
    ```

---

## 15. 链接

方式 1: 这是一个链接[菜鸟教程](https://www.runoob.com)

方式 2: <https://www.runoob.com>

```
方式1: [链接名称](链接地址)
	这是一个链接[菜鸟教程](https://www.runoob.com)
方式2: <链接地址>
	<https://www.runoob.com>
```

#### 高级链接

这个链接用 1 作为网址变量 [Apple][1]
这个链接用 bing 作为网址变量 [Bing][bing]
然后在文档的结尾为变量赋值（网址）

[1]: http://www.apple.com/
[bing]: http://www.bing.com/

```
这个链接用 1 作为网址变量 [Apple][1]
这个链接用 bing 作为网址变量 [Bing][bing]
然后在文档的结尾为变量赋值（网址）

[1]: http://www.apple.com/
[bing]: https://www.bing.com/
```

---

## 16. 图片

#### 插入图片 Markdown 语法代码：

`![图片alt](图片链接 "图片title")`

#### 对应的 HTML 代码：

`<img src="图片链接" alt="图片alt" title="图片title">`

    ![图片alt](图片链接 "图片title")

    1. 开头一个感叹号 !
    2. 接着一个方括号，里面放上图片的替代文字
    3. 接着一个普通括号，里面放上图片的网址，最后还可以用引号包住并加上选择性的 'title' 属性的文字。

![帅](image/wangye.jpeg "shuaige")

```
![alt 属性文本](图片地址)

![alt 属性文本](图片地址 "可选标题")

![帅](image/wangye.jpeg "shuaige")
```

#### 链接图片（点击图片跳转网页）

[![百度](image/baidu.jpeg "baidu")](https://baidu.com.cn)

```
[![百度](image/baidu.jpeg "baidu")](https://baidu.com.cn)

给图片增加链接，请将图像的Markdown 括在方括号中，然后将链接添加在圆括号中。
```

#### 插入网络图片

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")

```
![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png)

![RUNOOB 图标](http://static.runoob.com/images/runoob-logo.png "RUNOOB")
```

#### 可以把图片的网址赋值给文字

这个链接用 2 作为网址变量 [RUNOOB][2].
然后在文档的结尾为变量赋值（网址）

[2]: http://static.runoob.com/images/runoob-logo.png

```
这个链接用 2 作为网址变量 [RUNOOB][2].
然后在文档的结尾为变量赋值（网址）

[2]: http://static.runoob.com/images/runoob-logo.png
```

#### 插入图片

简单：

    ![alt text](/path/to/img.jpg "Title")

高级

    ![alt text][id]

    [id]: /path/to/img.jpg "Title"

HTML:

    <img src="/path/to/img.jpg" alt="alt text" title="Title" />

---

## 17. 表格

Markdown 制作表格使用 ' | ' 来分隔不同的单元格，使用 ' - ' 来分隔表头和其他行。

| 表头   | 表头   |
| ------ | ------ |
| 单元格 | 单元格 |
| 单元格 | 单元格 |

```
|  表头   | 表头  |
|  ----  | ----  |
| 单元格  | 单元格 |
| 单元格  | 单元格 |
```

#### 对齐方式：

-: 设置内容和标题栏居右对齐。
:- 设置内容和标题栏居左对齐。
:-: 设置内容和标题栏居中对齐。

| 左对齐 | 右对齐 | 居中对齐 |
| :----- | -----: | :------: |
| 格     |     格 |    格    |
| 单元格 | 单元格 |  单元格  |

```
| 左对齐 | 右对齐 | 居中对齐 |
| :-----| ----: | :----: |
| 单元格 | 单元格 | 单元格 |
| 单元格 | 单元格 | 单元格 |
```

### 高级设置：

不在 Markdown 涵盖范围之内的标签，都可以直接在文档里面用 HTML 撰写。
目前支持的 HTML 元素有：`<kbd> <b> <i> <em> <sup> <sub> <br>` 等 ，如：

使用 <kbd>Ctrl</kbd>+<kbd>Alt</kbd>+<kbd>Del</kbd> 重启电脑

---

## 18. 转译

反斜杠进行转译

**文本加粗**
\*\* 正常显示星号 \*\*

```
**文本加粗**
\*\* 正常显示星号 \*\*
```

每个符号前都需要反斜杠进行转译

---

## 19. 公式

 $ ... $ 或者 \\(...\\) 中的数学表达式将会在行内显示。
$f(x)=sin(x)+9$
\(f(x)=sin(x)+9\)

```
  $f(x)=sin(x)+9$
  \(f(x)=sin(x)+9\)
```

\$\$...\$\$ 或者 \\[...\\] 或者 ```math 中的数学表达式将会在块内显示

$$
\begin{Bmatrix}
   a & b \\
   c & d
\end{Bmatrix}
$$

$$
\begin{CD}
   A @>a>> B \\
@VbVV @AAcA \\
   C @= D
\end{CD}
$$
