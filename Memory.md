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
- 每个 `解读.md` 末尾加入“互动创作讨论”区块：包含一个复制提示词并尝试打开 Codex Documents 项目新聊天的按钮，同时保留可手动复制的提示词文本。
- “互动创作讨论”按钮使用 `codex://new` 深链，URL 参数同时传入 `project`、`projectPath`、`cwd`，值均为 `D:/WSLlib/Documents`，并把同一个讨论提示词作为 `prompt` 参数传入。
