---
layout: post
title: DManual-Top
date: 2014-9-2 11:10:00
category: dmanual
tag: dmanual
---

## これはなんなの？

D言語の入門記事を目指しているドキュメントです。  
対象を「全くプログラミングをしたことがない人」にしたいですが、
k3kaimuの文章がわかりにくいために、「C言語がある程度使える人向け」な記事になっています。


### ライセンス

このページを含め、原則としてd-manualのすべての記事(ソースコードを含む)にはCC BY-NC-SAを適用します。  

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.ja"><img alt="クリエイティブ・コモンズ・ライセンス" style="border-width:0" src="http://i.creativecommons.org/l/by-nc-sa/3.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" href="http://purl.org/dc/dcmitype/Text" property="dct:title" rel="dct:type">d-manual</span> は <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/3.0/deed.ja">クリエイティブ・コモンズ 表示 - 非営利 - 継承 3.0 非移植 ライセンスの下で提供されています。</a>.

プログラムのソースコードとは違い、ドキュメントはある程度厳しいライセンスであったほうがよいと判断しました。


### 執筆者リスト

* けーさん(twitter: k3_kaimu, github: k3kaimu)


### 執筆協力者の皆様

以下に記載しているのは、監修や推敲などで記事の執筆を協力してくださった方々です。
ありがとうございます。

* きょんたん (twitter: kyonfuee, github: kyontan)
* github: majiang
* github: shirataki
* tom tan (twitter: tm_tn, github: tom-tan)

## 記事リスト

<div class="list-group">
{% assign sorted_pages = (site.pages | sort: 'title') %}
{% for post in sorted_pages %}
{% for cp in post.categories %}
{% if cp[0] == dmanual %}
  <a href="{{ site.baseurl }}{{ post.url }}" class="list-group-item col-md-6 col-sm-12 col-xs-12">
    <p class="list-group-item-heading">{{ post.title }}</p>
  </a>
{% endif %}
{% endfor %}
{% endfor %}
</div>
