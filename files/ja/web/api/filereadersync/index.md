---
title: FileReaderSync
slug: Web/API/FileReaderSync
---

{{APIRef("File API")}}

`FileReaderSync` インターフェイスで、 {{DOMxRef("File")}} または {{DOMxRef("Blob")}} オブジェクトを同期的に読み込むことができます。

{{AvailableInWorkers}}

> **Warning:** このインターフェイスは、ブロックが発生する可能性がある同期 I/O を使用するため、[ワーカー](/ja/docs/Web/API/Worker)**でのみ**利用できます。

## プロパティ

このインターフェイスにはプロパティはありません。

## メソッド

- {{DOMxRef("FileReaderSync.readAsArrayBuffer","FileReaderSync.readAsArrayBuffer()")}}
  - : このメソッドは、指定された {{DOMxRef("Blob")}} または {{DOMxRef("File")}} を、入力データをバイナリー文字列として表す {{jsxref("ArrayBuffer")}} に変換します。
- {{DOMxRef("FileReaderSync.readAsBinaryString","FileReaderSync.readAsBinaryString()")}} {{deprecated_inline}}
  - : このメソッドは、指定された {{DOMxRef("Blob")}} または {{DOMxRef("File")}} を、入力データをバイナリー文字列として表す文字列に変換します。このメソッドは非推奨であり、代わりに `readAsArrayBuffer()` を使用することを検討してください。
- {{DOMxRef("FileReaderSync.readAsText","FileReaderSync.readAsText()")}}
  - : このメソッドは、指定された {{DOMxRef("Blob")}} または {{DOMxRef("File")}} を、入力データをテキスト文字列として表す文字列に変換します。オプションの **`encoding`** 引数は、使用するエンコーディングを示します（例: iso-8859-1 や UTF-8）。これがない場合、このメソッドはエンコーディングの検出アルゴリズムを適用します。
- {{DOMxRef("FileReaderSync.readAsDataURL","FileReaderSync.readAsDataURL()")}}
  - : 指定された {{DOMxRef("Blob")}} または {{DOMxRef("File")}} を、入力データをデータ URL として表す文字列に変換します。

## 仕様書

{{Specifications}}

## ブラウザーの互換性

{{Compat}}

## 関連情報

- {{DOMxRef("FileReader")}}
- {{DOMxRef("BlobBuilder")}}, {{DOMxRef("Blob")}}
- {{DOMxRef("File")}}
- {{DOMxRef("FileReader")}}
