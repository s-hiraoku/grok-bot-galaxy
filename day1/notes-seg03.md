# Grok Bot Galaxy Day 1 — セグメント03 厚めノート（2:00:00–3:00:00）

- **範囲**: ストリーム時刻 2:00:00–3:00:00（クリップ 0:00＝ストリーム 2:00:00）
- **音声**: `/workspace/recap-audio-v2/clips/seg03.mp4`（約3600秒）成功
- **字幕**: `/workspace/recap-audio-v2/seg03/seg03.vtt`（Whisper tiny / en）成功
- **画面**: スタジオ4人（Matt / Motion / Lauren + ゲスト Peter Yang → 後半 Cody）＋ Grok Bot 画面共有（steve / Dr. Eggbot / Grokpot / Tater 等）＋チャット
- **注**: Whisper は Grok Bot を Rockbot / Gratbot / Grockbot / Grogpot / graph 等と誤認しやすい。画面・文脈に合わせて **Grok Bot** に正規化。**Grokpot** はプロトタイピング用ボット名として残す。Versel→**Vercel**、Plan at scale→**PlanetScale**、pigsfield→聞き取り不明（AI動画ツール）。不明箇所は「聞き取り不明」。発明した発話はなし。

---

## 2:00–2:04｜方向合わせ：レストラン／Pop-up vs 対面ビジネス案

- **[~2:00:00]** Lauren 側: Steve が call-for-ideas を整理。他案もあるが、**レストラン／Pop-up**でプロト開始したい。Motion が大量ワークフローを回すなら別、とも。
- **[~2:00:30]** Motion: 対面ビジネス案でフィルタ。ポテト／チップス／フライ系レストランのリサーチも冗談交じりに提案。
- **[~2:00:48]** 分業: **prospecting（見込み開拓）** と **building（構築）**。Divide and conquer。
- **[~2:01:00]** デザイナー bot を入れ、プロトをレビューさせる案。Lauren はデザイン bot を探す。
- **[~2:01:12]** チャット視聴者のボットを雇う案。Lauren のサイドバーは寂しい: X プラグイン bot、**Steve**（メイン／デフォルト）、**Dr. Eggbot**（剛導入）。
- **[~2:01:36]** Steve の対面会社案: paint shop、local service、**piano tuning**、AI＋建設／trades、billboard／屋外サイン。3日では難しいもの: hardware、recycling、festival 系、robotaxi 等。
- **[~2:02:22]** 合意: **pop-up idea**（プラットフォーム）に寄せる。GitHub・Notion は空。Lauren がビジョンのシェルをプロト。

---

## 2:03–2:08｜Dictation→ランディング・Prospecting bot・Steve＝CoS

- **[~2:02:46]** Lauren: **dictation（音声入力）**で方針を Steve に流し込む。「pop-up platform startup」を口頭で定義。
- **[~2:03:17]** Dr. Eggbot と小さなエンジニアリングチームで、loose／scrappy な検証プロト。最初は DB 不要 → **Google Sheet** でも可。
- **[~2:03:51]** まず **landing page**＋サインアップ。ノイズ交じりの口述を編集しつつ Steve に「pop-up 用 LP を作れ」と依頼。
- **[~2:04:35]** Motion（並行）: Dr. Eggbot 導入。「**prospecting bot** が必要」と口述 — レストラン pop-up の実現可能性調査、店と来客の両方を探す。ソースは X／視聴者の知人シェフ、提出用サイト、電話・メール等。
- **[~2:05:38]** Dr. Eggbot が prospecting bot 作成中。画面に作成中ボット一覧。チャットでも追える、と案内。
- **[~2:05:56]** Steve はテンプレではなく**デフォルト bot**。Dr. Eggbot の強み: 既存ボットを横断して**改変**できる。
- **[~2:06:15]** Lauren: Dr. Eggbot に「Steve を **chief of staff / executive assistant** に」依頼。ボットごとに文脈を持たせ専門化、チーム協業。普段は Steve 経由で話す想定。
- **[~2:06:58]** 同時に「プロトタイプ bot を作れ」— loose な **vanilla HTML/CSS**、楽しいフード系の名前。
- **[~2:07:24]** Motion: 公開 GitHub リポ作成（音声: very vocal pop up → 画面文脈 **popup**）。ライブ後に PR 整理。Dr. Eggbot は must-have、と複数人。

