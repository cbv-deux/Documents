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
- 第一层子文件夹表示论文大类，例如 `ArxivDaily`；更深一层子文件夹在 QWiki 首页中作为所属大类内部的模块显示。
- 论文文件夹命名格式为 `English Title - Authors - YYYY-MM-DD`。
- 每次阅读论文后，把解读文档放进对应论文文件夹。
- 默认解读文件名为 `解读.md`；如有需要，也可以增加 `摘要.md`、`批注.md`、`问题清单.md`、`复现笔记.md` 等文件。
- `Files/Authors/` 用于保存作者档案，并通过相对 Markdown 链接与论文解读互相引用。
- 每次新增、删除或调整 QWiki 论文条目时，同步扫描全部论文卡片作者，更新 `Files/Authors/_index.md`、缺失作者档案和 `index.html` 作者导航；缺失身份信息先标记“待核验”，不要猜测机构、导师或学术历史。
- `Files/Sources/` 用于保存本地核验证据，例如 arXiv 源文件。
- 正文内容中文为主，必要术语中英文并列。
- LaTeX 公式行内使用 `$...$`，行间使用 `$$...$$`；不要使用反斜杠圆括号或反斜杠方括号作为公式分隔符。
- 每个 `解读.md` 末尾保留“互动创作讨论”区块，用于复制提示词并通过 `codex://new` 尝试打开 Codex 的 Documents 项目新聊天，继续讨论可视化、交互工具或 QWiki 页面增强。
- `index.html` 顶部保留搜索框和筛选菜单，支持按论文分类、阅读状态、标签和文本搜索检索。
- `index.html` 中每篇论文的阅读状态和“学习情况 / 印象”保存在浏览器本地 `localStorage`，键名为 `qwiki.paperState.v1`。
- `index.html` 底部作者区默认不显示作者详情；通过 `A-Z` 和“其它”的可见姓氏首字母按钮，或作者搜索框直接显示作者按钮，不使用作者下拉选择框。点击作者后显示“评价”文本框、“主页”链接、“讨论作者”按钮和可切换星标按钮；右侧栏显示“星标作者”，只列出已星标作者。作者交互状态保存在浏览器本地 `localStorage`，键名为 `qwiki.authorState.v1`。
- `index.html` 中每个论文大类和内部模块都支持折叠/展开；分类筛选选择母文件夹时包含其子模块，选择子模块时只显示该模块。折叠状态保存在浏览器本地 `localStorage`，键名为 `qwiki.categoryCollapse.v1`。

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
