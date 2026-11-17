---
name: "nro-context"
description: "野辺山宇宙電波観測所の文脈基盤（GitHub の nobeyama-radio-observatory/nro-context）への入口。観測所全体に関わる問い（業務改善、システムやソフトウェアの統合整理、新規事業、ビジョン策定）を扱うとき、複数のリポジトリにまたがる作業をするとき、観測所の装置・業務・判断の経緯・公開方針を調べるとき、文脈基盤のリポジトリ（nro-context、nro-*）に変更を加えるときに使う。ハブの目録と進め方の決まりを最初に読ませる。"
---

# nro-context：観測所の文脈基盤への入口

このスキルは入口だけを持ちます。決まりや中身は書き写さず、ハブのリポジトリを読みに行きます。

## 最初に読むもの

ハブは `nobeyama-radio-observatory/nro-context` です。手元にクローンがあればそれを、なければ GitHub から次の順に読みます。

1. 目録：https://raw.githubusercontent.com/nobeyama-radio-observatory/nro-context/main/catalog/catalog.yaml
2. 進め方の決まり：https://raw.githubusercontent.com/nobeyama-radio-observatory/nro-context/main/CONTRIBUTING.md
3. 公開方針：https://raw.githubusercontent.com/nobeyama-radio-observatory/nro-context/main/policy/disclosure.md

そのうえで、必要なときだけ目録にある個別のリポジトリに入ります。上流の問いを扱うときは `questions/README.md` を、過去の判断を調べるときは `decisions/` を読みます。

## 必ず守ること

次の三つは CONTRIBUTING.md にもありますが、取り返しがつかないのでここにも書きます。

- **公開リポジトリに機微情報を入れない。** 個人に結びつく情報、装置の制御やセキュリティの詳細、契約、未公開の観測データ、認証情報。迷ったら入れずに issue で相談する。
- **主ブランチに直接書き込まない。** 作業用のブランチで変更を作り、プルリクエストを出す。
- **取り込みは人が行う。** AI が作ったプルリクエストと issue には、ラベル `AI作成` を付ける。

## 答えるときの規則

- 根拠には、ハブやリポジトリの該当ファイルを示す。根拠の確からしさを、体系知（研究で裏づけ）、実践知（他組織で実績）、仮説（観測所内の経験や見立て）に区別する。
- 文脈基盤に記録がないことは「記録がない」と言う。推測で補うときは推測だと明示する。
- 上流の問いに答えられなかった点は、issue（雛形「上流の問いへの未回答」）として記録することを提案する。
