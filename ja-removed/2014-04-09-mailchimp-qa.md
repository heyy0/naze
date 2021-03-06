---
layout: post
title: "MailChimpについてのQ&A"
tags: ["1404-April 2014"]
see_also: ["/mail-magazine"]
ogi: "021"
---

わたしがメルマガに使っているソフトウェア・[MailChimp](http://mailchimp.com/)について色々と質問を頂くことが多くなりましたので、それらの答えをまとめています。随時更新中です。

## 購読解除リンクについて

> [上杉様の記事](/mail-magazine)には「MailChimpにはワンクリックで購読を解除する機能が備わっており(画像参照)」とありました。
>
> 私はMailChimpを使ってメール購読のシステムを作ろうと設定を行っていたのですが、テストメールを配信し、試しに購読を停止する「unsubscribe from this list」というリンクをクリックしたら、確かにそのまま自動ですぐに購読が解除されてしまいました。一瞬だけ「Unsubscribe form」という画面が表示されましたが、そこにはすでに自分のアドレスが自動で入力されていたため、こちらでは何の作業も入力もせずに数秒で自動的にページがジャンプされ、「Unsubscribe Successful」になってしまいました。
>
> 「ワンクリックで購読解除」というのは、このことでしょうか。これでは、誤ってリンクをクリックした瞬間にすぐに解除されてしまいます。自分でアドレスを入力して確認するというもう１つのプロセスをしっかり踏みたいのですが、そのようなプロセスを加えることはできないのでしょうか。これだとせっかく登録していただいたメンバーを簡単に失ってしまいそうで不安に感じてしまいました。

[Wikipedia](http://en.wikipedia.org/wiki/Email_marketing)によると、「ワンクリックで購読解除」はアメリカの規制に従うために必要なようです:

> The CAN-SPAM Act of 2003 authorizes a US $16,000 penalty per violation for spamming each individual recipient. Therefore, many commercial email marketers within the United States utilize a service or special software to ensure compliance with the Act. ... To comply with the Act's regulation of commercial email, services typically require users to authenticate their return address and include a valid physical address, provide a one-click unsubscribe feature, and prohibit importing lists of purchased addresses that may not have given valid permission.
>
> 2003年に施行されたCAN-SPAM法によると、スパムメール行為に対し受け取った人数×$16,000の罰金が課せられることがある。よって、米国内の商業目的のEメールマーケターは、CAN-SPAM法に沿ったマーケティングソフトやサービスを利用することが多い。それらのソフトやサービスは(1)ユーザーに購読用メールアドレスを確認させること、(2)発信人の物理的な住所を記載すること、**(3)ワンクリックで購読を解除できるようにすること**、(4)ユーザーのメールアドレスを無断で購読リストに追加しないことなどが義務付けられている。

MailChimpはアメリカ発のソフトなので、このような制限があるのですね。最近になり、Gmailにも購読解除を容易にする機能が[追加されたようです](http://gigazine.net/news/20140224-gmail-add-unsubscribe/):

> 2014年2月24日からGmailは、ユーザーが広告メールを簡単に購読中止できるように、広告メールの最上部にある差出人のメールアドレスの横に「メーリングリストの登録解除」というリンクを追加しました。リンクは自動的に追加されているので、ユーザー側で設定を操作する必要はありません。

質問への答えですが、法律で義務付けられている以上、ワンクリックで解除されてしまうのは避けられません。ですので、この問題については次のように考てみてはいかがでしょうか。

1. **購読解除のリンクを一番下に配置し、リンクを日本語にしておく**

    「誤ってリンクをクリックした瞬間にすぐ解除されてしまいます」というのはごもっともです。しかし、リンクをメールの下部に配置し、日本語で「購読を解除する」と明記しておけば、誤ってクリックしてしまう確率を下げることができます。わたしのメルマガでもそのようにしています。

    {% include i.html i='1.png' t='border' %}

    リンクを日本語にするには、デザインを編集する必要があります。メールの編集画面で該当部分をクリックすれば編集できます。文字は小さく薄くしたほうが良いですが、可読性が失われない程度にしましょう。

    {% include i.html i='3.png' t='border' %}

    2回め以降は、キャンペーンをReplicate(コピペ)すればデザインを使いまわすことができます。

    {% include i.html i='2.png' t='border' %}

2. **誤って購読を解除してしまっても、ユーザーはすぐ購読し直せる**

    購読を解除すると以下のようなメールが送られてくるのですが、このメール内の「購読する」リンクをクリックすれば購読し直すことができます。

    {% include i.html i='4.png' t='border' %}

3. **当たり前だが、質が良ければ購読解除する人は減る**

    わたしのメルマガにもワンクリックで購読を解除できるリンクを貼っていますが、3通のメールを数百人に送ったにもかかわらず、2人しか購読を解除していません。

    {% include i.html i='5.png' t='border' %}

    購読を解除されるかどうかは、購読解除リンクがワンクリックであるかないかよりもコンテンツの質で決まると思います。「購読を解除する」リンクをクリックしようと思われた時点でもう手遅れ、と考えたほうが良いでしょう。
