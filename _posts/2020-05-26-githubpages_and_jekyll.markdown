---
layout: post
title: "GitHub Pagesを使ってブログを作成する方法"
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
    この時のリポジトリ名はブログのURLの一部になります  
    [GitHubのアカウント名].github.io/[リポジトリ名]
* ローカルリポジトリを用意する  
    リポジトリ名  
    <p class="box">
    <span class="span-black">[GitHubのユーザ名].github.io</span></p>
* リモートリポジトリにpushする  
    <p class="box">
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">cd&nbsp;[ローカルリポジトリのパス]</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">git&nbsp;init</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">echo&nbsp;HelloWorld&nbsp;>>&nbsp;index.html</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">git&nbsp;add&nbsp;.</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">git&nbsp;commit&nbsp;-m&nbsp;"first commit"</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">git&nbsp;remote&nbsp;add&nbsp;origin&nbsp;https://github.com/[GitHubのユーザ名]/[リポジトリ名].git</span>
    <br>
    <span class="span-green">$</span>&nbsp;&nbsp;&nbsp;<span class="span-red">git&nbsp;push&nbsp;-u&nbsp;origin&nbsp;master</span>
    </p>

* ブラウザからアクセス  
    <p class="box">
    <span class="span-black">https://[GitHubのユーザ名].github.io/</span></p>  
    するとHelloWorldと書かれたWebページが表示されるはずです。

***


#### Jekyllを使ってThemeを適用する方法
参考  
[GitHub PagesにJekyllを使っていい感じのページを作る例](https://qiita.com/stkdev/items/0e2df27736acbea9bd26)

***








