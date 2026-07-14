# Memory

这个文件保存 `D:\WSLlib\Documents` 工作区内的全局要求。以后处理本工作区内的项目文件前，先读取并遵守本文件。

## Global Requirements

- 文件夹名字全部使用英文。
- 内容中文为主；必要时使用英文原文、标准术语或中英文并列，方便检索和保持数学精确性。
- LaTeX 公式格式：
  - 行内公式使用 `$...$`。
  - 行间公式使用 `$$...$$`。
  - 不使用反斜杠圆括号或反斜杠方括号作为公式分隔符。

## Reading Papers / QWiki

- 论文阅读主页目录为 `D:\WSLlib\Documents\Reading papers`。
- 论文文件夹命名格式为 `English Title - Authors - YYYY-MM-DD`。
- 论文解读默认放在对应论文文件夹的 `解读.md`。
- 作者档案放在 `Reading papers/Files/Authors/`。
- 论文解读文档和作者档案之间使用相对 Markdown 链接互相引用。
- 每次新增、删除或调整 QWiki 论文条目时，同步扫描全部论文卡片作者，更新 `Reading papers/Files/Authors/_index.md`、缺失作者档案和 `index.html` 作者导航；缺失身份信息先标记“待核验”，不要猜测机构、导师或学术历史。
- 每个 `解读.md` 末尾加入“互动创作讨论”区块：包含一个复制提示词并尝试打开 Codex Documents 项目新聊天的按钮，同时保留可手动复制的提示词文本。
- “互动创作讨论”按钮使用 `codex://new` 深链，URL 参数同时传入 `project`、`projectPath`、`cwd`，值均为 `D:/WSLlib/Documents`，并把同一个讨论提示词作为 `prompt` 参数传入。
- QWiki 首页为每篇论文提供阅读状态（未读/正在读/已读）和“学习情况 / 印象”文本框；这些页面交互状态保存在浏览器本地 `localStorage`，键名为 `qwiki.paperState.v1`。
- QWiki 首页顶部保留搜索框和筛选菜单，至少支持按论文分类、阅读状态、标签和文本搜索检索。
- QWiki 首页底部的作者区默认不显示作者详情；应提供 `A-Z` 和“其它”的可见姓氏首字母按钮，以及作者搜索框。点击字母或搜索后直接显示作者按钮，不使用作者下拉选择框；点击某位作者后，再显示“评价”文本框、“主页”链接、“讨论作者”按钮和可切换的星标按钮。右侧栏显示“星标作者”，只列出已星标作者。作者交互状态保存在浏览器本地 `localStorage`，键名为 `qwiki.authorState.v1`。
- QWiki 首页以 `Reading papers` 第一层子文件夹作为论文大类；更深一层子文件夹在所属大类内部显示为可折叠模块。分类筛选选择母文件夹时包含其子模块，选择子模块时只显示该模块。
- QWiki 首页每个论文大类和内部模块均应支持折叠/展开；折叠状态保存在浏览器本地 `localStorage`，键名为 `qwiki.categoryCollapse.v1`。
