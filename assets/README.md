# 資産

7つの区分のうち「資産」の台帳の項目の定義と、移行中の台帳を置きます。台帳は、装置、システム、ソフトウェアの構成、依存関係、保守の状況の一覧です。

- **正本は装置群ごとの運用リポジトリです**（[0006](../decisions/0006-資産の情報を装置群ごとの運用リポジトリに置く.md)）。各運用リポジトリの直下の `assets.yaml` に、下の項目で書きます。運用リポジトリの一覧は[目録](../catalog/catalog.yaml)にあります。
- **ハブにしかない装置の情報を置きません。** ハブに残すのは、項目の定義と、資産の索引（`id`、名称、運用リポジトリ）だけです。
- **仮置きの台帳は空になりました。** 2026-11-18 に、`nro45m.yaml` の項目をすべて運用リポジトリに移しました。ファイルは、判断記録からのリンクを保つために残しています。

確認日：2026-11-18

| ファイル | 範囲 | 状態 |
|---|---|---|
| [nro45m.yaml](nro45m.yaml) | 45m 鏡の観測システム | 空。初版の15件はすべて運用リポジトリに移した |

## 資産の索引

運用リポジトリに移した資産です。項目の中身は運用リポジトリの台帳が正本です。

| id | 名称 | 運用リポジトリ |
|---|---|---|
| nro45m | 45m 電波望遠鏡 | [nro-45m-antenna](https://github.com/nobeyama-radio-observatory/nro-45m-antenna/blob/main/assets.yaml) |
| beam-transmission | ビーム伝送系 | [nro-45m-antenna](https://github.com/nobeyama-radio-observatory/nro-45m-antenna/blob/main/assets.yaml) |
| nro45m-acu | アンテナ制御ユニット（ACU） | [nro-45m-antenna](https://github.com/nobeyama-radio-observatory/nro-45m-antenna/blob/main/assets.yaml) |
| nro45m-master-collimator | マスターコリメーター | [nro-45m-antenna](https://github.com/nobeyama-radio-observatory/nro-45m-antenna/blob/main/assets.yaml) |
| sw-cosmos | COSMOS（観測制御ソフトウェア） | [nro-45m-control](https://github.com/nobeyama-radio-observatory/nro-45m-control/blob/main/assets.yaml) |
| sw-obs-ui | 観測の操作のユーザーインターフェース | [nro-45m-control](https://github.com/nobeyama-radio-observatory/nro-45m-control/blob/main/assets.yaml) |
| sw-remote-obs | リモート観測のシステム | [nro-45m-control](https://github.com/nobeyama-radio-observatory/nro-45m-control/blob/main/assets.yaml) |
| ctl-computers | 制御用の計算機と仮想化の基盤 | [nro-45m-control](https://github.com/nobeyama-radio-observatory/nro-45m-control/blob/main/assets.yaml) |
| be-sam45 | SAM45（分光計） | [nro-45m-spectrometer](https://github.com/nobeyama-radio-observatory/nro-45m-spectrometer/blob/main/assets.yaml) |
| be-yatsugatake | YATSUGATAKE（分光計） | [nro-45m-spectrometer](https://github.com/nobeyama-radio-observatory/nro-45m-spectrometer/blob/main/assets.yaml) |
| sw-sam45compat | SAM45 互換のソフトウェア | [nro-45m-spectrometer](https://github.com/nobeyama-radio-observatory/nro-45m-spectrometer/blob/main/assets.yaml) |
| rx-h22 | H22 | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-h40 | H40 | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-z45 | Z45 | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-forest | FOREST（4ビーム受信機） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-hinotori-tz | HINOTORI-TZ | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-7bee | 7BEE（7ビーム3帯域受信機） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-t70 | T70（廃止） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-eq | eQ（所外の装置、試験中） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-s40 | S40（廃止） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-s100-80 | S100/80（廃止） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| rx-bears | BEARS（廃止） | [nro-45m-receivers](https://github.com/nobeyama-radio-observatory/nro-45m-receivers/blob/main/assets.yaml) |
| db-nrodb-nobeyama | NRODB（野辺山） | [nro-data](https://github.com/nobeyama-radio-observatory/nro-data/blob/main/assets.yaml) |
| db-nrodb-mitaka | NRODB（三鷹） | [nro-data](https://github.com/nobeyama-radio-observatory/nro-data/blob/main/assets.yaml) |
| db-radio-archive | 電波アーカイブ | [nro-data](https://github.com/nobeyama-radio-observatory/nro-data/blob/main/assets.yaml) |
| tool-obs-script | 観測指示書の作成ソフト | [nro-user-tools](https://github.com/nobeyama-radio-observatory/nro-user-tools/blob/main/assets.yaml) |
| tool-newstar | NEWSTAR | [nro-user-tools](https://github.com/nobeyama-radio-observatory/nro-user-tools/blob/main/assets.yaml) |
| tool-nostar | NOSTAR | [nro-user-tools](https://github.com/nobeyama-radio-observatory/nro-user-tools/blob/main/assets.yaml) |
| tool-cont | cont | [nro-user-tools](https://github.com/nobeyama-radio-observatory/nro-user-tools/blob/main/assets.yaml) |
| tool-casa-export | CASA の形式への書き出しとパイプライン処理 | [nro-user-tools](https://github.com/nobeyama-radio-observatory/nro-user-tools/blob/main/assets.yaml) |
| if-system | IF 系（共通 IF 系を含む） | [nro-45m-if](https://github.com/nobeyama-radio-observatory/nro-45m-if/blob/main/assets.yaml) |
| be-continuum | 連続波のバックエンド | [nro-45m-continuum](https://github.com/nobeyama-radio-observatory/nro-45m-continuum/blob/main/assets.yaml) |
| time-standard | 標準時計 | [nro-time-standard](https://github.com/nobeyama-radio-observatory/nro-time-standard/blob/main/assets.yaml) |

まだ入っていないもの：建物と共通の設備（電源、冷却、ネットワークなど）、計算機（所内の共通のサービス用の基盤）、観測所のほかの装置、事務のシステム、廃止した資産のうち受信機以外（AOS、旧 IF 系など。経緯は [history/](../history/README.md)）。

## 項目の定義

項目の定義の変更は、上流の変更として扱います。判断記録を添えたプルリクエストで行ってください。

| 項目 | 必須 | 内容 |
|---|---|---|
| `id` | 必須 | 識別子。英小文字、数字、ハイフン。ファイルをまたいで一意にする |
| `name` | 必須 | 名称。観測所で使っている呼び名 |
| `kind` | 必須 | 種別。`アンテナ`、`受信機`、`分光計`、`信号処理`、`制御`、`ソフトウェア`、`時刻`、`建物・設備`、`計算機` のいずれか |
| `part_of` | 任意 | どのまとまりの一部か。上位の `id` |
| `depends_on` | 任意 | 動くために必要なものの `id` の一覧。依存の向きは「この資産が、あれを必要とする」 |
| `status` | 必須 | 状態。`運用中`、`一部運用`、`試験中`、`停止中`、`廃止`、`計画中` のいずれか |
| `offered` | 任意 | 観測時間の利用者への提供の状態。`提供`、`リスクシェアで提供`、`所内のみ`、`提供停止`。利用者に提供しないものは書かない |
| `introduced` | 任意 | 導入の時期（年、または年度）。出典を `sources` に書く |
| `ended` | 任意 | 終了の時期 |
| `maintenance` | 必須 | 保守の状況。次の小項目を持つ |
| `maintenance.by` | 必須 | 保守の担い手の種類。`所内`、`メーカー`、`大学など外部`、`なし`、または組み合わせ。個人名は書かない |
| `maintenance.condition` | 必須 | 故障の傾向、予備品の有無、部品の入手の見込み。分からなければ `未記入` |
| `maintenance.effort` | 必須 | 保守の手間。`大`、`中`、`小`、または `未記入`。根拠（worklog の集計など）を `sources` に書く |
| `renewal` | 必須 | 更新の見込み。更新や廃止の予定、使い続けられる見込みの時期。分からなければ `未記入`。見立てなら `（仮説）` と添える |
| `owner_role` | 必須 | 担当の役割。個人名ではなく役割で書く。未定なら `未定` |
| `maintainers` | 必須 | 保守を担える人の数（単独で判断できる人の数）。人数だけを書き、個人に結びつけない。分からなければ `未記入` |
| `repos` | 任意 | 関係する製品と開発のリポジトリ。名前と URL を書く。運用リポジトリから下の層を参照する唯一の場所（[0006](../decisions/0006-資産の情報を装置群ごとの運用リポジトリに置く.md)） |
| `docs` | 任意 | 手順や資料の在りか。公開のものは URL。非公開のものは「非公開（所在のみ）」として場所の種類だけを書く |
| `sources` | 必須 | 各項目の出典（[0004](../decisions/0004-事実の根拠は出典で示す.md)）。聞き取りで得た値は、運用リポジトリの `interviews/YYYY-MM-DD.md` の該当の問いを指す。出典のない記述は仮説として扱う |
| `note` | 任意 | 補足 |

## 書き方の決まり

- **入れないもの：** 接続先、アドレス、アカウント、ネットワーク構成、制御の手順（[CONTRIBUTING.md](../CONTRIBUTING.md)）。保守の状況（故障の傾向、予備品の有無、外部の支援）は入れてよい。
- **聞き取りの記録：** 公開資料にない値は、保守の担い手に聞き取って集めます。書き方は [interviews.md](interviews.md) です。
- **`未記入` を残してよい。** 空欄にせず `未記入` と書くと、埋めるべき箇所が数えられる。
- **廃止した資産も残す。** `status: 廃止` と `ended` を書き、消さない。統合や更新の経緯の材料になる。経緯の要約は [history/](../history/README.md) にある。
