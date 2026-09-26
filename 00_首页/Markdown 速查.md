# Markdown 速查

Obsidian 支持 CommonMark、GitHub Flavored Markdown、LaTeX，并额外支持 Wikilink、嵌入、Callout、高亮等语法。快捷键可以在 **设置 → 快捷键 Hotkeys** 里搜索命令修改。

### 最常用格式

| 用途 | Markdown 写法 | 快捷键 |
| --- | --- | --- |
| 加粗 | `**文字**` | `⌘B` / `Ctrl+B` |
| 斜体 | `*文字*` | `⌘I` / `Ctrl+I` |
| 加粗 + 斜体 | `***文字***` | 可分别按加粗、斜体 |
| 高亮 | `==文字==` | 默认通常没有固定快捷键，可自定义 |
| 删除线 | `~~文字~~` | 默认通常没有固定快捷键，可自定义 |
| 行内代码 | `` `代码` `` | 默认通常没有固定快捷键 |
| 代码块 | 三个反引号包裹 | 默认通常没有固定快捷键 |
**加粗**
*斜体*
***加粗+斜体***
==高亮==
~~删除~~
`行内代码`
```
代码块
```


### 标题、列表、任务

```markdown
# 一级标题
## 二级标题
### 三级标题

- 无序列表
- 另一项

1. 有序列表
2. 另一项

- [ ] 未完成任务
- [x] 已完成任务
- [/] 进行中
```

- [ ] 待办
- [/] ing
- [x] done 


### 链接和嵌入

```markdown
[[笔记名]]
[网页链接](https://example.com)

![[另一篇笔记]]
![[图片.png]]
![[图片.png|300]]
![[文档.pdf#page=3]]
![[笔记名#某个标题]]
![[笔记名#^某个块ID]]
```
*`!` 的意思是“嵌入显示”，不加 `!` 就只是普通链接。*

[[#快速入口]] 链接到本文档其他小节
[[AI产品出海实践 SOP]] 链接到其他文件
[Mediaclaw](https://mediaclaw.app)

### 引用和 Callout

```markdown
> 这是一段引用

> [!note] 标题
> 内容

> [!tip]- 默认折叠
> 内容

> [!tip]+ 默认展开
> 内容
```

>这是一段引用

> [!note] note

> [!info] info

> [!tip] tip

> [!waring] waring

> [!danger] danger

> [!question] question

> [!todo] todo

> [!example] example

>[!quote] quote

> [!tip]+ 默认展开
> 这有一句话

> [!tip]- 默认折叠
> 这有一句话


常用类型：`note`、`info`、`tip`、`warning`、`danger`、`question`、`todo`、`example`、`quote`。

### 表格

```markdown
| 名称 | 状态 | 备注 |
| --- | --- | --- |
| A | 完成 | 可以 |
| B | 待办 | 继续 |

| 左对齐 | 居中 | 右对齐 |
| :-- | :--: | --: |
| A | B | C |
```

| 名称 | 状态 | 备注 |
| --- | --- | --- |
| A | 完成 | 可以 |
| B | 待办 | 继续 |

| 左对齐 | 居中 | 右对齐 |
| :-- | :--: | --: |
| A | B | C |


### 标签和属性

正文标签：

```markdown
#阅读
#项目/进行中
#todo_today
```

属性区，也就是笔记最上面的 YAML：

```yaml
---
tags:
  - 阅读
  - 项目/进行中
aliases:
  - 别名1
status: draft
---
```