---

## 2:08–2:12｜Chat-first・Potato Lab・Grokpot 命名・Prioritizer

- **[~2:07:59]** チャット: Dr. Eggbot は自分でインストール可？ → **Marketplace** で追加可能（Grok Bot 内で前面表示）。
- **[~2:08:08]** 「名前が気に入らない」→ **話すだけで全部変えられる**（chat-first／malleable）。Steve に新プロト名を尋ねさせるデモ。
- **[~2:08:38]** Motion: チャネル設計 — シェフ／スペース連絡手段、スペース調査、メール。会社メール未整備。**社名→ドメイン→メール**の順。
- **[~2:09:19]** 社名案 **Potato Lab**（フード文脈）。SF のレストラン pop-up、「pop-up as a service」。Grok Bot で空きドメインも調べる案。
- **[~2:09:42]** Lauren: プロト bot 名候補をチャット投票 — Pickle / waffle / dumpling / meatball 等。**Potato** 票多数。**Grokpot** が好評 → 採用方向。
- **[~2:10:29]** どんな restaurantier が pop-up 向きか — オープン。Grokpot／ボットに聞く。
- **[~2:10:38]** Motion: Dr. Eggbot で **Prioritizer（優先順位 bot）** 作成中。配信・来客・思考が多すぎるので、AI に「頭の中を整理・減速」させる使い方。
- **[~2:11:00]** ボット提案例: ideal restaurantier brief、出荷スパイク、リードマップ、outreach、ゲスト獲得パス。
- **[~2:11:26]** Lauren: Grokpot 起動に不具合気味だが自力で続行。プロト前に**良質な LP デザイン参照**を集め、ほぼ mood board を組む。

---

## 2:12–2:19｜Dogfood・二系統LP・口述プロンプト・デザイン3方向

- **[~2:12:10]** Motion: デザイン bot 準備済み。LP は「特定店」か「レストラン登録」か。
- **[~2:12:25]** Lauren: プラットフォーム構築だが、**自社でも pop-up を運営して dogfood** したい。Motion: 野心的だが「好きな会社は野心的」。ピボットもありうる。
- **[~2:13:07]** Grokpot が LP ギャラリー候補を提示。方向を数個選んで進める。
- **[~2:13:34]** Lauren が Steve へ長い stream-of-consciousness: pop-up プラットフォーム＋自社 dogfood → **LP は複数面**（プラットフォーム／オペレーター向け、自社イベント向け、来客向け）。料理内容は未定。まずは場所・作り手・来客の接続。全部のソフトを先に作らず、メール収集など**手動から**でもよい。
- **[~2:15:20]** プロンプト技: マイクで数分しゃべったあと「自分の言葉で言い直せ」と確認させる。Steve の要約: 都市でフード pop-up を立ち上げるソフトウェア＋ops；自社でも同じスタックで運営；メガ1ページではなく複数の公開面。
- **[~2:16:59]** Steve の助言: ボトルネックは LP 乱造ではなく **first loop** — 場所・オペレーター／作り手、来客はその後。
- **[~2:17:23]** Motion: そのループ用ソフトが会社になる。テーブル予約前提 vs カウンター／並びの低リフト案。Lauren: シェフ＋倉庫＋体験型イベント寄りも検討中だが、フライ売りカウンターの方が予約不要で楽、とも。
- **[~2:18:46]** 早期プロトをデプロイしてネット上に出す瞬間が欲しい。**3方向**のデザイン案（暗いプロダクト風／コーポレート寄り／もう1つ）。Grok Bot 内で HTML/CSS をそのまま描画 — 外部デプロイ不要。フィードバックで調整へ。

---

## 2:19–2:24｜Peter Yang 助言・プロアクティブ化・マルチプレイ要望・退席

