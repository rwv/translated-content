---
title: 204 No Content
slug: Web/HTTP/Status/204
tags:
  - HTTP
  - Success
  - ステータスコード
  - リファレンス
translation_of: Web/HTTP/Status/204
---
{{HTTPSidebar}}

HTTP のレスポンスコード **`204 No Content`** は、リクエストが成功した事を示しますが、クライアントは現在のページから遷移する必要はありません。レスポンスコード 204 が返された場合は、デフォルトでキャッシュ可能になっています。そのようなレスポンスには、{{HTTPHeader("ETag")}} ヘッダーが含まれています。

レスポンスコード 204 は、主に、ユーザーに表示されるコンテンツ (ページの内容) の変更が不要な、{{HTTPMethod("PUT")}} リクエスト、リソースのアップデートなどに用いられます。リソースが作成される場合は、204 の代わりに、レスポンスコード {{HTTPStatus("201")}} `Created` が返されます。リクエスト後にページ内容の更新が必要な場合、レスポンスコード {{HTTPStatus("200")}} を用います。

## ステータス

    204 No Content

## 仕様

| 仕様                                                     | タイトル                                                      |
| -------------------------------------------------------- | ------------------------------------------------------------- |
| {{RFC("7231", "204 No Content" , "6.3.5")}} | Hypertext Transfer Protocol (HTTP/1.1): Semantics and Content |

## ブラウザの互換性

{{Compat("http/status", "204")}}

## 参照

- [HTTP リクエストのメソッド](/ja/docs/Web/HTTP/Methods)