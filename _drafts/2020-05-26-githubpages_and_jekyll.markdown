---
layout: post
title: "GitHub Pages&Jekyllを使ってブログを作成する方法1"
date: 2020-05-26 12:00:00 +0900
description:
img: 2020-05-26_1.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [GitHub Pages, Jekyll]
---

今回、初めてGitHub PagesとJekyllを使ってブログを作成してみました。

結論...

__早い__

__楽__

ということで

### 今回はGitHub PagesとJekyllを使って、簡単にブログを作成する方法をご紹介します。

***

# GitHub Pagesとは

_参考_  
[GitHub Pages公式ドキュメント](https://help.github.com/ja/github/working-with-github-pages)

## GitHub Pagesの良い点

1. 無料で"github.io"ドメインを利用することができる。
1. Markdown（マークダウン）記法を使って、記事を書くことができる。
1. GitHubにpushするだけで記事を更新することができる。
1. Jekyllを使えば、HTMLやCSSの知識が無くても作れるので敷居が低い。

## GitHub Pagesの運用方法

__前提__  
* GitHubのアカウントを持っていること

GitHubのアカウントを持っていない方は、以下を参考にアカウントを作成してください。

_参考_  
[GitHubアカウント作成とリポジトリの作成手順](https://qiita.com/kooohei/items/361da3c9dbb6e0c7946b)

#### GitHubにログインさえできれば、後はリポジトリを作成してリモートにpushするだけ

__手順__  
* リポジトリの作成  
    _参考_  
    [GitHubアカウント作成とリポジトリの作成手順](https://qiita.com/kooohei/items/361da3c9dbb6e0c7946b)  
* ローカルリポジトリを用意する
    名前はなんでも良いです。
* リモートリポジトリにpushする  
<p style="padding: 5px;border: 2px solid gray;background: whitesmoke;">
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">cd&nbsp;[ローカルリポジトリのパス]</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">git&nbsp;init</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">echo&nbsp;HelloWorld&nbsp;>>&nbsp;index.html</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">git&nbsp;add&nbsp;.</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">git&nbsp;commit&nbsp;-m&nbsp;"first commit"</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">git&nbsp;remote&nbsp;add&nbsp;origin&nbsp;https://github.com/[GitHubのユーザ名]/[リポジトリ名].git</span>
<br>
<span style="color: green">$</span>&nbsp;&nbsp;&nbsp;<span style="color: red">git&nbsp;push&nbsp;-u&nbsp;origin&nbsp;master</span>
</p>

* ブラウザからアクセス  
<p style="padding: 5px;border: 2px solid gray;background: whitesmoke;">
<span style="color: black">https://[GitHubのユーザ名].github.io</span></p>  
するとHelloWorldと書かれたWebページが表示されるはずです。

***


#### 次回はJekyllを使った様々なテーマの適用方法を紹介します。