- **[~2:19:40]** Motion→Peter: ソロプレナーへの良い助言は？
- **[~2:19:53]** Peter: **自分が楽しいことを増やす設計**にせよ。儲けるが嫌いな仕事ばかりだと起業の意味が薄れる。
- **[~2:20:17]** アイデア選び: PM 時代の長い社内議論・文書より、**できるだけ早く市場／顧客に当てる**。口では良いと言っても実際に**払うか**で見る。アイデアは安い、チームが重要。
- **[~2:21:21]** 今は誰でも作れるが、**純粋ソフトウェアだけでは稼ぎにくい** — 物理／サービス要素がないと「LP＋DB になぜ金を払う？」になる。**最初の1ドル**まで検証。
- **[~2:22:04]** ハードな仕事（レストラン探し・調理等）には金が払われる、という合意。次のゲスト前にロックイン。
- **[~2:22:20]** Peter への parting: 製品が「人格のある人／チームと話している感じ」で好き。Tips: ボットを**プロアクティブ**に — LP 指標追跡、レストラン prospecting、**週次 cron／スケジュール**で更新を送らせる。番号付きリストで返信しやすい形式。毎週金曜に全ボットがチェックイン。
- **[~2:23:35]** 自動化したい作業を任せ、こちらから聞きに行かずボットが押してくる形へ。
- **[~2:23:47]** Feature request: なぜ Slack？ **人間が Grok Bot 内のチャネルでボットと協働**したい。一人でボットと話すのは寂しい — Lauren や他者とコラボしたい。ホスト: 近日／需要あり、今日は各自が別ボットチームで調理。
- **[~2:24:25]** Peter 退席。「フライを買う」ジョーク。感謝。

---

## 2:24–2:30｜Tater 誕生・Model/Harness・Notion 会社文書・役職ネタ

- **[~2:24:38]** Lauren: Steve にプロトが bland／boring とフィードバック。Grokpot に新プロト依頼。並行で Dr. Eggbot に **correct engineer bot**（本格エンジニア）作成 → プロト用 Grokpot と分離。
- **[~2:25:21]** チャットでエンジニア bot 名 — **Tater(s)** 採用（potato オーバーライド）。
- **[~2:25:48]** 楽しいがデザイン寄りすぎな案も。Motion 解説: **Grok＝モデル**、その上の **harness（実行コード）**。Grok Bot は軽量（coding harness 例: Grok Build 等とは別）。本格コードは **Cursor**（特に **Cursor cloud agents**）へ寄せ、低→高 fidelity へ進化する、と予告。
- **[~2:26:52]** スタック議論。Lauren→Steve→Tater: **Vercel + PlanetScale** を意識（両社からゲスト予定のネタバレ）。他は柔軟。Endless tech debate は避け PMF 優先。
- **[~2:27:46]** Motion: Notion に合意内容を文書化（Lauren は Notion 嫌いだが自分は計画に有用）。暫定社名 **Ship by Thursday**（より良い名が出るまで）。役職: Lauren＝**CTO**、Motion＝**CPO**（Chief Product／ジョークで Chief Potato ではない）、Lauren＝**Chief Potato Officer**、Matt＝**CEO**（grown-up）。
- **[~2:28:47]** やること: SF でフード pop-up をやり、その経験で **pop-up 運営 OS**（メタ製品）を作る。楽しさ＝人を集めること。文脈を短く一貫させ、ゲストにもボットにも同じ説明を渡す。
- **[~2:29:50]** 紙のネームプレート遊び（Chief Potato Officer 等）。次ゲスト準備。チャットが Grok Bot アプリの**アップデート可用**に気づく — 配信中は怖いので休憩で、と。

---

## 2:30–2:38｜ピンクLP選定・Slack/Repo・ドメイン案・Vercel接続・配信トラブル

- **[~2:31:07]** Lauren: プロト色を**ピンク**寄り／night market 方向で即決。細部より速さ。後で Cursor cloud＋デザイナー bot。
- **[~2:31:39]** 数分後にゲスト。その間に cloud agents で FE/BE スタブ、リポにコード。Lauren: 既にリポ作成 → Slack に **popup.git**（聞き取り）共有。Slack 表示名を **Lauren, Chief Potato Officer** に。
- **[~2:32:37]** LP をリポ経由でビルド／ホスト。ドメイン即買いは保留 — まず Vercel テスト、名前確定後にドメイン。
- **[~2:33:10]** マーケ／ブランディング bot 雇用案。CPO がドメイン候補生成。リポにコードが入ればボットが **PR** を出せる、と Motion。
- **[~2:34:09]** ドメイン案一覧（音声）: cleanstall.com、stall.run、nightmarket.app、popup.plates、openstall.co、peanut popup、popetto.com、host the popup.com 等 — しっくり来ない。Notion 会社 doc を共有しボットに文脈投入。
- **[~2:34:53]** Motion: AI への入力は**簡潔で良い情報だけ** — 悪い文脈は悪い出力。
- **[~2:35:30]** Cursor bot を Slack に。Lauren を **Vercel org の owner** に追加。リポは空だが存在。
- **[~2:36:12]** `index.html`（インライン CSS）がリポに — 開始時より前進。Vercel をリポ接続し Deploy。認可作業。
- **[~2:37:21]** Motion: **Ops bot** と **Creative Director** bot 作成中（命名・ハイレベル／オペ実行）。会社運営の地味作業も自動化へ。
- **[~2:38:01]** Vercel 招待メール確認のため画面共有を一時カット要求 → 共有トラブル／「technical difficulty」。別の人がストリーム救済。〜2:39 頃復帰。

