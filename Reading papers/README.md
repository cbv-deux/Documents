# Reading papers

这个文件夹用于保存论文阅读、解读材料和作者档案。

## 目录结构

```text
Reading papers/
  index.html
  ArxivDaily/
    English Title - Authors - YYYY-MM-DD/
      解读.md
  Files/
    Authors/
      Author-Name.md
    Sources/
      arxiv-eprints/
```

## 使用约定

- 文件夹名字全部使用英文。
- 第一层子文件夹表示分类，例如 `ArxivDaily`。
- 论文文件夹命名格式为 `English Title - Authors - YYYY-MM-DD`。
- 每次阅读论文后，把解读文档放进对应论文文件夹。
- 默认解读文件名为 `解读.md`；如有需要，也可以增加 `摘要.md`、`批注.md`、`问题清单.md`、`复现笔记.md` 等文件。
- `Files/Authors/` 用于保存作者档案，并通过相对 Markdown 链接与论文解读互相引用。
- `Files/Sources/` 用于保存本地核验证据，例如 arXiv 源文件。
- 正文内容中文为主，必要术语中英文并列。
- LaTeX 公式行内使用 `$...$`，行间使用 `$$...$$`；不要使用反斜杠圆括号或反斜杠方括号作为公式分隔符。
- 每个 `解读.md` 末尾保留“互动创作讨论”区块，用于复制提示词并尝试打开 Codex 的 Documents 项目新聊天，继续讨论可视化、交互工具或 QWiki 页面增强。

## 默认解读模板

```markdown
# English Title

## 基本信息

- 作者：
- 年份：
- 来源：
- 链接或文件：

## 一句话概括

## 核心问题

## 主要贡献

## 方法与思路

## 关键定义与概念

## 重要结论

## 证明或实验结构

## 我的理解

## 疑问与后续阅读
```
