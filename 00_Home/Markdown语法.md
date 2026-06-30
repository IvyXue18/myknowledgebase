可以。我按 **Mac 快捷键优先**写；Windows/Linux 通常把 `⌘` 换成 `Ctrl`。另外，Obsidian 里的快捷键都可以在 **设置 → 快捷键 Hotkeys** 里搜命令改掉。

Obsidian 支持 CommonMark、GitHub Flavored Markdown、LaTeX，并额外支持 Wikilink、嵌入、Callout、高亮等语法。参考官方文档：[Basic syntax](https://obsidian.md/help/syntax)、[Advanced syntax](https://obsidian.md/help/advanced-syntax)、[Obsidian Flavored Markdown](https://obsidian.md/help/obsidian-flavored-markdown)、[Hotkeys](https://obsidian.md/help/hotkeys)。

## 最常用格式

| 用途      | Markdown 写法 | 快捷键              |
| ------- | ----------- | ---------------- |
| 加粗      | `**文字**`    | `⌘B` / `Ctrl+B`  |
| 斜体      | `*文字*`      | `⌘I` / `Ctrl+I`  |
| 加粗 + 斜体 | `***文字***`  | 可分别按加粗、斜体        |
| 高亮      | `==文字==`    | 默认通常没有固定快捷键，可自定义 |
| 删除线     | `~~文字~~`    | 默认通常没有固定快捷键，可自定义 |
| 行内代码    | `` `代码` ``  | 默认通常没有固定快捷键      |
| 代码块     | ```<br>```  | 默认通常没有固定快捷键      |

---
**加粗**
*斜体*
***加粗 + 斜体***
==高亮==
~~删除线~~
```
这是一段代码
```



## 标题

```
# 一级标题
## 二级标题
### 三级标题
#### 四级标题
##### 五级标题
###### 六级标题
```

标题没有特别必要记快捷键，直接打 `#` 最快。

## 列表

```
- 无序列表
- 另一项

1. 有序列表
2. 另一项

- [ ] 未完成任务
- [x] 已完成任务
- [/] 进行中
```

---
- 无序列表
- 2

1. 有序列表
2. 2

- [ ] 待办任务
- [x] 已完成
- [/] 进行中


## 链接和 Obsidian 双链

```
[[笔记名]]
[网页链接](https://example.com)
```

---
[[AI产品出海实践流程]]
[Mediaclaw](https://mediaclaw.app)

实用输入方式：

| 动作         | 用法 / 快捷键                  |
| ---------- | ------------------------- |
| 插入内部链接     | 直接输入 `[[`，Obsidian 会自动提示  |
| 打开链接预览     | 编辑模式下按住 `⌘` / `Ctrl` 悬停链接 |

## 嵌入内容

```
![[另一篇笔记]]
![[图片.png]]
![[图片.png|300]]
![[文档.pdf]]
![[文档.pdf#page=3]]
![[笔记名#某个标题]]
![[笔记名#^某个块ID]]
```

`!` 的意思是“嵌入显示”，不加 `!` 就只是普通链接。

---
![[状态书影音地图.base]]



## 引用和 Callout

普通引用：

```
> 这是一段引用
```

>这是一段引用

Obsidian Callout：

```
> [!note] 标题
> 内容
```

常用类型：

```
> [!note]
> [!info]
> [!tip]
> [!warning]
> [!danger]
> [!question]
> [!todo]
> [!example]
> [!quote]
```

> [!note] note

> [!info] info

> [!tip] tip

> [!warning] warning

> [!danger] danger

> [!question] qustion

> [!todo] todo

> [!example] example

> [!quote] quote

```
> [!tip]- 默认折叠
> 内容

> [!tip]+ 默认展开
> 内容
```

> [!tip]- 默认折叠
> 这里面有内容哦

>[!tip]+ 默认展开
>我在这


## 表格

```
| 名称 | 状态 | 备注 |
| --- | --- | --- |
| A | 完成 | 可以 |
| B | 待办 | 继续 |
```

| 名称 | 状态 | 备注 |
| --- | --- | --- |
| A | 完成 | 可以 |
| B | 待办 | 继续 |

对齐：

```
| 左对齐 | 居中 | 右对齐 |
| :-- | :--: | --: |
| A | B | C |
```

| 左对齐 | 居中 | 右对齐 |
| :-- | :--: | --: |
| A | B | C |


**标签和属性**

正文标签：

```
#阅读
#项目/进行中
#todo_today
```

属性区，也就是笔记最上面的 YAML：

```
---
tags:
  - 阅读
  - 项目/进行中
aliases:
  - 别名1
status: draft
---
```