---

## 2:39–2:46｜デプロイ成功・Notionサインアップ・PlanetScale・ゲスト欠席

- **[~2:39:21]** デプロイ稼働。main に push で deploy。現状はただの HTML — サインアップ保存先が必要。Google Sheet vs **Notion DB**（Notion MCP あり）。Flat file 案も。
- **[~2:40:17]** Lauren: Vercel 接続完了。Steve に「LP はデプロイ済み → **Notion にサインアップ用 DB** を繋げ」と依頼。
- **[~2:41:44]** 計画修正: **PlanetScale**（Postgres）希望。Payments は後回し。PlanetScale チーム shout-out／数日中にゲストの可能性。
- **[~2:42:47]** 画面共有復旧待ちの口頭リキャップ: Matt＝ops／会社プレイブック；早期 HTML LP；方向＝pop-up 事業／プラットフォーム＋自社運営；DB 統合作業中。
- **[~2:43:50]** ドメイン未決。Creative Director＋チャットに案を募る。**shipbythursday.com** が空いてるか確認。
- **[~2:45:07]** 次ゲストは来られず — ビルド時間が増える。PlanetScale 資格情報待ち。テーブル設計・依存関係でアンブロックを。
- **[~2:45:57]** Vercel／メール招待の続き。Lauren→Steve: **Tater は今後 Cursor cloud agents** を使え、project agent も検討。

---

## 2:46–2:52｜Cursor Cloud Agents 解説・shipbythursday 取得・main直push・BRB

- **[~2:46:42]** Lauren 解説: Grok Bot＝オーケストレーションに強い；**Cursor の harness**＝コーディングに強い。Grok Bot から **cloud agents** を spawn — クラウド VM でアプリ起動・クリック・CPU トレース等。既存リポなら環境セットアップも指示可。
- **[~2:47:58]** Tater に cloud agents／プロジェクト用エージェントを使わせ、長期の技術文脈を保持。PlanetScale 資格待ちの間はローカル or cloud agent マシンで開発し、動画／スクショで報告 → デプロイは後。
- **[~2:49:49]** Motion: **ship by thursday** ドメイン取得済み。会社lander用に配線。製品は別ドメイン。Ship by Thursday＝「会社の会社」。製品の仮タイトルはこれから。
- **[~2:50:27]** Dr. Eggbot で Cursor team kit／skills／**peestack** 等を入れ cloud agents 接続 → 会社lander用コードへ。
- **[~2:51:12]** Steve が PR を開いた → 新ルール: **当面 PR 禁止、main に直接 ship**（誰かに怒られるまで）。巨大 diff は読まない方針。
- **[~2:52:12]** Lauren: Tater に加え **reviewer bot** も Steve 経由で検討。その後 **技術的都合でフル画面カット／BRB**（〜数分の無音・You 等）。

---

## 2:55–3:00｜復帰・ゲスト Cody・ブックローンチ／Pulse・検証助言（途中で区切り）

