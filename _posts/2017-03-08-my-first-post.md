---
title: "关于markdown #的测试"
---


# 我的第一个markdown
严格说之前用过，但并没有仔细研究，
这次自己建立git blog正好写下学习过程，
可能有人回说直接看文档学习就可以了，
但我记性不是那么好，还是自己写一边，并记录下来靠谱。
## “#” 的测试

<p>
#标示加大加粗 一个#为最大，以此类推，下为测试代码
</p>

```markdown
# title
# 标题
## category
## 种类
### tab
### 标签
#### child tab
##### 子标签
```

实际效果如下：

# title
# 标题
## category
## 种类
### tab
### 标签
#### child tab
##### 子标签

<p>
可以发现，“#”与“##”结束将会有一个分割线，而“###”及其以下就没有。
那么却真如我所猜想的一样，是紧跟在“#”及“##”修饰的内容后么？马上来试验一下。
</p>

```markdown
# title
title content
#### 标题 //这里与为了看出行间距问题，所以与上面的title差了较多字号
#### category
##### category 2
###### tab
###### 标签
####### child tab
```
效果如下：
# title
title content
#### 标题
#### category
##### category 2
###### tab
###### 标签
####### child tab
<p>
邓爷爷说过，实践是检验真理的唯一标准，果然如我们当初所猜想的。
而且还可以发现 所有由"#"类符号修饰的文本都会与之前的内容有一个行间距，
并且这个行间距与现所修饰字体的高度相同。数量不同也带来的不同的变化。
</p>

### 总结：“#”类修饰

##### 功能：
>(1)为其后修饰的文本 加大 加粗 加黑（萨满嗜血起～）
>>使用数量大于等于七个的时候无法识别（识别为普通文本）

>> 字号加大 根据其数量 使用一个 “#” 为最大号，
四个为最小号（比正文文本大一号）
四五六个字号相同

>>使用其修饰的所有文本字体均会加粗

>>使用数量小于等于五个的时候文本会为黑色，使用六个的时候文本为灰色。

>(2)与之前内容保持一个当前字符高度的行间距

>(3)当使用数量小于等于两个时，默认会在其修饰文本文本结束的下一行绘制分割线。

---