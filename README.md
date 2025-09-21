# BNU Beamerposter & Presentation Theme (Unofficial)

一个基于 [FSU Beamerposter & Presentation Theme (Unofficial)](https://github.com/rispace/unofficial-FSU-beamer-theme-template) 制作的，专为北京师范大学（BNU）定制的非官方 **Beamerposter** 和 **演示文稿** 主题。此主题遵循BNU的蓝色与红色配色方案，完美支持**海报**布局和标准的**幻灯片**演示。

**重要提示：** 此主题基于原版的 `FSU` 主题适配修改而来，根据[北京师范大学视觉形象识别系统(2008年版) ](https://xcb.bnu.edu.cn/fwzn/xzzx/index.html)指定色彩提供部分色彩规范。有问题请邮件联系：email(liuziqi1026@outlook.com)

---

## 主要特性

### 海报模式 (Poster Mode)

✅ 优雅的页眉，支持校徽/院徽放置

✅ 标准的 BNU 蓝与红配色方案

✅ 优化的衬线字体，提升阅读体验

✅ 带阴影和圆角的区块设计

✅ 带编号的图表和表格

✅ 支持海报的多栏（如3栏）布局

✅ 可自定义的页脚信息栏

---

### 演示文稿模式 (Presentation Mode)

✅ 现代化的幻灯片页眉，带可点击的圆点导航

✅ 自定义页脚线，包含作者/标题/日期/页码信息

✅ 自动列出章节的目录页

✅ 为屏幕阅读优化的字体样式

✅ 可选的、可点击的幻灯片项目符号链接

✅ 为数学公式提供完整支持 (`amsmath`, `amssymb`, `unicode-math`)

✅ 轻松在海报和演示文稿样式之间切换

---

## 如何编译

本项目使用 **LuaLaTeX** 引擎进行编译，以获得最佳的字体支持和功能。

**推荐编译配方 (Compilation Recipe):**

`lualatex -> bibtex -> lualatex -> lualatex`

### 在 Overleaf 上使用

1.  在 Overleaf 中新建项目，选择 **上传项目**。
3.  将本仓库的所有文件打包为 ZIP 并上传。
5.  在 Overleaf 的项目菜单中，将 **编译器** 设置为 **LuaLaTeX**。
7.  编译主文件 (`poster.tex` 或 `presentation.tex`)。

### 在本地使用

确保你的 TeX 发行版（如 TeX Live 或 MiKTeX）已更新并包含所有必要包。使用支持 LuaLaTeX 的编辑器（如 TeXworks, TeXstudio, VS Code with LaTeX Workshop），将编译引擎设置为 **LuaLaTeX**，并运行上述编译流程。

---

## 包含的文件

- `beamerthemebnu.sty` – 主题结构和布局定义
- `beamercolorthemebnucolor.sty` – BNU 配色方案定义
- `presentation.tex` – 演示文稿示例文件
- `poster.tex` – 海报示例文件
- `logo/` – 存放徽标（请替换为您自己的徽标文件）
- `images/` – 示例图片
- `ref.bib` – 示例参考文献文件
- `README.md` – 说明文件

---

## 使用方法

1.  **选择模式:** 在主文件（如 `presentation.tex`）中，通过向主题和颜色主题传递 `presentation` 选项来启用演示文稿模式。
    ```latex
    \usetheme[presentation]{bnu}
    \usecolortheme[presentation]{bnucolor}
    ```
    移除选项即可使用海报模式。

2.  **填写信息:** 修改 `\title`, `\author`, `\institute`, `\date` 等信息。
3.  **添加徽标:** 使用 `\logoleft{}` 和 `\logoright{}` 命令（海报模式）或 `\presentationlogo{}` 命令（演示文稿模式）来插入徽标。
4.  **编写内容:** 在 `frame` 环境中使用 `block`, `alertblock`, `exampleblock` 等环境组织内容。
5.  **编译:** 按照上述编译说明进行操作。

---

## 致谢与来源

此主题改编自 Rafiq Islam 为佛罗里达州立大学 (FSU) 设计的优秀模板：[FSU Beamerposter & Presentation Theme (Unofficial)](https://github.com/rispace/unofficial-FSU-beamer-theme-template)。我们在此表示感谢。

---

## 作者

**Liu Ziqi (刘子旗)**
Beijing Normal University

GitHub: [xier-1026](https://github.com/xier-1026)

---

## 许可证

此项目在原 FSU 模板的许可证下发行。请参考原仓库的许可证信息。