- **[~2:55:08]** 復帰。会社lander着手、Cursor 上で他エージェントも見える、と。
- **[~2:55:38]** ゲスト **Cody** 参加。ビジネス売買マーケットプレイス＋アドバイザリー；オンライン約 **1500万**フォロワー規模の話（音声どおり）。チームで Grok Bot 利用中。
- **[~2:56:14]** 画面共有: 今週発売の**本のローンチダッシュボード**（〜13.5万ユーザー表示）— Grok 等ミックスで構築、**Vercel** 上。リアルタイム参加者、paid vs organic、チャネル、平均注文単価等。
- **[~2:57:13]** 別画面 **Pulse**: 事業の見方／ピッチ／低利益レバレッジに基づく計画、など AI でライブ構築したツール群の紹介。
- **[~2:57:45]** ホスト: 最大の課題は？ → アイデアはあるが**検証**したい。方向: レストラン pop-up（店とゲスト接続・場所）→ そのプロセスをソフトウェア化し販売。Ops 優先、legal／リース等は後。
- **[~2:58:42]** Cody: 事業を決める前に**3人に売れ**。レストラン pop-up は VC 前提にしない（VC はごく少数）。**Distribution に執着**。配信の数万人は不公平な優位だが、それがなくても考える。Controversy は時に有効 — 自身の「controversial tweets」例（Austin 移住を勧める AI 生成動画等）を見せ始める。
- **[~3:00:00]** セグメント区切り（Cody の distribution／論争ネタ解説の途中）。

---

## 画面メモ（スクリーンショット参照）

| おおよそ時刻 | ファイル例 | 見えるもの |
|---|---|---|
| 2:00–2:05 | `t020005_steve_ideas_dump.jpg`, `t020140_inperson_ideas_list.jpg` | Steve／X スレッド要約、対面ビジネス案リスト |
| 2:03–2:08 | `t020310_popup_platform_dictation.jpg`, `t020440_prospecting_bot_eggbot.jpg`, `t020615_steve_chief_of_staff.jpg` | 口述で LP／prospecting、Dr. Eggbot、Steve＝CoS |
| 2:07–2:11 | `t020740_github_popup_repo.jpg`, `t021020_grokpot_name_poll.jpg` | 公開リポ、名前投票（Grokpot） |
| 2:16–2:19 | `t021620_steve_restates_plan.jpg`, `t021850_design_directions_poll.jpg` | 計画言い直し、LP 3方向ポーリング |
| 2:20–2:24 | `t022000_peter_solopreneur_advice.jpg`, `t022400_peter_goodbye_fries.jpg` | Peter 助言〜退席 |
| 2:25–2:30 | `t022500_tater_engineer_bot.jpg`, `t022730_vercel_planetscale_stack.jpg`, `t022830_notion_company_doc.jpg`, `t022950_chief_potato_nameplate.jpg` | Tater、スタック、Notion、ネームプレート |
| 2:31–2:40 | `t023120_pink_night_market_pick.jpg`, `t023620_vercel_connect_deploy.jpg`, `t023830_stream_glitch_rescue.jpg` | ピンク LP、Vercel、配信トラブル |
| 2:40–2:52 | `t024100_notion_signup_db.jpg`, `t024650_cursor_cloud_agents.jpg`, `t024950_ship_by_thursday_domain.jpg`, `t025240_brb_tech_break.jpg` | Notion DB、cloud agents、ドメイン、BRB |
| 2:55–3:00 | `t025620_cody_guest_join.jpg`, `t025700_book_launch_dashboard.jpg`, `t025930_controversy_distribution.jpg` | Cody、ローンチダッシュボード、distribution 助言 |

---

## この時間の要約（親エージェント向け）

1. **会社アイデア確定寄り**: 対面／非SaaS案を見たうえで **SF フード pop-up ＋ pop-up OS（dogfood）** に収束。分業＝prospecting（Motion）／プロト（Lauren）。
2. **ボットチーム拡張**: Dr. Eggbot、Steve＝chief of staff、**Grokpot**（軽量 HTML プロト）、**Prioritizer**、prospecting、後に **Tater**（エンジニア／Cursor cloud）、Ops／Creative Director、reviewer 検討。
3. **実行インフラ**: 公開 GitHub popup リポ、Notion 会社 doc、**Vercel** に HTML LP デプロイ、サインアップは Notion→**PlanetScale** 志向、**shipbythursday** ドメイン取得、当面 **main 直 push**。
4. **ゲスト**: Peter Yang — 楽しさ設計・早期市場検証・純粋SaaSの難しさ・プロアクティブ cron・人間マルチプレイ要望で退席。〜2:45 次ゲスト欠席。〜2:55 **Cody** — 本ローンチ／Pulse デモ、「3人に売れ」＋ distribution／controversy。3:00 で途中切り。
5. **運用メモ**: 途中 AV／画面共有トラブル（メール隠し・ストリーム救済・BRB）。Whisper ゆれ多めだが画面で Grok Bot／bot 名を確認して正規化済み。
