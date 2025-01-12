---
nav_title: カスタムイベントの追跡
article_title: Roku のカスタムイベントのトラッキング
platform: Roku
page_order: 2
page_type: reference
description: "このページでは、Roku のカスタムイベントを Braze SDK から記録する方法について説明します。"

---

# カスタムイベントのトラッキング

> Braze でカスタムイベントを記録することで、アプリの使用パターンに関する詳細を把握し、ダッシュボードでのアクションによってユーザーをセグメント化できます。また、[イベントの命名規則]({{site.baseurl}}/user_guide/data_and_analytics/custom_data/event_naming_conventions/)についてもよく理解しておくことをお勧めします。

## カスタムイベントの追加

```brightscript
m.Braze.logEvent("YOUR_EVENT_NAME")
```

### プロパティの追加

カスタムイベントに関するメタデータを追加するには、カスタムイベントとともにプロパティディクショナリを渡します。

プロパティはキーと値のペアとして定義されています。 キーは `String` オブジェクトで、値は `String` または `Integer` になります。

```brightscript
m.Braze.logEvent("YOUR_EVENT_NAME", {"stringPropKey" : "stringPropValue", "intPropKey" : Integer intPropValue})
```
