---
title: "Test"
date: 2022-02-08T00:13:43+09:00
categories:
  - ラーメン班
  - うどん班
tags:
  - scribble
  - test
description: テスト記事
slug: test1
image: https://2.bp.blogspot.com/-n8sq01oQyhQ/Wn1WcCmGgTI/AAAAAAABKKI/-OwhP3j-NhUl6OlmqX_HG5ve-VcqVTcHwCLcBGAs/w1200-h630-p-k-no-nu/yatai_ra-men_man.png
---

# 見出しはh2から
h1はTOCに含まれない

## 日本語文のテスト

Goはプログラミング言語の1つである。2009年、GoogleでRobert Griesemer、ロブ・パイク、ケン・トンプソンによって設計された。Goは、静的型付け、C言語の伝統に則ったコンパイル言語、メモリ安全性、ガベージコレクション、構造的型付け（英語版）、CSPスタイルの並行性などの特徴を持つ。Goのコンパイラ、ツール、およびソースコードは、すべてフリーかつオープンソースである。

また、軽量スレッディングのための機能、Pythonのような動的型付け言語のようなプログラミングの容易性、などの特徴もある。Go処理系としてはコンパイラのみが開発されている。マスコット・キャラクターはGopher（ホリネズミ）。

発表当初はLinuxとMac OS Xのみしかサポートしていなかったが、2012年3月にリリースされたバージョン1.0からはWindowsもサポートされている。2014年12月にリリースされたバージョン1.4からAndroidをサポートし、2015年8月19日にリリースされたバージョン1.5からiOSをサポートしている。また、2011年5月10日に公開された Google App Engine 1.5.0 でも、Go言語がサポートされている。2018年8月にリリースされたバージョン1.11からWebAssemblyをサポートした。

>「そうなのか？お前が欲したのはそれなのか？とすれば、それこそまさしくお前がこれまで一度も経験しなかったことだ（思い出すがいい、お前は言葉で自分自身を騙してきた。お前が冒険と呼んだのは、旅で得た粗悪な模造品であり、街で拾った女たちとの情事であり、殴り合いであり、ガラス細工に過ぎなかった。）。以下略。」 _J.P.Sartre 「嘔吐」 鈴木道彦訳.　人文書院、2010_


## リンクカード
リンクカードの挿入は`{{</* linkcard url="https://example.com/" */>}}`で

{{< linkcard url="https://github.com/microsoft/TypeScript">}}

{{< linkcard url="https://zenn.dev/">}}

{{< linkcard url="https://qiita.com/e869120/items/1b2a5f0f07fd927e44e9">}}

## 意味のないプログラム
```haskell
data Iminai deriving (Show, Ord)
```


```go
package main

import "fmt"

func main() {
  fmt.Printf("Hello World\n")
}
```


## 🐕

これは...何だ？
               🐱🐙🔥 Octocatの塩焼き


## 数式てすと
KaTeX

https://katex.org/docs/supported.html



改行は`\\\\`で

$$
\sin \alpha\\\\
\cos \beta\\\\
\tan{\alpha+\beta}
$$

$$
\begin{aligned}
x &= 1+1 \\\\
&= 2
\end{aligned}
$$

$$
\begin{cases}
y = 3x \\\\
y = x + 6
\end{cases}
$$

$$
\int_{0}^{1} f(x) \ dx
= \lim_{n \to \infty} \dfrac{1}{n} \sum_{k=0}^{n-1} f \left (\dfrac{k}{n} \right)
$$

$$
\begin{pmatrix}
a & b \\\\
c & d
\end{pmatrix}
$$



This article offers a sample of basic Markdown syntax that can be used in Hugo content files, also it shows whether basic HTML elements are decorated with CSS in a Hugo theme.
<!--more-->

## Headings

The following HTML `<h1>`—`<h6>` elements represent six levels of section headings. `<h1>` is the highest section level while `<h6>` is the lowest.

# H1
## H2
### H3
#### H4
##### H5
###### H6

## Paragraph

