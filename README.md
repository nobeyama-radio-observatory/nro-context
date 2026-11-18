# nro-context

国立天文台 野辺山宇宙電波観測所の文脈基盤のハブです。

観測所の活動に関わる文脈（目的、判断の記録、資産、運用の知見など）を、人と AI が読める形で集めて公開します。このリポジトリはその入口で、データそのものは置きません。全体の索引と全リポジトリに共通の決まりを置き、個別のデータは種別ごとのリポジトリ（`nro-*`）に置きます。装置とシステムの情報は、装置群ごとの運用リポジトリに置きます（[0006](decisions/0006-資産の情報を装置群ごとの運用リポジトリに置く.md)）。

## 読み方

人も AI も、まず次の順に読んでください。

1. [catalog/catalog.yaml](catalog/catalog.yaml)：目録。文脈基盤に関わるすべてのリポジトリの一覧
2. [CONTRIBUTING.md](CONTRIBUTING.md)：進め方の決まり
3. [policy/disclosure.md](policy/disclosure.md)：公開方針

| 場所 | 中身 |
|---|---|
| [summary/](summary/README.md) | 現状サマリー。全体がどこまでできているかの要約 |
| [policy/](policy/) | 公開方針と、非公開の一覧（区分・理由・正本の場所だけ） |
| [catalog/](catalog/) | 目録と、その項目の定義 |
| [questions/](questions/) | 上流の問い。文脈基盤の完成度を測る物差し |
| [mission/](mission/) | 使命：目的、中期計画、法令、関係者 |
| [assets/](assets/README.md) | 資産の台帳の項目の定義と、運用リポジトリへ移すまでの仮置きの台帳 |
| [work/](work/README.md) | 業務の公開の項目の定義と、公開用の書き出しの手順（値は nro-work） |
| [metrics/](metrics/README.md) | 数値の項目の定義と、系列の索引（値は nro-metrics） |
| [history/](history/README.md) | 経緯：装置と運用形態の変更の年表 |
| [external/](external/README.md) | 外部：他の施設の事例、将来の施設と技術の動向 |
| [decisions/](decisions/) | 判断記録（ADR） |
| [skills/](skills/) | 観測所全体で使う Claude のスキルの正本 |

## 現状

立ち上げの準備中です。どこが埋まっていてどこが空いているかは、[現状サマリー](summary/README.md)にまとめています。

## 利用許諾

- コード：BSD 3-Clause License（[LICENSE](LICENSE)）
- 文書：クリエイティブ・コモンズ 表示 4.0 国際（CC BY 4.0、[LICENSE-docs](LICENSE-docs)）
