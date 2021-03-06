---
title: パイプライン順序の更新
type: apicontent
order: 25.2
external_redirect: "/api/#update-pipelines-order"
---

## パイプライン順序の更新

パイプラインの順序を更新します。ログは順番に処理されるため、パイプラインの順序を変更すると、他のパイプラインやそのプロセッサーによって処理されるデータの構造や内容が変化する可能性があります。

**注**: `PUT` メソッドを使用すると、現在の順序を Datadog Organization に送信された新しい順序に**置き換えて**、パイプライン順序が更新されます。

**引数**:

* **`pipeline_ids`** [必須]:
    `<PIPELINE_ID>` 文字列の順序付き配列。配列内のパイプライン ID の順序は、Datadog のパイプライン全体の順序を定義します。
