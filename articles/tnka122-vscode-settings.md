---
title: "個人的VSCodeの設定"
emoji: "📘"
type: "idea" # tech: 技術記事 / idea: アイデア
topics: [VSCode, テーマ, フォント, 拡張機能]
published: true
published_at: 2023-12-31 20:00
---

備忘録も兼ねてVSCodeの設定を書きました。  
主に使っていて良かったカラーテーマやフォント、拡張機能を載せています。

他に良さそうなものがあれば追記します。

（以下のコード例は全て[Next.jsのテンプレート](https://github.com/vercel/next.js/blob/canary/packages/create-next-app/templates/app/ts/app/layout.tsx)です）

# テーマ

全てダーク系です

## Everforest Dark

![Everforest Dark](/images/tnka122-vscode-settings/themes/everforest_dark.png)

https://marketplace.visualstudio.com/items?itemName=sainnhe.everforest

現在使用中。

追加で以下のような設定によってパネル間に線を引いています。

```json
"workbench.colorCustomizations": {
    "contrastBorder": "#77777777",
    "panel.border": "#77777777",
}
```

## Gruvbox Material Dark

![Gruvbox Material Dark](/images/tnka122-vscode-settings/themes/gruvbox_material_dark.png)

https://marketplace.visualstudio.com/items?itemName=sainnhe.gruvbox-material

## Nord

![Nord](/images/tnka122-vscode-settings/themes/nord.png)

https://marketplace.visualstudio.com/items?itemName=arcticicestudio.nord-visual-studio-code

## Catppuccin Frappé

![Catppuccin Frappé](/images/tnka122-vscode-settings/themes/catppuccin_frappe.png)

https://marketplace.visualstudio.com/items?itemName=Catppuccin.catppuccin-vsc

# フォント

## Monaspace Radon + Zen Maru Gothic Medium

![Monaspace Radon](/images/tnka122-vscode-settings/fonts/monaspace_radon.png)

https://github.com/githubnext/monaspace

現在使用中。

GitHubが出しているフォント。  
単語に応じて単語内の文字幅を少しだけ変更するテクスチャヒーリング機能搭載。リガチャにも対応しており、特定の文字のみリガチャするといった取捨選択もできます。  
Radonは手書き風フォントなので少し特殊ですが、もちろん通常の書体もあります。Radon含め全5種類。

日本語には非対応。  
自分は日本語フォントとしてZen Maru Gothicを利用しています。  
Mediumと指定することで文字の太さがMonaspaceに近くなります。

## 0xProto

![0xProto](/images/tnka122-vscode-settings/fonts/0xProto.png)

https://github.com/0xType/0xProto

以下のように控え目なリガチャをしてくれるフォント。  

![0xProto ligature](https://github.com/0xType/0xProto/blob/b926d11143f08956e299dc9dfef856620e9e0f6d/images/all_ligatures.png?raw=true)
*0xProtoのGitHubページより引用*

日本語非対応。  
[v1.500](https://github.com/0xType/0xProto/releases/tag/1.500)からテクスチャヒーリングに対応したようです。（スクショはテクスチャヒーリングoffの状態）

## UDEV Gothic 35

![UDEV Gothic 35](/images/tnka122-vscode-settings/fonts/udev_gothic_35.png)

https://github.com/yuru7/udev-gothic

日本語対応フォント。  
リガチャ対応版やNerdFonts対応版など様々なスタイルが用意されています。

また、このフォントの制作者の方が作成している[HackGen](https://github.com/yuru7/HackGen)や[PlemolJP](https://github.com/yuru7/PlemolJP)などのフォントもオススメです。

# 拡張機能

## VSCode Neovim

https://marketplace.visualstudio.com/items?itemName=asvetliakov.vscode-neovim

VSCode上でvimのキーバインドが使えます。

ctrl-c (cmd-c) でinsertモードを抜けるデフォルトの設定だけ消しています。

## Git Graph

https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph

gitの履歴を見るのに便利です。

## GitHub Markdown Preview

https://marketplace.visualstudio.com/items?itemName=bierner.github-markdown-preview

VSCode上のmarkdownプレビューがGitHub上のものの見た目と近くなります。

## GistPad

https://marketplace.visualstudio.com/items?itemName=vsls-contrib.gistfs

VSCode上のどのワークスペースからでもGitHub Gistに書き込めるようになります。  
GitHub Gist利用者にはオススメ。

## Todo Tree

https://marketplace.visualstudio.com/items?itemName=Gruntfuggly.todo-tree

`TODO`、`FIXME`コメントが探しやすくなります。

## Trailing Spaces

https://marketplace.visualstudio.com/items?itemName=shardulm94.trailing-spaces

末尾の空白の視認性が上がります。
