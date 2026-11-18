# 数値

7つの区分のうち「数値」の項目の定義と、数値の系列の索引を置きます。値そのものの正本は、数値のリポジトリ `nro-metrics` です（[0007](../decisions/0007-業務と数値を区分ごとのリポジトリに置き数値から始める.md)）。

項目の定義の変更は、上流の変更として扱います。判断記録を添えたプルリクエストで行ってください。

## 置き方

- **系列ごとに1ファイル。** `nro-metrics` の `series/<id>.yaml` に置きます。系列とは、同じ定義で数えた値の並び（たとえば「年度ごとの見学者数」）です。
- **定義を値と一緒に持つ。** 何をどう数えたかが変わったら、別の系列にします。同じファイルの中で定義を変えると、前後の値を比べられなくなるためです。

## 項目

| 項目 | 必須 | 内容 |
|---|---|---|
| `id` | 必須 | 識別子。英小文字、数字、ハイフン |
| `name` | 必須 | 名称 |
| `category` | 必須 | 分類。`運用`（提供時間、停止など）、`利用`（観測提案、利用者など）、`障害`、`成果`（論文など）、`広報`（見学者など）、`人員`、`予算`、`料金` のいずれか |
| `unit` | 必須 | 単位（時間、件、人、%、円など） |
| `period` | 必須 | 値の区切り。`年度`、`暦年`、`月`、`観測期`（有料望遠鏡時間の期など）、`時点` のいずれか |
| `definition` | 必須 | 何をどう数えたか。分からない部分は「未確認」と書く |
| `assets` | 任意 | 装置に紐づく系列なら、資産の `id` の一覧（[assets/](../assets/README.md) の索引で引ける） |
| `owner_role` | 必須 | 更新の担当の役割。未定なら `未定` |
| `update` | 必須 | 更新の頻度。`年次`、`月次`、`随時`、`止めた系列`（過去の値だけを持つ）など |
| `values` | 必須 | 値の列。次の小項目を持つ |
| `values[].period` | 必須 | 区切りの値（例：`2019`、`2019年度`、`2026-11`、`第41期`） |
| `values[].value` | 任意 | 値（数）。範囲しか分からないときは書かず、`range` を使う |
| `values[].range` | 任意 | 範囲 `[下限, 上限]` |
| `values[].estimate` | 任意 | `true` なら見積もり。グラフからの読み取り、聞き取りの見立てなど。理由を `note` に書く |
| `values[].source` | 必須 | 出典（[0004](../decisions/0004-事実の根拠は出典で示す.md)）。資料とページ、または聞き取りの記録 |
| `values[].note` | 任意 | 補足 |
| `note` | 任意 | 系列全体の補足 |

## 書き方の決まり

- **個人が特定できるほど細かくしない。** 人数は、1〜2人のチームの内訳を出さず、グループ単位でまとめます。判断レベルの集計は業務の区分（`nro-work`）で扱い、ここには置きません。
- **予算は公開資料の水準から始める。** 内訳の公開の範囲は、担当と確かめてから広げます。
- **出典が食い違うときは、一次資料を採る。** 年次報告と40周年記念誌が食い違えば、年次報告を採ります（[history/](../history/README.md) と同じ）。
- **値のない年は書かない。** 0 と「記録がない」を混同しないためです。

## 系列の索引

値の正本は [nro-metrics](https://github.com/nobeyama-radio-observatory/nro-metrics) です。ここには系列の一覧だけを置きます。

| id | 名称 | 区切り | 期間 |
|---|---|---|---|
| [budget-operations](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/budget-operations.yaml) | 観測所の予算（規模） | 年度 | 2023年度 |
| [charge-per-hour](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/charge-per-hour.yaml) | 有料の望遠鏡時間の単価 | 時点 | 2026-11-18 時点（国内の機関の研究代表者）〜2026-11-18 時点（国外の機関の研究代表者） |
| [downtime-ratio](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/downtime-ratio.yaml) | 45m 鏡の観測の停止の割合（天候と技術的な故障） | 年度 | 2019年度〜2020年度 |
| [offered-hours](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/offered-hours.yaml) | 45m 鏡の観測の提供時間 | 年度 | 2018年度〜2022年度 |
| [papers-refereed-45m](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/papers-refereed-45m.yaml) | 査読論文の数（45m 鏡） | 暦年 | 2013〜2021 |
| [papers-refereed-all](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/papers-refereed-all.yaml) | 査読論文の数（観測所全体） | 暦年 | 2013〜2021 |
| [papers-refereed-nma](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/papers-refereed-nma.yaml) | 査読論文の数（ミリ波干渉計） | 暦年 | 2013〜2021 |
| [proposals-accepted](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/proposals-accepted.yaml) | 45m 鏡の共同利用の観測提案の採択件数 | 年度 | 1982年度〜2021年度 |
| [proposals-submitted](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/proposals-submitted.yaml) | 45m 鏡の共同利用の観測提案の件数 | 年度 | 1982年度〜2021年度 |
| [staff-technical-onsite](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/staff-technical-onsite.yaml) | 現地の技術系職員の数 | 年度 | 2018年度〜2019年度 |
| [staff-total](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/staff-total.yaml) | 観測所の職員の数（規模） | 年度 | 2023年度 |
| [trouble-count](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/trouble-count.yaml) | 45m 鏡の障害の件数（観測期） | 観測期 | 2026-2027年の観測期（2026-11-12 まで） |
| [visitors-monthly](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/visitors-monthly.yaml) | 見学者数（月） | 月 | 2012-04〜2021-03 |
| [visitors-yearly](https://github.com/nobeyama-radio-observatory/nro-metrics/blob/main/series/visitors-yearly.yaml) | 見学者数（年度） | 年度 | 1982年度〜2020年度 |
