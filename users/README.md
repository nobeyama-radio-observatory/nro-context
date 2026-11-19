# 利用者と観測者の資料と窓口

45m 鏡の利用者（観測提案を作る人）と観測者（観測時間を割り当てられた人）が読む公開資料の所在と、問い合わせの窓口の索引です（[0012](../decisions/0012-利用者と観測者の資料と窓口の所在をハブに索引する.md)）。

- **正本は観測所のウェブサイトです。** ここには所在と、要点を一行だけ書きます。手順、締切、料金、性能の値は写しません。使う前に必ず正本で確かめてください。
- **装置ごとの資料は、各運用リポジトリの台帳の `docs` にあります。** 受信機、分光計、アンテナ、データの保管、解析のソフトウェアの資料です。ここでは、装置をまたぐ資料と窓口だけを扱います。
- **非公開の資料は、所在だけを書きます。** 中身と接続先は書きません（[非公開の一覧](../policy/non-public.md)）。

確認日：2026-11-19（各ページの本文を読んで確かめた。ページの最終更新日は括弧内）

## 窓口

役割と経路だけを書きます。宛先（メールアドレス、招待の URL）は正本のページで確かめてください。

| 用件 | 窓口（役割） | 経路 | 宛先が書かれている正本 |
|---|---|---|---|
| 45m 鏡の共同利用全般の質問と要望（提案の前後とも） | ヘルプデスク | メーリングリスト、Discord | [プロポーザル募集](https://www.nro.nao.ac.jp/projects/45m/proposals/calls/)の「Helpdesk」の節（2026-11-17） |
| 大学などからのリモート観測の準備（接続試験）、VPN の期限の延長、観測指示書の作成で困ったとき | 計算機チーム（NRO computing team） | メール | [観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)は「計算機チームに連絡」とするだけで、宛先がない（下の「一次資料の食い違いと欠け」1） |
| 観測の中断、終了、次の観測者への引き継ぎの連絡 | 観測者と観測所の間 | Rocket.Chat の #ObsMessages | [望遠鏡運用のルール](https://www.nro.nao.ac.jp/projects/45m/observations/regulations/)、[遠隔観測のビューア](https://www.nro.nao.ac.jp/projects/45m/observations/windows/)（2026-06-23） |
| 観測者が復旧できない障害の報告 | 計算機チーム（日中に復旧する） | Rocket.Chat の #trouble_report | トラブルシューティングのページ（作られているが開けない。下の「一次資料の食い違いと欠け」8） |
| 地震（震度4以上、またはポインティングが大きくずれたとき）の緊急連絡 | 観測所の緊急連絡先 | 電話 | 番号は非公開の観測者向けのページにある（下の「非公開の資料」）。所在は[望遠鏡運用のルール](https://www.nro.nao.ac.jp/projects/45m/observations/regulations/)が示す |
| 野辺山での観測（来所）、三鷹での観測（観測室の予約） | 観測所 | ウェブのフォーム（野辺山は到着の2営業日前まで、三鷹は2週間前まで） | [観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)の「Before Observation」の節 |
| 装置の開発、持ち込み | 開発プログラムの窓口 | メーリングリスト | [野辺山キャンパスを利用した開発プログラム](https://www.nro.nao.ac.jp/projects/developments/)（2026-07-02） |
| 電波天文観測実習 | 観測実習の窓口 | メーリングリスト | [野辺山・電波天文観測実習](https://www.nro.nao.ac.jp/projects/45m/proposals/hands-on-tutorials/)（2026-06-30） |
| VLBI の観測提案 | 水沢 VLBI 観測所 | — | [プロポーザル募集](https://www.nro.nao.ac.jp/projects/45m/proposals/calls/)の「VLBI observations」の節 |

## 段階ごとの資料

### 観測提案を作る

| 資料 | 要点 |
|---|---|
| [プロポーザル募集](https://www.nro.nao.ac.jp/projects/45m/proposals/calls/)（2026-11-17） | 枠と期間、締切、提出の方法と書式、提供する装置とリスクシェアの装置、SAM45 の使えないアレイと YATSUGATAKE、占有期間、注意（自動車のレーダー、OTF のダンプ時間、FOREST の回転角）。観測の補助者は付かず、観測者がウェブで学ぶ前提。経験者を共同研究者に入れることを強く勧め、経験者のいないチームは平日日中の割り当てか練習の時間を求められる |
| [観測計画の立案方法](https://www.nro.nao.ac.jp/projects/45m/proposals/how2plan/)（2026-07-01） | 観測できる仰角（11〜80度）、太陽からの離角、スカイライン、LST の範囲、雑音の見積もり。日本語化の途中 |
| [積分時間の見積もり（Time Estimator）](https://www.nro.nao.ac.jp/projects/45m/proposals/time-estimator/)（2026-06-30） | ポジションスイッチと OTF の見積もりの計算ページと、その使い方。見積もりの結果は提案に貼る |
| [45m 望遠鏡の装置情報（Status Report）](https://www.nro.nao.ac.jp/projects/45m/datasheets/)（2026-07-01） | 今季の装置の能力の表、ビームサイズと能率、ポインティングの精度と頻度の目安、受信機と分光計のページへの入口。HINOTORI-TZ と 7BEE はリンク先のページがない（下の 6） |
| [採択されたプロポーザル](https://www.nro.nao.ac.jp/projects/45m/proposals/accepteds/) | 経験のある観測者を探す手がかりとして、プロポーザル募集が勧めている |
| [友達紹介制度](https://www.nro.nao.ac.jp/projects/45m/proposals/refer-a-friend/)、[CSV 観測貢献プログラム](https://www.nro.nao.ac.jp/projects/45m/proposals/csv-contributors/) | 無料の枠 |
| 料金、利用要領、運用のルール、免責同意 | 所在は[使命](../mission/README.md)の「観測所の利用の決まり」の節にある。失った時間の扱いは下の「トラブルに対処する」 |

### 採択から観測日まで

| 資料 | 要点 |
|---|---|
| [観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)（2026-07-02） | 採択後の流れ。利用料の支払い → 観測用アカウント（観測の2週間前までに PI にメールで届く。VPN と共通で、期限は観測シーズン後の6月末） → 観測の場所の選択と事前の申し込み → 観測指示書の作成。初めての観測者には野辺山での観測を勧める。大学などからの観測はリスクシェアで、毎年の接続試験が要る。ネットワークの切断で失った時間は補償しない |
| [nobs](https://www.nro.nao.ac.jp/projects/45m/observations/nobs/)（2026-06-30） | 観測指示書の作成ソフトの使い方。各タブの説明のページへの入口。台帳は nro-user-tools の `tool-obs-script` |
| [7BEE による観測指示書の作り方](https://www.nro.nao.ac.jp/projects/7bee/7bee-obsfile/)（2026-10-27） | nobs は 7BEE に対応していないため、FOREST の指示書を変換スクリプトで書き換える |
| [便利ツール](https://www.nro.nao.ac.jp/projects/45m/observations/manuals-2/)（2026-06-24） | 天体の仰角と回転角の確認、指示書の観測点の確認 |

### 観測する

| 資料 | 要点 |
|---|---|
| [遠隔観測のビューア](https://www.nro.nao.ac.jp/projects/45m/observations/windows/)（2026-06-23） | 4つのビューアと、それぞれにある画面。前の観測者が終えたことを Rocket.Chat で確かめてから、望遠鏡の優先権を取る |
| [受信機チューニング](https://www.nro.nao.ac.jp/projects/45m/observations/tunings/)（2026-06-30） | H22、H40、Z45 はチューニング不要。FOREST の手順。7BEE、HINOTORI-TZ、eQ は記載がない（下の 3） |
| [強度較正（Intensity Calibration）](https://www.nro.nao.ac.jp/projects/45m/observations/calibrations/)（2026-06-30） | 標準天体の観測を1日1回以上行うことを強く勧める。その方法 |
| [45m 望遠鏡の装置情報](https://www.nro.nao.ac.jp/projects/45m/datasheets/)の「Pointing Accuracy and Strategy」 | ポインティングは 1〜1.5 時間ごと（日の出と日の入りは30分ごと）。ポインティング天体の一覧。風速 4 m/s 未満で約3秒角の精度 |
| [望遠鏡運用のルール](https://www.nro.nao.ac.jp/projects/45m/observations/regulations/)（2026-06-23） | 中断の基準と手順：強風（最大風速 20 m/s 以上で中止し、30分は再開しない）、降雪（中止し、所員が許可するまで再開しない）、ギアの凍結のおそれ、地震。観測の終了時のアンテナの格納 |
| [観測ログ](https://www.nro.nao.ac.jp/projects/45m/observations/logs/)（2026-06-30） | 観測ログとポインティングのログの取り出し方 |

### トラブルに対処する

| 資料 | 要点 |
|---|---|
| トラブルシューティング（2026-06-30 に更新。ただし開けない。下の 8） | SAM45 のエラー、IF 系のエラーの対処の段階。どれでも直らなければその日の観測はあきらめ、#trouble_report に報告する。サイトの API からは本文を読めたが、ページは 404 で、観測準備のページからのリンクもない |
| [NRO45m 障害情報](https://www.nro.nao.ac.jp/projects/45m/projects-45m-trouble/)（2026-11-13） | Trouble ID ごとの原因、影響、現在の状態。台帳の `sources` が引く Trouble ID の正本 |
| 失った時間の扱い | 天候、災害、装置のトラブルで観測できなくても、原則として補償しない（利用要領 第10。所在は[使命](../mission/README.md)）。ネットワークの切断は、天文台側が原因のとき以外は補償しない（[観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)）。リスクシェアの装置の故障で失った時間は補償しない。YATSUGATAKE の問題で SAM45 の代わりのアレイが使えなかったときは、影響を受けた時間の4分の1を補償する（[プロポーザル募集](https://www.nro.nao.ac.jp/projects/45m/proposals/calls/)） |

### データを取得する

| 資料 | 要点 |
|---|---|
| [観測データ](https://www.nro.nao.ac.jp/projects/45m/data/)（2026-06-30） | 取得の方法は計算機のページにあり、所内のネットワークか VPN からだけ読める。データの量の目安。占有期間の後は Nobeyama 45m Science Data Archive で公開。占有期間の長さは資料によって違う（下の 2） |
| [Nobeyama 45m Science Data Archive](https://nobeyama-archive.nao.ac.jp/user/index.html) | 電波アーカイブの入口。台帳は nro-data の `db-radio-archive` |
| [Data releases](https://www.nro.nao.ac.jp/projects/45m/data/releases/)、[野辺山レガシープロジェクト](https://www.nro.nao.ac.jp/projects/45m/data/legacies/) | 公開済みのデータ |

### データを解析する

| 資料 | 要点 |
|---|---|
| [PSW データリダクション](https://www.nro.nao.ac.jp/projects/45m/data/psw/)（2026-06-30） | NEWSTAR のマニュアル。台帳は nro-user-tools の `tool-newstar` |
| [OTF データリダクション](https://www.nro.nao.ac.jp/projects/45m/data/otf/)（2026-06-30） | NOSTAR と CASA による OTF のデータの処理。台帳は `tool-nostar`、`tool-casa-export` |
| [OTF マニュアル](https://www.nro.nao.ac.jp/projects/45m/observations/otf-manuals/)（2026-06-29） | OTF の観測の原理、スキャンのパターンと観測のパラメータ |

### 観測を学ぶ

| 資料 | 要点 |
|---|---|
| [野辺山・電波天文観測実習](https://www.nro.nao.ac.jp/projects/45m/proposals/hands-on-tutorials/)（2026-06-30） | 3つのプログラム（観測所の主催、研究室向けの無料と有料）。観測所の主催の実習は2026年度は行わない |
| 外部評価2023 の指摘 | 訓練の手順と資料を整えるよう求めている（[経緯](../history/README.md)） |

## 非公開の資料（所在だけ）

| 資料 | 正本の場所 | 公開側の入口 |
|---|---|---|
| リモート観測のマニュアル（三鷹から、大学などから）、緊急連絡先（For Remote Observers）、データの取得の方法、VPN の接続の手順 | 計算機グループの計算機とネットワークのシステムのページ（所内のネットワークか VPN からだけ読める） | [観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)、[観測データ](https://www.nro.nao.ac.jp/projects/45m/data/)、[望遠鏡運用のルール](https://www.nro.nao.ac.jp/projects/45m/observations/regulations/) |
| 降雪のモニター | 同上（VPN か所内から） | [望遠鏡運用のルール](https://www.nro.nao.ac.jp/projects/45m/observations/regulations/) |

区分と非公開の理由は[非公開の一覧](../policy/non-public.md)にあります。

## 一次資料の食い違いと欠け

2026-11-19 にウェブサイトを読んで気づいた点です。直すのはウェブサイトの担当です。直ったら、ここから消します。

1. **計算機チームの宛先がない。** [観測準備](https://www.nro.nao.ac.jp/projects/45m/observations/)は、リモート観測の準備や指示書の作成で困ったら計算機チームに連絡するよう繰り返し求めるが、宛先がない。宛先とみられるメールアドレスは、[PSW データリダクション](https://www.nro.nao.ac.jp/projects/45m/data/psw/)のページに編集用のメモの形で残っているだけ。
2. **占有期間が資料によって違う。** [観測データ](https://www.nro.nao.ac.jp/projects/45m/data/)は「全観測の終了から18か月」。[プロポーザル募集](https://www.nro.nao.ac.jp/projects/45m/proposals/calls/)は有料の望遠鏡時間について「各プロジェクトの全観測の終了から3年」。利用要領の第7は「データの取得後3年間」。
3. **受信機チューニングのページが古い。** 7BEE、HINOTORI-TZ、eQ の記載がない。観測の補助者（assistant）に指示書を渡すという、いまはない運用の記述が残る。リンク先の観測の流れ図のページ（/projects/45m/observations/manuals/）は 404。
4. **ヘルプデスクのフォームが開けない。** [CSV 観測貢献プログラム](https://www.nro.nao.ac.jp/projects/45m/proposals/csv-contributors/)と [FOREST](https://www.nro.nao.ac.jp/projects/forest/) のページが、旧サイトのフォームを窓口としているが、403 になる。
5. **編集用のメモが公開されたまま。** 「==ここに画像==」などが、遠隔観測のビューア、受信機チューニング、nobs、観測ログ、便利ツールなどのページに残る。画像のない手順のページがある。
6. **リスクシェアの装置のページがない。** 装置情報の HINOTORI-TZ と 7BEE はリンクがなく、[7BEE](https://www.nro.nao.ac.jp/projects/7bee/) のページは準備中。[7BEE による観測指示書の作り方](https://www.nro.nao.ac.jp/projects/7bee/7bee-obsfile/)は、作成の手順の参照先を資料の名前だけで示し、リンクがない。
7. **公開資料に書かれていないこと。** 強風、降雪、凍結、地震以外の天候（雲、雨、大気の状態）で観測を続けるかの判断の基準。OTF のマップの縞やベースラインのうねりへの対処。観測シーズンの期間の一覧（募集は期ごとの期間だけを書く）。
8. **トラブルシューティングのページが開けない。** ページ（/projects/45m/observations/トラブルシューティング/、2026-06-30 に更新）はサイトの中に作られているが、開くと 404 になり、どこからもリンクされていない。SAM45 と IF 系のエラーの対処、障害報告の経路（#trouble_report）は、このページにしか書かれていない。日本語の URL のままで、英語の URL への付け替えが済んでいない可能性がある（推測）。
