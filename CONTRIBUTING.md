# 贡献指南

🎉 感谢您关注并有兴趣为本项目做出贡献！

我们是一个开放、友好、互助的社区，致力于创建高质量的文档。我们相信，最好的文档是由社区共同创造的。您的每一份贡献，无论大小——从修正一个拼写错误，到撰写一个完整的章节——都对我们至关重要。

本指南将引导您顺利地参与到项目中来。

## 您能做些什么？

作为一份文档，我们欢迎所有能提升其质量和可读性的贡献，包括但不限于：

*   **✍️ 修正错误**：修正拼写、语法或标点错误。
*   **🔍 发现过时内容**：如果您发现某些信息已不再准确，请告诉我们。
*   **💡 提出内容建议**：有任何关于新主题、新章节或改进现有内容的想法，欢迎创建 [Issue](https://github.com/zeronx798/go-arcade-ustb/issues) 来和我们探讨。
*   **📝 完善内容**：补充缺失的细节、增加更清晰的示例、优化语句使其更易理解。
*   **🌐 翻译文档**：帮助我们将文档翻译成其他语言。
*   **💬 参与讨论**：在 [Issues](https://github.com/zeronx798/go-arcade-ustb/issues) 中帮助回答他人的问题，或对改进建议发表您的看法。

如果您是新手，可以从带有 `good first issue` 或 `help wanted` 标签的 Issue 开始，这些通常是比较简单、适合上手的任务。

## 贡献流程

我们遵循标准的 GitHub Fork & Pull Request 流程。即使您不熟悉 Git，也请不要担心，这是一个很棒的学习机会！

1.  **Fork 本项目**
    点击项目主页右上角的 "Fork" 按钮，将项目 Fork 到您自己的 GitHub 账户下。

2.  **Clone 到本地**
    将您 Fork 后的仓库 Clone 到本地计算机。
    ```bash
    git clone https://github.com/your-username/your-repo.git
    cd your-repo
    ```

3.  **创建新分支**
    请务必创建一个新的分支来进行您的修改。一个清晰的分支名能让大家更好地理解您工作的目的。
    ```bash
    # 示例：修复 README 中的拼写错误
    git checkout -b fix/typo-in-readme

    # 示例：增加一个关于“高级用法”的新章节
    git checkout -b docs/add-advanced-usage-guide
    ```

4.  **进行修改并提交**
    在本地进行您的修改。完成后，将您的修改提交到分支上。请遵循下文的 [提交信息规范](#提交信息规范)。
    ```bash
    git add .
    git commit -m "docs: 修正贡献指南中的拼写错误"
    ```

5.  **推送至您的远程仓库**
    将您的本地分支推送到您在 GitHub 上的远程仓库。
    ```bash
    git push origin fix/typo-in-readme
    ```

6.  **创建 Pull Request (PR)**
    进入您 Fork 的 GitHub 仓库页面，点击 "Compare & pull request" 按钮。
    请在 PR 的描述中清晰地说明：
    *   **您做了什么？** (What did you do?)
    *   **为什么这么做？** (Why did you do it?)
    *   **关联的 Issue（如果有）** (e.g., `Closes #123`)

7.  **评审 (Review)**
    提交 PR 后，项目维护者会评审您的修改。我们可能会提出一些修改建议。这是一个共同学习和提升的过程，请积极参与讨论！

8.  **合并**
    一旦您的 PR 通过评审，我们就会将其合并到主分支中。恭喜您，您已经成功为项目做出了一次贡献！

## 文档与排版规范

为确保文档的一致性、可读性，请遵循以下风格指南。

### 1. Markdown 语法
本项目所有文档均使用 Markdown 编写。如果您对 Markdown 不熟悉，不必担心，它非常简单易学。
*   **我们强烈推荐您阅读 GitHub 官方的 [Markdown 基础写作和格式化语法](https://docs.github.com/zh/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax) 指南，几分钟即可上手。**

### 2. 标点符号
为保证中英文混排时格式的统一，本项目中文文档统一使用**全角标点符号**，英文内容使用一个**半角标点符号**并在标点符号后**紧跟一个半角空格**。

*   **正确示例:**
    *   `你好，世界。`
    *   `This is an open-source project, and your participation is welcome.`
*   **错误示例:**
    *   `Hello,World.` (标点后缺少空格)
    *   `你好,世界.` (中文内容使用了半角标点)

### 3. 中英文混排
在中文和英文单词、数字之间增加一个半角空格，以提高可读性。
例外：若数字的一侧为全角字符（中文字符、中文标点等），该侧可以不添加空格。

*   **正确示例:**
    *   `在处理 GitHub issue 时，请保持礼貌。`
    *   `该项目基于 Markdown 构建。`
    *   `乘坐15号线到达终点。` 或 `乘坐 15 号线到达终点。`
*   **错误示例:**
    *   `在处理GitHub issue时，请保持礼貌。`
    *   `该项目基于Markdown构建。`

### 4. 专有名词
对于广为人知的专有名词，请尽量使用社区公认的通用写法和大小写规范。

*   **推荐**: `JavaScript`, `GitHub`, `Node.js`, `React`
*   **不推荐**: `Javascript`, `github`, `node.js`, `react`

### 5. 提交信息规范 (Commit Message)
我们采用 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/v1.0.0/) 规范来书写提交信息，这有助于我们清晰地追溯每一次修改。格式如下： `type: subject`

**常用 `type` 类型**:
*   `docs`: 新增或修改文档内容
*   `fix`: 修正内容中的事实性错误、链接失效等问题
*   `style`: 修改格式、标点等不影响内容含义的变动
*   `chore`: 项目维护相关的修改（例如更新本贡献指南）

**示例**:
*   `docs: 增加高级用法章节`
*   `fix: 修正 README 中的一个失效链接`
*   `style: 统一全文标点为全角`

---

再次感谢您的时间和贡献！我们期待与您共建一份更出色的文档。