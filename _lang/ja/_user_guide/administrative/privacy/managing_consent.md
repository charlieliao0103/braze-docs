---
nav_title: 同意の管理
article_title: 同意の管理
page_order: 10
page_type: reference
description: "このリファレンス記事には、Braze を使用して同意を管理する方法のヒントがあります。"
---

# 同意の管理

> このリファレンス記事には、Braze を使用してユーザーからの同意を管理する方法のヒントがあります。

Braze では、法令の解釈に関する具体的な助言や、同意の管理の取り扱いに関するガイダンスを提供することができません。これは、お客様の法務部による法律の解釈に基づかなければならないためです。しかし、弊社ではサブスクリプションと同意の管理をサポートするさまざまなツールを提供しています。

お客様の手法は、法務部による法律の解釈に基づいて要求される厳格さによって決まります。ここでは、検討すべきオプションを、最も厳しいものから順にいくつかリストします。

- **チーム:**真のガバナンスを実現するために、[Braze のチーム][1]を使用します。そして、すべてのユーザープロファイルに、同意ステータス、同意日、またはその両方を示すカスタム属性を追加します。次に、すべてのキャンペーンとキャンバスをその指定チームに移行し、ダッシュボードのユーザー権限を適宜調整する必要があります。
- **ユーザープロファイル属性:**すべてのユーザープロファイルに同意属性を追加します。この属性は、ユーザーが同意したかどうかを示します。その後、同意したユーザーのセグメント (`consent = true` など) をすべてのキャンペーンとキャンバスに含めることができます。
- **チャネル固有のサブスクリプショングループ:**特定のチャネル (プッシュ通知、メールなど) のサブスクリプショングループを操作して、同意を管理します。まず、これらのチャネルからユーザーを配信停止としてマークし、ユーザーが同意した後にのみサブスクリプション登録済みとしてマークします。

{% alert important %}
法務部に問い合わせて、組織の同意管理要件へのコンプライアンスを満たす適切な手法を決定してください。
{% endalert %}

[1]: {{site.baseurl}}/user_guide/administrative/manage_your_braze_users/teams/