Xerum, quo qui aut unt expliquam qui dolut labo. Aque venitatiusda cum, voluptionse latur sitiae dolessi aut parist aut dollo enim qui voluptate ma dolestendit peritin re plis aut quas inctum laceat est volestemque commosa as cus endigna tectur, offic to cor sequas etum rerum idem sintibus eiur? Quianimin porecus evelectur, cum que nis nust voloribus ratem aut omnimi, sitatur? Quiatem. Nam, omnis sum am facea corem alique molestrunt et eos evelece arcillit ut aut eos eos nus, sin conecerem erum fuga. Ri oditatquam, ad quibus unda veliamenimin cusam et facea ipsamus es exerum sitate dolores editium rerore eost, temped molorro ratiae volorro te reribus dolorer sperchicium faceata tiustia prat.

Itatur? Quiatae cullecum rem ent aut odis in re eossequodi nonsequ idebis ne sapicia is sinveli squiatum, core et que aut hariosam ex eat.

## Blockquotes

The blockquote element represents content that is quoted from another source, optionally with a citation which must be within a `footer` or `cite` element, and optionally with in-line changes such as annotations and abbreviations.

#### Blockquote without attribution

> Tiam, ad mint andaepu dandae nostion secatur sequo quae.
> **Note** that you can use *Markdown syntax* within a blockquote.
#### Blockquote with attribution

> Don't communicate by sharing memory, share memory by communicating.<br>
> — <cite>Rob Pike[^1]</cite>
[^1]: The above quote is excerpted from Rob Pike's [talk](https://www.youtube.com/watch?v=PAAkCSZUG1c) during Gopherfest, November 18, 2015.

## Tables

Tables aren't part of the core Markdown spec, but Hugo supports supports them out-of-the-box.

   Name | Age
--------|------
    Bob | 27
  Alice | 23

#### Inline Markdown within tables

| Italics   | Bold     | Code   |
| --------  | -------- | ------ |
| *italics* | **bold** | `code` |

| A                                                        | B                                                                                                             | C                                                                                                                                    | D                                                 | E                                                          | F                                                                    |
|----------------------------------------------------------|---------------------------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------------------------------------------|---------------------------------------------------|------------------------------------------------------------|----------------------------------------------------------------------|
| Lorem ipsum dolor sit amet, consectetur adipiscing elit. | Phasellus ultricies, sapien non euismod aliquam, dui ligula tincidunt odio, at accumsan nulla sapien eget ex. | Proin eleifend dictum ipsum, non euismod ipsum pulvinar et. Vivamus sollicitudin, quam in pulvinar aliquam, metus elit pretium purus | Proin sit amet velit nec enim imperdiet vehicula. | Ut bibendum vestibulum quam, eu egestas turpis gravida nec | Sed scelerisque nec turpis vel viverra. Vivamus vitae pretium sapien |

## Code Blocks

#### Code block with backticks

```html
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
```

#### Code block indented with four spaces

    <!doctype html>
    <html lang="en">
    <head>
      <meta charset="utf-8">
      <title>Example HTML5 Document</title>
    </head>
    <body>
      <p>Test</p>
    </body>
    </html>

#### Code block with Hugo's internal highlight shortcode
{{< highlight html >}}
<!doctype html>
<html lang="en">
<head>
  <meta charset="utf-8">
  <title>Example HTML5 Document</title>
</head>
<body>
  <p>Test</p>
</body>
</html>
{{< /highlight >}}

#### Diff code block

```diff
[dependencies.bevy]
git = "https://github.com/bevyengine/bevy"
rev = "11f52b8c72fc3a568e8bb4a4cd1f3eb025ac2e13"
- features = ["dynamic"]
+ features = ["jpeg", "dynamic"]
```

## List Types

#### Ordered List

1. First item
2. Second item
3. Third item

#### Unordered List

* List item
* Another item
* And another item

#### Nested list

* Fruit
  * Apple
  * Orange
  * Banana
* Dairy
  * Milk
  * Cheese

## Other Elements — abbr, sub, sup, kbd, mark

<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.

H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>

Press <kbd><kbd>CTRL</kbd>+<kbd>ALT</kbd>+<kbd>Delete</kbd></kbd> to end the session.

Most <mark>salamanders</mark> are nocturnal, and hunt for insects, worms, and other small creatures.

## Hyperlinked image

[![Google](https://www.google.com/images/branding/googlelogo/1x/googlelogo_color_272x92dp.png)](https://google.com)

## GitHub Gist

<script src="https://gist.github.com/spf13/7896402.js"></script>