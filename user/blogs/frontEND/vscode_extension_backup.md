---
title: vscode extension backup
description: Example post written using Markdown Syntax with QWER - Simply Awesome Blog Starter. Built using SvelteKit and Love.
summary: 📝 Showcase basic syntax of Markdown and HTML
published: '2024-09-06T03:48:17.421058+08:00'
updated: '2024-09-06T03:48:17.421058+08:00'
# cover: ./cover.jpg
coverCaption: Photo by <a href="https://unsplash.com/@etiennegirardet?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Etienne Girardet</a> on <a href="https://unsplash.com/s/photos/motivation?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>
language: cht
tags:
  - [vscode]

---

要將你在 Visual Studio Code (VSCode) 已安裝的 extensions 輸出成 TXT 檔案，並在另一台裝置上安裝，你可以按照以下步驟進行：

### 步驟 1: 將已安裝的 extensions 輸出成 TXT 檔案
1. 打開 VSCode。
2. 打開終端機（**Terminal**），可以使用快捷鍵 `Ctrl + `（反引號）。
3. 輸入以下指令，將已安裝的 extensions 列表輸出到一個 `extensions-list.txt` 檔案中：

   ```bash
   code --list-extensions > extensions-list.txt
   ```

4. 在你的工作目錄下，會生成一個 `extensions-list.txt` 檔案，裡面列出所有已安裝的 extensions。

### 步驟 2: 在另一台裝置上安裝 extensions
1. 把 `extensions-list.txt` 檔案複製到另一台裝置。
2. 打開另一台裝置的 VSCode 終端機，並執行以下指令，根據 `extensions-list.txt` 中的列表安裝所有 extensions：

   ```bash
   cat extensions-list.txt | xargs -n 1 code --install-extension
   ```

這樣就可以批量安裝所有的 extensions 了！
