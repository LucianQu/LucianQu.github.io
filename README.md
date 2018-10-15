QuLusheng

<p>行内式 <a href="https://lucianqu.github.io/" title="我的个人博客">博客</a> 链接，带 title。</p>

<p>行内式 <a href="https://github.com/LucianQu">GitHub</a> 链接。</p>

# Automic

## Android

###### 水利

Setext-style 一级标题
===

二级标题
---
预览效果：

atx-style 一级标题
二级标题
六级标题
Setext-style 一级标题
二级标题
对应 HTML：

<h1>atx-style 一级标题</h1>

<h2>二级标题</h2>

<h6>六级标题</h6>

<h1>Setext-style 一级标题</h1>

<h2>二级标题</h2>
段落
中间没有空行的连续不断的几行文字被视为一个段落。

Markdown：

白日依山尽，

黄河入海流。
（句号后面没空格）

欲穷千里目，

更上一层楼。  
（句号后面有俩空格）
预览效果：

白日依山尽，

黄河入海流。 （句号后面没空格）

欲穷千里目，

更上一层楼。
（句号后面有俩空格）

对应 HTML：

<p>白日依山尽，</p>

<p>黄河入海流。
（句号后面没有空格）</p>

<p>欲穷千里目，</p>

<p>
  更上一层楼。
  <br>
  （句号后面有俩空格）
</p>
行内格式
对段落或者部分文本的强调效果。

Markdown：

后面俩字**加黑**

后面俩字*斜体*
预览效果：

后面俩字加黑

后面俩字斜体

对应 HTML：

<p>
  后面俩字
  <strong>加黑</strong>
</p>
<p>
  后面俩字
  <em>斜体</em>
</p>
引用块
Markdown：

> 引用块段落一。
>
> 引用块段落二。
>> 内嵌引用块段落一。
>
> ### 引用块内的标题
预览效果：

引用块段落一。

引用块段落二。

内嵌引用块段落一。

引用块内的标题
对应 HTML：

<blockquote>
  <p>引用块段落一。</p>
  <p>引用块段落二。</p>
  <blockquote>
    <p>内嵌引用块段落一。</p>
  </blockquote>
  <h3 id="引用块内的标题">引用块内的标题</h3>
</blockquote>
超链接
Markdown 支持行内式链接和引用式链接。

Markdown：

行内式 [博客](https://lucianqu.github.io/ "我的个人博客") 链接，带 title。

行内式 [GitHub](https://github.com/LucianQu) 链接。

引用式 [博客][1] 链接。

引用式 [GitHub][2] 链接，带 title。

[1]: https://lucianqu.github.io/
[2]: https://github.com/LucianQu "我的 GitHub 主页"
预览效果：

行内式 博客 链接，带 title。

行内式 GitHub 链接。

引用式 博客 链接。

引用式 GitHub 链接，带 title。

对应 HTML：

<p>行内式 <a href="https://lucianqu.github.io/" title="我的个人博客">博客</a> 链接，带 title。</p>

<p>行内式 <a href="https://github.com/LucianQu">GitHub</a> 链接。</p>

<p>引用式 <a href="https://lucianqu.github.io/">博客</a> 链接。</p>

<p>引用式 <a href="https://github.com/LucianQu" title="我的 GitHub 主页">GitHub</a> 链接，带 title。</p>
图片
在超链接的写法前加一个 !，就是引用图片的方法。

Markdown：

![Alt text](https://github.com/LucianQu "favicon")
预览效果：

Alt text

对应 HTML：

<img src="https://github.com/LucianQu" alt="Alt text" title="favicon">
列表
包括有序列表和无序列表。

Markdown：

- 苹果
- 葡萄
- 榴莲

1. 苹果
2. 葡萄
3. 榴莲
预览效果：

苹果
葡萄
榴莲
苹果
葡萄
榴莲
对应 HTML：

<ul>
  <li>苹果</li>
  <li>葡萄</li>
  <li>榴莲</li>
</ul>
<ol>
  <li>苹果</li>
  <li>葡萄</li>
  <li>榴莲</li>
</ol>
其中无序列表的标记可以使用 +、- 或 *，有序列表前的数字可以是乱序的。

代码块
支持行内代码和代码块。

Markdown：

Android 里使用 `TextUtils` 类的 `isEmpty` 方法来判断字符串是否为空。

```java
if (TextUtils.isEmpty(text)) {
    return null;
}
```
预览效果：

Android 里使用 TextUtils 类的 isEmpty 方法来判断字符串是否为空。

if (TextUtils.isEmpty(text)) {
    return null;
}
对应 HTML：

<p>Android 里使用 <code>TextUtils</code> 类的 <code>isEmpty</code> 方法来判断字符串是否为空。</p>

<div class="highlight highlight-source-java"><pre><span class="pl-k">if</span> (<span class="pl-smi">TextUtils</span><span class="pl-k">.</span>isEmpty(text)) {
    <span class="pl-k">return</span> <span class="pl-c1">null</span>;
}</pre></div>
上例中的语言标记 java 可选填，可用于在编辑器和渲染后的效果里添加语法高亮。

块式代码也可以对整个代码段缩进四个空格，或一个 Tab 来实现。

水平分割线
使用一个单独行里的三个或以上 *、- 来生产一条水平分割线，它们之间可以有空格。

Markdown：

***

-----

- - -
预览效果：

对应 HTML：

<hr />

<hr />

<hr />
嵌入 HTML
Markdown 标记语言的目的不是替代 HTML，也不是发明一种更便捷的插入 HTML 标签的方式。它对应的只是 HTML 标签的一个很小的子集。

对于那些没有办法用 Markdown 语法来对应的 HTML 标签，直接使用 HTML 来写就好了。

扩展语法
本节的内容是介绍一些受到广泛支持的 Markdown 扩展语法。

表格
Markdown：

| 编号  | 姓名（左） | 年龄（右） | 性别（中） |
| ----- | :--------  | ---------: | :------:   |
| 0     | 张三       | 28         | 男         |
| 1     | 李四       | 29         | 男         |
预览效果：

编号	姓名（左）	年龄（右）	性别（中）
0	张三	28	男
1	李四	29	男
对应 HTML：

<table>
  <thead>
    <tr>
      <th>编号</th>
      <th align="left">姓名（左）</th>
      <th align="right">年龄（右）</th>
      <th align="center">性别（中）</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>0</td>
      <td align="left">张三</td>
      <td align="right">28</td>
      <td align="center">男</td>
    </tr>
    <tr>
      <td>1</td>
      <td align="left">李四</td>
      <td align="right">29</td>
      <td align="center">男</td>
    </tr>
  </tbody>
</table>
任务列表
在 GitHub / GitLab 里有较好的支持。

Markdown：

- [x] 洗碗
- [ ] 清洗油烟机
- [ ] 拖地
预览效果：

 洗碗
 清洗油烟机
 拖地
对应 HTML：

<ul class="contains-task-list">
  <li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox" checked=""> 洗碗</li>
  <li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"> 清洗油烟机</li>
  <li class="task-list-item"><input type="checkbox" id="" disabled="" class="task-list-item-checkbox"> 拖地</li>
</ul>
