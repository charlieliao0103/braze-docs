---
nav_title: FAQ
article_title: WhatsApp FAQ
page_order: 80
description: "この記事では、WhatsAppキャンペーンの設定時によくある質問のいくつかに対処します。"
page_type: FAQ
channel:
  - WhatsApp

---

# よくある質問

> このページでは、WhatsAppに関する最も厳しい質問にお答えします！<br><br>このFAQは、法的助言を提供することを意図しておらず、法的助言として依拠することもできません。WhatsAppチャネルの使用は、特定のMeta Platforms, Inc.の要件に従います。すべての適用される要件および特定の法律に準拠してWhatsAppチャネルを使用していることを確認するために、法務顧問の助言を求めるべきです。

## FAQトピック
- [WhatsAppビジネスアカウント](#whatsapp-business-accounts)
- [WhatsAppビジネスアカウントの電話番号](#whatsapp-business-account-phone-numbers)
- [オプトインとサブスクリプション管理](#opt-in-and-subscription-management) 
- [メッセージングの制限](#messaging-limits) 
- [WhatsAppテンプレート](#whatsapp-templates)
- [配信可能性](#deliverability) 
- [その他](#miscellaneous)

### WhatsAppビジネスアカウント 

#### WhatsAppビジネスアカウントを作成するにはどうすればよいですか？ 
Braze ダッシュボードの埋め込みサインアップフローを通じて、WhatsApp ビジネスアカウント (WABA) を作成することをお勧めします。 

#### すでにMetaビジネスアカウントを持っています。WhatsAppビジネスアカウントはまだ必要ですか？ 
はい、WhatsAppビジネスアカウントを作成する必要があります。[メインのMetaビジネスアカウントの下にWABAをネストすることをお勧めします]({{site.baseurl}}/user_guide/message_building_by_channel/whatsapp/overview/)。 

#### WhatsAppビジネスアカウントにアクセスするにはどうすればよいですか？ 
埋め込みサインアップフローを完了すると、business.facebook.comでアカウントにアクセスでき、[WhatsAppセクション](https://business.facebook.com/wa/manage/home)に移動します。 

#### 複数のWABAをBrazeに接続できますか？ 
はい、ワークスペースごとに1つのWABAを接続できます。したがって、複数のWABAを複数のBrazeワークスペースに接続できます。例えば、異なるブランドのための異なるワークスペースや、異なる国のための異なるワークスペースがある場合、それぞれに独自のWABAを接続することができます。

### WhatsAppビジネスアカウントの電話番号 

#### WhatsAppビジネスアカウントに電話番号が必要ですか？ 
はい、アクセスできる番号が必要です。埋め込みサインアップフローを進める際に、2要素認証で電話番号を確認するよう求められます。電話番号は他のWhatsAppアカウント（ビジネスまたは個人）には使用できません。

#### WhatsAppでサポートされている電話番号の種類は何ですか？ 
Metaの[電話番号](https://developers.facebook.com/docs/whatsapp/phone-numbers)の要件を参照してください。 

#### 複数のWABAで1つの電話番号を使用できますか？ 
いいえ。電話番号は複数のWABAで共有することはできません。 

#### 特定の国にメッセージを送信するには、特定の種類の電話番号が必要ですか？ 
いいえ。WhatsAppを使用すると、サポートされている任意の国の任意の電話番号からエンドユーザーにメッセージを送信できます。Metaの[電話番号](https://developers.facebook.com/docs/whatsapp/phone-numbers)の要件を参照してください。 

#### 特定の国に送信するには、国ごとの電話番号を使用する必要がありますか？
いいえ。WhatsAppを使用すると、サポートされている任意の電話番号から、サポートされている任意の国のエンドユーザーに送信できます。

### オプトインおよびサブスクリプション管理 

#### エンドユーザーにWhatsAppでマーケティングメッセージを送信するためにオプトインを収集する必要がありますか？ 
はい、WhatsAppは企業がエンドユーザーにマーケティングメッセージを送信するために[オプトインの同意を収集する](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in/)ことを要求します。

#### WhatsAppでエンドユーザーに積極的にメッセージを送信してオプトインの同意を得ることはできますか？ 
エンドユーザーに積極的にメッセージを送信することを選択した場合、最初のビジネス開始メッセージでは、ユーザーがあなたのビジネスからマーケティングメッセージを受け取りたいかどうかを尋ね、Metaの[オプトインを取得する](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in/)要件に従う必要があります。WhatsAppはチャネル上であなたのビジネスの評判を監視するため、推奨される最善の方法はエンドユーザーに対して明確にし、彼らが受け取りたいと示したメッセージのみを送信することです。
 
#### オプトインを収集する際に、エンドユーザーの電話番号を収集する必要がありますか？ 
メッセージを送信するには、Brazeプロファイルにエンドユーザーの電話番号が必要です。 
- すでに相手の番号を持っている場合、オプトイン時に収集する必要はありません。 
- エンドユーザーの番号がない場合、オプトイン方法には電話番号の取得を含める必要があります。 

#### エンドユーザーのサブスクリプションステータスを更新するにはどうすればよいですか？ 
WhatsAppチャネルのサブスクリプション管理は、他のBrazeチャネルでの機能と同様に機能します。[ユーザーのサブスクリプション管理]({{site.baseurl}}/user_guide/message_building_by_channel/whatsapp/user_subscription/)を参照してください。  

#### もし、すでにWhatsAppでマーケティングメッセージを受け取ることに同意したユーザーのリストがある場合、Brazeで彼らのサブスクリプションステータスをどのように更新しますか？ 
[ユーザーインポート]({{site.baseurl}}/user_guide/data_and_analytics/user_data_collection/user_import#importing-custom-data)を介してサブスクリプションステータスを更新できます。 

#### オプトインを収集するためにどのような方法を使用すべきですか？ 
Brazeは、コンプライアンスを維持するために[Metaのオプトイン方法に関するガイドライン](https://developers.facebook.com/docs/whatsapp/overview/getting-opt-in/)を参照することをお勧めします。Brazeの[チャネルおよびオプトインのアイデアと提案](https://docs.google.com/document/d/1rNKnKN2oIn-e9bXdYEvnwdlzlCsEOKs-xREcdVvPBE8/edit)に関する次のリソースを参照してください。

#### WhatsAppにダブルオプトインは必要ですか？ 
いいえ、ダブルオプトインは必要ありません。 

#### ユーザーはどのようにしてWhatsAppメッセージの受信を拒否しますか？ 
ユーザーは2つの方法でオプトアウトできます:
1. 特定のオプトアウトワードを使用してインバウンドWhatsAppメッセージを設定し、Webhookを使用してユーザーのサブスクリプションステータスを更新します。
2. WhatsAppテンプレート内にオプトアウトのクイック返信を追加し、対応するWebhookで更新します。 

### メッセージングの制限 

#### メッセージングの制限とは何ですか？ 
メッセージングの制限は、WhatsAppの完全性を構築するための概念です。それらは、各電話番号がローリング24時間以内に開始できるビジネス開始会話の最大数を決定します。メッセージングの制限レベルは4つあります：1k、10k、100k、無制限。

#### メッセージングの上限を増やすにはどうすればよいですか？ 
WhatsAppは、次の条件を満たすとメッセージングの制限を増やします:
1. [電話番号ステータス](https://www.facebook.com/business/help/896873687365001) は **接続済み** 
2. [電話番号の品質評価](https://www.facebook.com/business/help/896873687365001)は**中**または**高**です
3. 過去7日間で、あなたは一意のユーザーとの会話をX回以上開始しました。ここで、Xは現在のメッセージング制限を2で割った値です。 

したがって、100kから無制限に移行するには、7日間で少なくとも50,000件のビジネス開始の会話を送信する必要があります。 

#### メッセージングの制限を増やすのにどれくらい時間がかかりますか？ 
すべての以前の条件が満たされている場合、4日以内にメッセージングの制限を1kから無制限に増やすことができます。 

#### 現在のメッセージング制限はどこで確認できますか？ 
**WhatsAppマネージャー > 概要ダッシュボード > インサイト**タブで現在のメッセージング制限を確認できます。 

#### メッセージングの上限に達しているときにメッセージを送信しようとするとどうなりますか？
現在の制限を超えてより多くのユニークユーザーにキャンペーンやキャンバスを送信しようとすると、メッセージの送信に失敗します。Brazeは、メッセージングの制限が増加した場合、最大1日間メッセージの再送信を試み続けます。 

#### メッセージングの制限が減少することはありますか？
はい、電話番号の品質評価が低すぎると、WhatsAppがメッセージングの制限を減らすリスクがあります。Brazeは、WhatsAppからの品質関連の更新、電話番号のステータスおよびメッセージング制限レベルの更新を購読して通知を受け取ることをお勧めします。WhatsAppマネージャーダッシュボードで通知を直接購読できます。 

#### Metaのスループット制限は何ですか？
Metaには、WABAメッセージング制限とは別に独自のスループット制限があります。クラウドAPIがサポートするデフォルトの制限は、1秒あたり80メッセージです。キャンペーンがこの制限を超えると思われる場合は、制限を増やすように[リクエスト](https://developers.facebook.com/docs/whatsapp/cloud-api/overview/#throughput)できます。Metaは、キャンペーンの送信の少なくとも3日前にこのリクエストを提出することをお勧めします。

### WhatsAppテンプレート 

#### WhatsAppテンプレートとは何ですか？ 
WhatsAppは、すべてのビジネスが開始するメッセージに承認されたテンプレートを使用する必要があります。テンプレートには、メッセージのコピーに加えて、画像、アクション、クイック返信ボタンなどのオプションのリッチメディアが含まれています。WhatsAppがテンプレートを承認すると、それらを使用してBrazeでWhatsAppメッセージを作成できます。 

#### WhatsAppテンプレートの作成、編集、管理はどこで行いますか？ 
テンプレートを作成、編集、管理、および送信して、WhatsAppマネージャーで直接承認を受けます。WABAがBrazeに接続されると、ダッシュボードにすべてのテンプレートがステータスインジケーターとともに表示されます。テンプレートが拒否された場合は、WhatsAppマネージャーを通じて直接再提出します。**テンプレートはBrazeで直接作成または編集することはできません。**

#### WhatsAppがテンプレートの提出をレビューするのにどれくらい時間がかかりますか？ 
承認プロセスには最大で24時間かかることがありますが、テンプレートは数時間または数分で処理されることがよくあります。 

#### 一度にいくつのテンプレートを持つことができますか？ 
メッセージテンプレートの制限は、ビジネス認証ステータスによって異なります。**WhatsApp マネージャー > メッセージテンプレート**ページで制限を確認できます。 

#### Brazeでテンプレートコピーとリッチメディアをパーソナライズするにはどうすればよいですか？ 
WhatsAppは、メッセージテンプレートに変数パラメータを挿入することができます。メッセージは変数パラメータで始まったり終わったりすることはできません。変数パラメータはBrazeプラットフォームのLiquidロジックで入力できます。BrazeでWhatsAppメッセージを作成する方法については、可変パラメータの詳細を学ぶために[参照してください]({{site.baseurl}}/user_guide/message_building_by_channel/whatsapp/whatsapp_campaign/create#step-2-compose-your-whatsapp-message)。 

#### 私のテンプレートは拒否されました。Brazeは承認を得るのに役立ちますか？ 
Brazeチームはテンプレートの拒否を確認できません。テンプレートを編集して再送信するには、WhatsAppビジネスマネージャーと直接連携する必要があります。必要に応じてサンプルテンプレートを提供してください。テンプレートがMetaの[ビジネス](https://www.whatsapp.com/legal/business-policy/?fbclid=IwAR2qWg6yFKdyjDMxJkbNSM38FLGsxXxffC1qStY2gaHOyp-gl_8g72rZNIw)または[商取引](https://www.whatsapp.com/legal/commerce-policy/?fbclid=IwAR3bzN3LTZ-7kO-wnO7X3smtPKGy0asxaFod-U1Ub8B9JUpnrfy1_y7LpAQ)ポリシーに従っていることを再確認してください。

#### リッチメディアはBrazeでターゲティングまたはパーソナライズされたものにできますか？ 
画像はメディアライブラリーからアップロードできますが、動的にターゲットにすることはできません。URL の場合、リンクの最後の部分は Liquid を使用して動的に入力できます。 

### 配信可能性 

#### なぜメッセージが配信されないのですか？ 
メッセージが配信されない理由はさまざまで、ネットワークの問題やデバイスの電源が切れていることなどが含まれます。 

#### メッセージが配信されない場合、請求されますか？ 
いいえ。メッセージが配信されない場合、請求されません。 

#### エンドユーザーが私のビジネスをブロックした場合どうなりますか？ 
エンドユーザーがあなたのビジネスをブロックした場合、その後に送信しようとするメッセージは配信されず、請求もされません。 

#### エンドユーザーがメッセージを報告した場合はどうなりますか？ 
エンドユーザーがメッセージを報告した場合でも、このユーザーに後続のメッセージを送信できます。ただし、報告はチャネルの品質評価に影響を与える可能性があります。 

#### エンドユーザーが私のビジネスをブロックまたは報告した場合、Brazeで彼らのサブスクリプションステータスは更新されますか？ 
いいえ。彼らのBrazeサブスクリプションステータスは更新されません。 

### その他

#### Brazeは、WhatsAppのチャットボットや人間が支援するチャットのような顧客サポートのユースケースをサポートしていますか？ 
Brazeまたは直接統合を通じて、チャットボットや人間が支援するチャットをサポートしていません。 

すでに顧客サポートチャネルとしてWhatsAppを使用している場合は、現在の設定を維持し、マーケティングメッセージング用にBrazeを介して新しいWABAを作成することをお勧めします。このWABAには新しい電話番号が必要です。 

#### どのようにして顧客サポートメッセージングとマーケティングメッセージングをBrazeを通じて「ギャップを埋める」ことができますか？ 
WhatsApp Liquidプロパティを使用して、Brazeから他のプラットフォーム（メッセージ本文やメディアURLを含む）に受信WhatsAppメッセージの内容を転送できます。これには、任意の顧客サポートツールが含まれます。詳細については、[サポートされているパーソナライゼーションタグ]({{site.baseurl}}/user_guide/personalization_and_dynamic_content/liquid/supported_personalization_tags/)をご覧ください。 

Brazeに情報を送信するには、例えば、ユーザーがアクティブなサポート会話に参加していることを示すために、カスタム属性（例えば、ブール値の「既存のサポートチャットがある = true/false」）を記録し、それをマーケティングキャンペーンのセグメンテーション基準として使用できます。また、2つのチャットスレッド間でディープリンクを作成して、ユーザーをマーケティングスレッドからサポートスレッドに、またその逆に誘導することもできます。 

#### Brazeはユーザーの回答を保存しますか？ 
メッセージは処理されるまでの間だけ保存されます。ユーザーメッセージにアクセスするには、Currentsを使用します。 

#### ユーザーの電話番号はBrazeにどのように保存する必要がありますか？ 
ユーザーの電話番号は[E.164形式]({{site.baseurl}}/user_guide/message_building_by_channel/whatsapp/user_phone_numbers/#formatting)で保存する必要があります。

#### WhatsApp テンプレートでサポートされているリッチメディアの種類は何ですか？ 
WhatsAppテンプレートに画像、アクション（URLまたは電話番号）、クイック返信ボタンを追加できます。WhatsAppでテンプレートを直接作成する際に、これらの要素を追加できます。 

#### ユーザーの電話番号をインポートできますか？ 
そうです。[ユーザーの電話番号をインポートできます]({{site.baseurl}}/user_guide/message_building_by_channel/whatsapp/user_phone_numbers/)。 

#### 事業の検証とは何ですか？ 
ビジネス認証は、ブランドが正当なビジネスであることを確認するために使用されるWhatsAppの概念です。WhatsAppマネージャーで完了できます。ビジネスの確認もメッセージングを拡大するために必要です。ビジネス認証がない場合、顧客は24時間のローリング期間に最大250人のユニークなエンドユーザーにしか送信できません。 

#### 公式ビジネスアカウントとは何ですか？ 
OBAは表示名の横に緑のチェックマークを付けるオプションです。事業認証を完了した後、公式ビジネスアカウントに申し込むことができます。ビジネス認証と公式ビジネスアカウントは異なるWhatsAppの概念であることに注意してください。 

#### Brazeダッシュボードで利用可能な指標は何ですか？ 
Brazeダッシュボードで一意の受信者、送信、配信、読み取り、および失敗を確認できます。エンドユーザーの既読レシートが「オン」になっている必要があることに注意してください。Brazeが読み取りを追跡するためです。コンバージョンイベントを設定して、他のチャネルと同様にキャンペーンのパフォーマンスを監視することもできます。 

#### WhatsAppの会話とは何ですか？ 
WhatsAppは2ウェイメッセージングに焦点を当てたチャネルであり、したがって個々のメッセージの数ではなく会話に基づいています。会話は、ビジネスとエンドユーザーの間の24時間のスレッドです。

- **ビジネスが開始した会話**:ビジネスが承認されたテンプレートメッセージをエンドユーザーに送信することから始まる会話。ビジネスがメッセージを送信するとすぐに、24時間のウィンドウが始まります。
- **ユーザー-initiated conversation**:エンドユーザーがビジネスにメッセージを送信する会話。ビジネスが返信メッセージを送信すると、これにより24時間のウィンドウが開始されます。

#### 電話番号の品質評価に影響を与える要因は何ですか、そして品質評価が低すぎるとどうなりますか？ 
電話番号の品質評価に影響を与える要因には、エンドユーザーがビジネスをブロックすること（およびビジネスをブロックする際に提供する理由）や、エンドユーザーがビジネスを報告することが含まれます。 

品質評価が低い場合、電話番号のステータスは**接続済み**から**フラグ付き**に変更されます。品質が7日間改善されない場合、ステータスは**Connected**に戻ります。ただし、メッセージングの制限は次のレベルに減少します。例えば、以前はメッセージングの上限が100,000だった電話番号が、現在はメッセージングの上限が10,000になっています。
