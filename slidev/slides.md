---
# try also 'default' to start simple
theme: default
# random image from a curated Unsplash collection by Anthony
# like them? see https://unsplash.com/collections/94734566/slidev
background: https://source.unsplash.com/collection/94734566/1920x1080
# apply any windi css classes to the current slide
class: 'text-center'
# https://sli.dev/custom/highlighters.html
highlighter: shiki
# some information about the slides, markdown enabled
info: |
  ## Slidev Starter Template
  Presentation slides for developers.

  Learn more at [Sli.dev](https://sli.dev)
---

# MkDocs + draw.io + vscode で(技術)ドキュメント作成


<!--
The last comment block of each slide will be treated as slide notes. It will be visible and editable in Presenter Mode along with the slide. [Read more in the docs](https://sli.dev/guide/syntax.html#notes)
-->

---
layout: cover
background: https://source.unsplash.com/collection/94734566/1920x1080
---
# Table of Contens

- 背景
- ツール紹介
  - MkDocs
  - draw.io
  - vscode-drawio.integration
- デモ
- 所感


---

# Excel でドキュメントを作る/見るのは大変
- レイアウトが自由すぎる
- 画面が狭いと閲覧性が悪い
- 閲覧時の操作性に難あり
- 差分が不明/追うのが大変
- ...

<br>
<br>

### できればExcelは避けたい


---

# 快適なドキュメント作成/閲覧環境を求めて

- **シンプルなテキスト**形式が望ましい。好きなエディタを使いたい。
- **図を版管理**したい。が、コードから生成するのは辛い。(PlantUMLなど)。exportめんどくさい。
- 勝手に**いい感じのドキュメント**ができあがってほしい。
- Gitで管理したい。

<br>
<br>

<div grid="~ cols-3 gap-8">
<div>

  vscodeで軽快にMarkdown編集

</div>
<div>

  draw.io (+ vscode) で版管理可能な図をさっと作成

</div>
<div>

  MkDocsでいい感じのドキュメントをえいやと生成

</div>
</div>

<div grid="~ cols-3 gap-8">

  <div>

  <img border="rounded" src="/assets/vscode.png">

  </div>

  <div>

  <img border="rounded" src="/assets/example-screen1.png">

  </div>

  <div>

  <img border="rounded" src="/assets/mkdocs.png">

  </div>

</div>

---
layout: cover
background: https://source.unsplash.com/collection/94734566/1920x1080
---

# ツール紹介
- MkDocs
- draw.io
- vscode-drawio.integration

---

# MkDocs

**Markdown**だけでドキュメントサイトが構築できる**静的サイトジェネレーター**

- 📝 **Text-based** - Markdownファイルを放り込めばOK
- 🎨 **Themable** - いろいろテーマがある（Materialテーマが良さそう）+ 見た目もいじれる
- 👍 **Simple** - 基本は設定ファイル一つだけ
- 🛠 **Extensible** - 拡張Markdownの表現が便利 + プラグインで機能追加

<br>
<br>

<div grid="~ cols-2 gap-8">

<div>
<img border="rounded" src="/assets/mkdocs-material.png">
</div>

<div>
<img border="rounded" src="/assets/mkdocs.png">
</div>

</div>


---

# draw.io

<div grid="~ cols-2 gap-8">

<div>

GUIベースで使える図作成ツール/サービス
- オープンソース
- 登録不要
- ブラウザから手軽に利用できる
- デスクトップアプリもある（オフラインでも使用可）

👍 図形だけでなく、様々なIconがデフォルトで用意されている  

👍 編集可能な形式で保存できる

</div>

<div>

<br>
<br>
<br>
<img src="/assets/drawio.png" border="rounded">

</div>

</div>

---

# [vscode-drawio.integration](https://marketplace.visualstudio.com/items?itemName=hediet.vscode-drawio)

vscode上でdraw.ioが利用できるように (vscodeの拡張機能)

<img border="rounded" src="/assets/example-screen1.png">

---

# Markdown + draw.io (with vscode)
Markdownとdraw.ioの組み合わせがかなり便利です

<div grid="~ cols-2 gap-16">

<div style="text-align: center;">

draw.ioで作成したファイル(svg)を  
Markdownに埋め込み可能
### preview画面に直接画像が表示されます

</div>

<div style="text-align: center;">

直接編集が可能  
(svgなので版管理で差分も見れる)

### vscode内で編集 & 反映

</div>

</div>

<br>

<div grid="~ cols-2 gap-8">

<div>

<img border="rounded" src="/assets/vscode-drawio.png">

</div>

<div>

<img border="rounded" src="/assets/vscode-drawio2.png">

</div>

</div>



---
layout: cover
background: https://source.unsplash.com/collection/94734566/1920x1080
---

# デモ

---
layout: cover
---

<video controls="controls">
  <source src="/assets/mkdocs.mov">
</video>

---

<video controls="controls">
  <source src="/assets/demo.mov">
</video>

---

# 所感

## 😄

- Markdown に図を直接埋め込み & 編集できるのは素晴らしい
- 導入 & 使用へのハードルは低め
- 全部 Git で管理できる
  - 改善の提案、修正、レビューが楽に（on GitHub）
- vscode live share が使えるので、共同編集も可能
- ある程度見やすいドキュメントが作れる

## 😫

- 運用によっては管理が面倒
  - 技術ドキュメントであれば整理することが前提なのでそこまで気にならないかも...?
- ホスティングして使うことが前提
- 表はExcelに負けます

