---
title: トランザクション
taxonomy:
    category:
        - t
---

## Transaction
2,100 sats

トランザクションはビットコインの移動の記録です。全てのトランザクションはブロックチェーンのブロックの中に記録されます。ほとんどのユーザはビットコイントランザクションを送ったり、受け取ったりするのにウォレットを使います。ウォレットがバックグラウンドで技術的な作業を行うので、ユーザはアドレスと金額を簡単に指定できます。

準備が整うとトランザクションはビットコインネットワーク上のノードにブロードキャストされます。マイナーがトランザクションをブロックに追加するまでの間、ノードはトランザクションをmempoolに保持します。mempoolは承認が保留されているトランザクションのプールです。承認されると、トランザクションはブロックに追加されます。トランザクションが確定したとみなすときの安全な方法は、少なくとも6ブロック経つまで待つことです。

トランザクションは、3つのパートで構成されます。インプット、アウトプット、署名です。インプットは支払者が使うと決めたUTXOと呼ばれるビットコインの一部です。アウトプットは指定されたアドレスに指定された金額のビットコインを送り、新しいUTXOを作ります。ひとつのトランザクションは複数のインプットと複数のアウトプットを持つことができます。最後に、トランザクションを有効にするために、支払者はトランザクションに署名しなければなりません。これにより、支払いに使うインプットが自分のものであることを証明します。この署名は支払い者の秘密鍵を使って作られます。

トランザクションの例を見てみましょう。アリスが1BTCのUTXOを持っていて、ボブに0.4BTC払いたいとします。彼女はインプットとして1BTCのUTXOを使います。アリスは2つのアウトプットを作ります。1つ目はボブへ送る0.4BTC、2つ目は彼女自身への0.59BTCのおつりとなるアウトプットです。この例では、0.01BTCがトランザクション手数料として支払われます。トランザクション手数料はアウトプットではありません。インプットの合計（1BTC）からアウトプットの合計（0.4＋0.59＝0.99）引いたものであり、これはマイナーのものになります。

最後に、アリスはトランザクションをブロードキャストする前に、インプットのUTXOを制御できる秘密鍵でトランザクションに署名します。このトランザクションがブロックチェーンに追加されると、1BTCのUTXOは削除されて、新しく0.4BTCと0.59BTCのUTXOが生成されます。0.4BTCのUTXOはボブが、0.59BTCのUTXOはアリスが所有します。

---
コンテンツの著作権は [River Financial](https://river.com/) に帰属します。二次利用の可否は権利者にご確認ください。 / All rights reserved to River Financial.