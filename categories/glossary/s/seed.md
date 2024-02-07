---
title: シード
taxonomy:
    category:
        - s
---

## Seed
2,100 sats

シードは階層型決定性(Hierarchical Deterministic,略してHD)ウォレットを生成するために使用するデータです。これさえあれば、ウォレットの秘密鍵と公開鍵の再生成が可能なため、バックアップとして有効です。HDウォレットにおいてシードは決定論的であるため、所与のシードからは毎回全く同じ鍵が生成されます。また1つのシードから生成可能な公開鍵と秘密鍵のペアはほぼ無限です。

シードは単なるエントロピーであり、ランダムな数字の羅列でしかありません。シードはマスター秘密鍵と呼ばれる1つの拡張秘密鍵（extended private key/xprv）を生成するために使用され、拡張秘密鍵からは子秘密鍵だけでなく子公開鍵も生成できます。ウォレット利用者は拡張秘密鍵から必要に応じて無限に鍵ペアを生成することができるため、アドレスの再利用を回避してプライバシーを守れるだけでなく、ウォレットのバックアップも簡単にできます。

ランダムな数字の羅列であるシードは扱いにくいため、通常はニモニックフレーズで表現されます。ウォレットのバックアップにもニモニックフレーズが使われます。シードはビットコイン改善提案BIP32、ニモニックフレーズはBIP39で標準規格とされています。

---
コンテンツの著作権は [River Financial](https://river.com/) に帰属します。二次利用の可否は権利者にご確認ください。 / All rights reserved to River Financial.