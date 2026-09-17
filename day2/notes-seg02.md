# Grok Bot Galaxy Day 2 — セグメント02 厚めノート（1:00:00–2:00:00）

- **範囲**: ストリーム時刻 1:00:00–2:00:00（クリップ 0:00＝ストリーム 1:00:00）
- **音声**: `clips/seg02.mp4`（約3600秒）成功・mean ≈ −31 dB
- **字幕**: `seg02/seg02.vtt` / `.txt`（faster-whisper tiny int8）816 cues
- **画面**: Amrita SEデモ続き → 会場Q&A → スタジオ（Matt/Motion/Lauren）ゲームビルド → **1:41–1:48 BRB（技術トラブル）** → Cursor でプロトタイプ再開
- **注**: Grok Bot / peestack / potato mode / Dr. Eggbot / Sherlock / Serena / Mimi は画面・文脈で正規化。xAI。不明は「聞き取り不明」。

---

## 1:00–1:03｜Teach a Task（画面録画でスキル学習）

- **[~1:00:26]** Amrita続き: Sherlock / Serena にタスクを教えられる。Serena は Southwest 予約をコンピュータで継続中。
- **[~1:00:52]** Sherlock の画面をテイクオーバーし、競合の Hub changelog 等で技術ポストを探す手順を教える。
- **[~1:01:00]** **最大のレバーの一つ = ビデオ録画で教える（Teach a task）**。Google を開いて操作を録画→一時停止で完了。
- **[~1:01:41]** 録画からスキル学習完了。Southwest / Spirit / Skyscanner / Google Flights 等へ同じスキル適用可。AI関連ブログを重点監視、とボイスで注釈。
- **[~1:02:48]** スキルは作成したボットに限らず、**マーケットプレイス経由で他ボットも利用**可能。

## 1:03–1:05｜グループチャット協調＆ボット間タグ

- **[~1:03:17]** Sherlock×Serena グループチャット: 管理予約は競合のテーブルステークス、フレキシブル日付カレンダーはFEに既にある／低工数、往復・荷物は大だが低工数ではない、等を議論。
- **[~1:04:14]** ボット同士が **@タグ**で特定ボットに質問できる（人間がタグしてもよい）。

## 1:05–1:08｜ボットがボットを spin up

- **[~1:04:52]** Sherlock（＋Serena）に「競合差別化／SE向けで役立つボットを spin up して」と依頼。
- **[~1:05:47]** **リトルノーン: ボットは他ボットを起動できる**。例: Chief of Staff に日常向け3体（inbox / scheduler / calendar）を作らせる。
- **[~1:06:18]** 初見SE向け: 顧客POCデモ用に「役立つ3体を作って」と頼め、と推奨。

## 1:07–1:12｜Mimi: Salesforce スライド完成 → Grab 追加

- **[~1:07:37]** Mimi: Salesforce ペア作業中。ログイン詰まり → Amrita がコンピュータをテイクオーバーして支援。
- **[~1:08:07]** **2枚のスライド完成**（正しいロゴ、Problem/Solution/Impact/Quote）。所要おおよそ10–15分。
- **[~1:08:47]** 追加: Grab の公開ブログ（Cursor 利用事例）でも同様に依頼。複数顧客を一度に投げても可。
- **[~1:09:23]** Echo 連携イメージ: コール中にスマホから「このスライド隠せ」等。ノートPC不要でケーススタディ量産。
- **[~1:10:50]** 週15–20顧客分のスライドがボトルネックだった仕事をテンプレ＋メモリで加速。公開ブログは Cursor 公式ではなく顧客側投稿をクロール。

## 1:12–1:15｜Spin-up 結果: Battle Card Blair / Demo Drake / AI Radar

- **[~1:12:45]** Sherlock が3体を起動。
- **[~1:12:57]** **Battle Card Blair**: Serena の競合実機調査＋Sherlock のコードベース → SE向けバトルカード（claims / pilot reality 等）。
- **[~1:13:35]** **Demo Drake**: デモ／トークトラック。主張は Sherlock にグラウンド。必要なら Serena / Blair から対比を取得。
- **[~1:14:16]** **AI Radar**: 競合テックブログの AI 記述を追跡。先に教えたスキルを使用。真実源は Sherlock、実機フローは Serena。
- **[~1:14:50]** 社内ジョーク: 「できる？ → Ask Grok Bot」。モデルが **No と言える／押し返す**のも利点、と。

## 1:15–1:24｜Q&A（Captcha・MCP・本番安全・トークン）

- **[~1:15:34]** ラップアップ → 会場Q&A。
- **[~1:16:06]** Q: ボットが他サイトでログインするとBANされないか。A: CAPTCHAで止まるサイトあり。エンタープライズは **ボットPCでサイトブロック**推奨（業務不要な Facebook 等）。
- **[~1:18:37]** Q: Computer use vs MCP。A: 現状 Google Docs 等は MCP の方が速いことが多いが、computer use は高速化見込み。**監視・ガードレールは今は MCP が有利**（whitelist/blacklist）。将来 computer use にもガードが増える想定。
- **[~1:19:50]** Q: 本番変更／マルウェア。A: ハードニング継続中。Skills のルールで本番デプロイ禁止等。Settings の **Auto review** に言及（聞き取りやや不明）。
- **[~1:22:26]** トークン課金: 会話＋コンピュータ使用が消費。**Grok（音声: graphbott 6）**は安価で高効率を狙ったモデル、と。
- **[~1:23:19]** スライド一式のコスト感: **約 $20–30**（手作業なら4–5時間相当）で再利用可能。冗長トークンは「短く話せ」と指示で削減可。

## 1:24–1:33｜スタジオ再開: ランディング＆ peestack / potato mode

- **[~1:24:10]** Lauren オフライン気味 → Matt が break 中の Cloud Agents セットアップを画面共有で説明（「backseat driver」）。
- **[~1:24:44]** **Dr. Eggbot**（エンジニアボット作成役）＋ founding engineer がランディング作業。Lauren の計画ドキュメント／モノレポを共有コンテキストに。
- **[~1:25:03]** Lauren方針: **ゆるいプロト**（ログイン不要・DB不要・ハードコード可）で見た目の遊びを先に。
- **[~1:26:09]** Matt: ランディングが第一ゴール。個人スキル **project planning**（T3 / TanStack / Expo / Vite 等のスキャフォールド嗜好）＋ **make interfaces feel better**（Twitter発のUI磨きスキル）。
- **[~1:27:23]** MVP: Bun ベース lander（create-next-app 系）。OG メタタグ／サイトメタを必ず入れるポリッシュ。
- **[~1:28:08]** Grok Bot が「引き算してから足す」方向へ自己修正 → Cursor Cloud Agent へキック。**slash potato mode** / 「use potato mode」（peestack）。
- **[~1:29:46]** 余談: オープンソースのフラットSVGトークンスライダーでアセット遊び場。Matt はゲームデザイン初心者で調査依頼中。Phaser 経験あり。

## 1:30–1:41｜エンジニアボット指示・ビジュアル遊び場・Bufo・Notion

- **[~1:30:54]** Lauren: Dr. Eggbot（または Chief of Staff **Steve**）経由でインフラ／プロト用エンジニアボットを作成。Steve が資格情報・ゲーム文脈のハブ。
- **[~1:31:43]** エンジニアの仕事: cottages（agents）をオーケストレーション／監督。まず軽量プロトで「遊び感」→本格工は後。永続的に使える設計に。
- **[~1:33:00]** パターン: 大きな指示の後に **「自分の言葉で言い直せ」**（能動的傾聴）。
- **[~1:33:24]** Matt: ビジュアル playground がローカル起動。色に意味を持たせる議論。Lauren: まず最基本プロトを上げて全員がコードベースに入れる方が先。
- **[~1:35:42]** 「**time to fun を短く**」。定数スライダーでメカニクス試験。
- **[~1:37:03]** Founding engineer = Preview to Play。Growth engineer。余興: **Bufo mode** 用 GIF パック（約1200？）を Slack 用に—DevRel あるある。
- **[~1:38:03]** Knowledge base ボットが Notion の会社ドキュメント更新、ピボット記録、GTM、プロダクト計画取り込み。次は AEO/SEO、A/B、広告。
- **[~1:40:04]** 視聴者向け再掲: Day2 ライブでゲームスタジオ＆第1作をビルド中。ホワイトボード図も Notion へ。

## 1:41–1:48｜BRB / 技術トラブル（欠測）

- **[~1:41:27]** 「technical difficulties」「be right back」。
- **[~1:41:27–1:48:10]** **実質 BRB**。この間の詳細発言は字幕にほぼ無し／信頼性低 → **欠測扱い。内容を捏造しない**。

## 1:48–1:52｜復帰: Cursor でゲームプロト（ELO・3人ロスター）

- **[~1:48:10]** Welcome back。72時間でゲームスタジオ＆ゲーム構築、と再掲。PC問題は解消。
- **[~1:48:36]** Lauren: 知識仕事は Grok Bot、深いエンジニアリング反復は **Cursor**。ローカルエージェントを再起動（文脈不足でやり直し）。
- **[~1:49:17]** リポジトリの docs を読ませ「ゲームを自分の言葉で」再掲確認: 短い対戦ループ、ボットの import、**3人ロスター**、相手にはラインナップ秘匿、**ELO** マッチメイキング。
- **[~1:49:49]** ELO は未経験だが Marvel Rivals 等の論文を参考にできる、と。
- **[~1:50:37]** プロトでは **サインイン省略**、ローカル完結・**DB不要**、複数プロト候補、**デバッグパネル（スライダーで定数変更）**。

## 1:52–2:00｜potato mode prototyping / Architect 多モデル / vanilla HTML 設計

- **[~1:52:02]** 「use potato mode prototyping」で peestack のプロト節が効く。
- **[~1:52:18]** ゲームは **楽しいことが最優先**。他は後。スライダーで即リプレイし「楽しいか」を検証。
- **[~1:53:19]** Motion: プロンプト往復なしで MVP をライブ調整できる playground になる、と評価。
- **[~1:54:19]** peestack 思想: user delight、機能は正当化、少なく上手く出す、**HTMLでデザイン決定は安い**。
- **[~1:54:59]** **Architect スキル**: 複数モデル（Fable / Sol / Grok / Composer 等）にアーキ案を競わせマージ。プロト段階ではアーキより速さ優先 → **最初のプロトは Grok** 指定。
- **[~1:57:23]** Cursor 内蔵ブラウザでローカル再生。待ち時間に Subway Surfers ジョーク。
- **[~1:57:51]** Grok 案完成: **vanilla HTML/CSS/JS**、インメモリ、**3 UI バリアント切替**、Marketplace から一覧取得、データ駆動、**状態遷移（ステートマシン）**まで含む長めの設計＋代替案。続きは seg03。

---

## セグメント02 まとめ

| 項目 | 内容 |
|------|------|
| 前半 | Amrita: Teach task / ボット spin-up / Mimi・Sherlock・Serena 協調 |
| Q&A | Captcha、MCP vs computer use、本番安全、トークン/$20–30 |
| 中盤 | スタジオ: potato mode・lander・Dr.Eggbot・Notion |
| BRB | 1:41–1:48 技術トラブル（欠測） |
| 終盤 | Cursor プロト: ELO・3ロスター・デバッグスライダー・vanilla HTML 設計 |
