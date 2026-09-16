# Grok Bot Galaxy Day 1 — セグメント05 厚めノート（4:00:00–5:00:00）

- **範囲**: ストリーム時刻 4:00:00–5:00:00（クリップ 0:00＝ストリーム 4:00:00）。実尺約3647秒。
- **音声**: `/workspace/recap-audio-v2/clips/seg05.mp4` 成功（HLS fetch_range 14400–18000）
- **字幕**: `/workspace/recap-audio-v2/seg05/seg05.vtt`（faster-whisper tiny / en、10分WAVチャンク結合）成功 ※OpenAI whisper は他エージェントとCPU競合で極端に遅かったため同一 tiny モデルの faster-whisper に切替
- **画面**: ステージ「Grok Bot for Engineering」（発表者 Lynxie）続き → Introducing Grok Bot 4柱 → ユースケース → ライブデモ（Linga's Engineer Bot／Steve／Jenny／Craig／FlyLo fleet／Routines）→ スタジオ復帰（Matt／Lauren の potato／Thursday 構築）
- **注**: Whisper は Grok Bot を grock／graph／grab／scrap／Gropa 等と誤認。画面スライド **Introducing Grok Bot**／アプリ名 **Grok Bot** に合わせて正規化。Versel→**Vercel**、Flylow／FlyLo→画面・文脈の **FlyLo**／flyair.ai。発明発話なし。不明は聞き取り不明。

---

## 4:00–4:02｜Introducing Grok Bot① Cursor Cloud Agents 一次統合・ツール／MCP

- **[~4:00:00]** 前時間からの続き: **最大の強みは Cursor cloud agents とのファーストパーティ統合**。トランスクリプト読取・cloud agent 起動・プライベートワーカー（自分の Mac など）起動までツール経由。
- **[~4:00:18]** Cursor ウィンドウでできることは Grok Bot がツールで代行。UI を手動でデバッグ操作して agent を起こす必要が減る。
- **[~4:00:35]** 進行中／完了の cloud agent 作業を検査可能。例: 完了後に「証明」（スクショ、前後パフォーマンス比較など）が足りなければ **フォローアップ返信**を自動作成し、自分がPC前にいなくても継続。
- **[~4:01:28]** 第二柱: **日常ツール接続**。例: エンジニアが Vercel（音声: Versel）へデプロイするなら **Vercel MCP**。ローカル agent に繋ぐだけでなく、**24/7** でビルド失敗シグナルを見て修復開始、指定時刻（例: 翌朝6時）デプロイも可能。

---

## 4:02–4:04｜② Memories & Routines・③ なぜ Grok Bot か（他製品比較）

- **[~4:02:25]** **Memories & Routines** が大きなアンロック（継続学習より前進、と）。長期に選好を保持。**名前付き Grok Bot**ごと別メモリ → 無関係メモリで溢れない。
- **[~4:03:00]** 一度伝えた改善方針を次回の cloud agent／レビューに自動適用。繰り返し説明が不要。
- **[~4:03:36]** なぜ必要か: OpenClaw／Hermes 等（音声）はエンジニアリングまで弱い — **Grok Bot／Cursor 一次統合が無い**ため、と。
- **画面**: 「Introducing Grok Bot」4ボックス — Fully Autonomous／Connect to tools (MCP: Jira Notion Figma Slack)／Manage Cursor Cloud Agents／Memory & Routines。

---

## 4:04–4:06｜差別化: 常時稼働PC不要・全プラットフォーム・Computer use・一次統合再強調

- **[~4:04:01]** (1) **カフェインでノートPCを起こし続けなくてよい**。Grok Bot は自前コンピュータ。送信後はノートを閉じてよい。
- **[~4:04:43]** (2) **全プラットフォーム**: 最近 iPad／Android 出荷、既存 iOS／Windows／Linux／macOS。例: Golden Gate Park の芝生で横になりつつ bot が作業（音声: golden gay park）。
- **[~4:05:08]** (3) **必要時にコンピュータを操作できる**。他製品はログイン／クリックが要る局面で人間依存・トランスクリプト観察のみ。Grok Bot はモバイル／デスクトップからリモートPCを直接クリック（パスワードを渡したくないログイン等）。
- **[~4:06:02]** (4) **Cursor cloud agent 一次統合**の再確認 — Cursor UI でできることのほぼ全てが Grok Bot 経由でも可能、と。

---

## 4:06–4:11｜ユースケースA: 不在時に完了・Slack監視・境界設定

- **[~4:06:35]** 「Away でも進める」: 睡眠中／フライト中に唯一のコードオーナーが必要なとき、bot が Slack を監視し基準に沿ってアンブロック／レビュー／ACK。
- **[~4:07:33]** 監督が要る件はスマホで確認 → Grok Bot に approve → 相手へ通知。
- **[~4:07:54]** メンション以外の一般 Slack も監視し、レビュー基準（スクショ必須、本物のテスト等）を適用する方向。
- **[~4:08:37]** リポジトリ内 **skill** 実行にも言及（音声ゆれあり）。
- **[~4:10:28]** プロダクト境界: bot は親切で何でも受け入れがち → **何をすべき／すべきでない＋理由**を明示。メモリが将来判断に適用され、毎回「シンプルに」等を繰り返さなくてよい。
- **[~4:11:12]** 認証で詰まったとき、人間が短時間でアンブロックできる体験が重要、と。

---

## 4:11–4:16｜ユースケースB: Nightly code cleanup／TestFlight／CI赤の自動修復

- **[~4:11:29]** Marketplace にもあるお気に入り: **nightly code cleanup**。エージェント出荷の「slop」掃除を夜間（コンフリクト少・低リスク）に。冗長コメント圧縮・モジュール化など。証明付きなら cloud agent にマージ条件を委ねうる。
- **[~4:12:35]** 実セットアップ例: **毎朝3時**にリサーチ cloud agent が monorepo 横断で品質・モジュール化・コメント・セキュリティ監査。起床時に PR セットが揃う。
- **[~4:13:22]** 内部ツール: TestFlight 招待 — Slack で bot をメンション＋メール → webhook／routine で追加。安全な TestFlight アクセス＋ワンプロンプト。
- **[~4:14:54]** **Auto-fix everything**: CI 赤で毎回 on-call を叩かず、bot が調査→cloud agent 修復→マージ判断指示。デプロイ失敗・フレーキー・アラートもフック。**約10分未解決なら on-call**。多くの場合 Grok Bot が10分以内、と。

---

## 4:16–4:18｜ボット編成: 複数 Engineer Bot・Chief of Staff・メモリ分離

- **[~4:16:17]** ボット編成紹介。1体 vs 複数の議論。
- **[~4:16:44]** **Engineer bot を3体**にする理由: 同じモデルでもタスクはできるが、**コンテキストと艦隊管理**が違う。パイプライン／コンテキスト上限が別 → 分離してメモリを専門化（例: Hogan への指示は Hogan メモリに残る）。
- **[~4:17:45]** 個人 bot に全部話しかけなくてよい。**Chief of Staff** が誰が何をしているか把握してルーティング。CoS は詳細エンジニアリング手順を全部覚えなくてよい。

---

## 4:18–4:22｜ライブデモ① Marketplace から Engineer／Nightly Audit・ボット同士オンボード

- **[~4:18:12]** ライブデモ開始（本人も初回セットアップ気味）。Marketplace から **Linga's Engineer Bot**（音声: link she's engineered）を取得、リポ／Notion 接続済み。
- **[~4:18:35]** **Nightly Audit Engineer** も Marketplace（Grok Bot チーム）から。オンボード自動開始だが、既存ワークフロー文脈は無い。
- **[~4:19:16]** 人間が手順を再説明せず、**既存 Engineer bot に新メンバー（Nightly）をオンボードさせる**。
- **[~4:20:00]** Craig（音声ゆれ: correct）が **Steve** にクリーン定義・ステージ梯子・パイプライン要件をメッセージ。Steve がメモリに吸収。ボット間確認のみで人間は「confirmed」報告を受ける。
- **[~4:20:53]** 通常は午前4時の nightly を、デモのため今すぐ Steve に開始指示。
- **画面**: Linga's Engineer Bot チャット、FlyLo Engineering Fleet、PR #72 Trust polish、Nightly Audit→Steve リネーム指示など。

---

## 4:21–4:29｜ライブデモ② P0（flyair）・Jenny＝Ops／Playbook・P0定義と Routines

- **[~4:21:43]** 緊急: **FlyLo／flyair** 系で過去予約確認できない問題報告 → bot に急ぎ対応させるデモ。
- **[~4:23:51]** 「urgently」を毎回言いたくない → 自律の要点は繰り返し禁止。CoS に **Jenny**（Head of Operations）をオンボードし、**engineering playbook** を Notion 等で管理・更新させる。
- **[~4:26:28]** 「urgently」の意味を定義し直す必要 — 長時間 horizon で迷走する coding agent 対策。
- **[~4:27:38]** **P0 定義**: Grok Bot が cloud agent を**5分ごと**監視し、長スリープやゴール逸脱なら割り込み・新プロンプト。人間はプロンプトを書かず **P0 の定義だけ**書く。
- **画面**: Routines（Fleet watcher 30秒、Trip lookup 5分）、P0-101、Craig／Steve／Jenny サイドバー。

---

## 4:29–4:35｜ライブデモ③ Playbook 共有・証明付きPR・Fleet DB

- **[~4:31:26]** Jenny が全 engineer bot にアナウンス。ボット同士の会話が主で、人間は EM／メンター視点。
- **[~4:32:55]** Jenny→他ボット＋Craig へ playbook 更新（P0 urgent が standing ops）。
- **[~4:33:12]** PR に **proof**（UI ならスクショ、perf ならメトリクス）必須を playbook へ。Craig＝事実上の head of eng。クラウド agent 本体より**結果と証明**を見る運用。
- **[~4:34:17]** Steve が cleanup PR を用意 — チャット中も既存タスク継続（人間のマルチタスクに近い）。
- **[~4:35:08]** 例: 約20 cloud agent 管理時、全状態をコンテキストに載せず **DB／ボードを都度参照**して次タスクを取る。

---

## 4:35–4:43｜デモ締め〜スタジオ切替（AV）

- **[~4:35後半–4:42]** デモ続き／まとめ（一部 Whisper ゆれ大）。ステージ側のエンジニアリング・ワークショップパートが終わり、AV 切替でスタジオへ戻る流れ。
- **画面**: ステージ単写や切替フレーム（`t043600_stage_talk.jpg` 等）。

---

## 4:43–4:46｜スタジオ復帰・Thursday／shipbythursday・Dr. Eggbot・PR→Slack automation

- **[~4:43:04]** ホスト: レストラン事業構築中、自分は CEO 役。リポは主に **ship by Thursday／Thursday**（会社用）など。ドメインあり、Grok Bot からアクセス可。
- **[~4:43:58]** 作成中 bot: **Prioritizer**、**Operator Research**（Cody 対話を受け、類似 pop-up 事業者リサーチ — Flower and Water 等の良い店も）。
- **[~4:44:36]** bot 作成は Marketplace の **Dr. Eggbot**（Lauren 作・bot factory）。AV を Lauren 画面へ。
- **[~4:45:15]** Lauren: Slack に **#pr-reviews**。自分／bot が PR リンク投稿 → 剛セットの **Cursor automation**（現状は簡易プロンプト）がレビュー。**Piece Stack**（音声: pieceknack）で correctness／risk／missing tests 等を見る想定、これから反復。

---

## 4:46–4:52｜Verification skill・Tater／Steve・lander 並行

- **[~4:46:55]** Lauren: 検証（verification）が bot 活用の鍵。アプリ実行・トレース・ヒープ等を bot 自身が回せるようにしないと「あなたがクリックして結果教えて」往復で遅い。
- **[~4:47:56]** Steve に Piece Stack の **create verification skill** を依頼 → **Tater** に委任。status 確認しつつ待つ。
- **[~4:48:31]** 並行でホスト側: lander デザイン磨き（make design／interfaces feel better 系 skill、ミニマル優先）。Lauren のプロトタイプをプロ寄せし、ウェイトリスト系と接続予定。画面共有の AV トラブルありつつ再開。

---

## 4:50–5:00｜Verification の中身・ウェイトリスト／Resend・PlanetScale・UI方針

- **[~4:50:00]** Verification skill の二要素（経験則）: (1) 再現可能な **CLI／標準ツール**（毎回その場スクリプトはトークン浪費・ボットごとバラバラ）(2) **feature map**（機能名・到達方法・ショートカット等 — 今は機能が少ないが将来用）。
- **[~4:51:40]** ホスト: ウェイトリストはメール収集が当面必要。**Loops** も好きだがまず **Resend** が簡単、Thursday リポに Resend プラグインあり、とエージェント指示。
- **[~4:52:33]** ドメイン接続済み。提出フォームは試作で throwaway — 視聴者に「まだ本提出しないで」と。PlanetScale で裏を見る話。DB／収集項目は未整理と自己ツッコミ。
- **[~4:53:37]** UI を大幅にミニマル化。主目的: pop-up 参加希望の**ゲスト email**、右上にレストラン／提供者向け導線。予約・ゲスト情報を主に収集。
- **[~4:54後半–4:59]** イベント／体験の他フィールドや次タスクの雑談・実装指示が続く（Whisper 末尾は断片多め）。クリップは約 4:59:45 でほぼ時間切れ。

---

## 画面メモ（スクリーンショット参照）

| おおよそ時刻 | ファイル例 | 見えるもの |
|---|---|---|
| 4:00–4:06 | `t040030_introducing_grok_bot_slide.jpg` … | **Introducing Grok Bot** 4柱スライド＋発表者インセット |
| 4:06–4:16 | `t040600_presenter_stage.jpg` 等 | ステージ発表者（ユースケース解説） |
| 4:18–4:35 | `t042000_linga_engineer_bot_chat.jpg`, `t042800_p0_flyair_bug.jpg`, `t043000_trip_lookup_routine.jpg` | Grok Bot UI デモ（Engineer Bot／Steve／Jenny／Routines／P0） |
| 4:36–4:43 | `t043600_stage_talk.jpg`, `t044000_presenter_stage_wide.jpg` | ステージ締め〜切替 |
| 4:43–5:00 | `t044800_founding_eng_lander.jpg`, `t045000_grok_bot_desktop_agents.jpg`, `t045800_steve_tater_hashbrown.jpg` | スタジオ／Grok Bot デスクトップ（Founding Eng, dr eggbot, tater, hashbrown, steve） |

---

## この時間の要約（親エージェント向け）

1. **ステージ（Lynxie）**: AI Maturity の頂点としての Grok Bot — Cloud Agents 一次統合、MCP/ツール、Memories&Routines、自前PC＋全OS＋computer use。Away時Slack、nightly cleanup、TestFlight、CI自動修復。複数 engineer＋CoS でコンテキスト分離。
2. **ライブデモ**: Marketplace の Engineer／Nightly Audit をボット同士オンボード（Craig→Steve）。FlyLo P0、Jenny＝Ops＋playbook、P0＝5分監視 routine、証明付きPR、fleet board／DB。
3. **スタジオ（〜4:43–5:00）**: Thursday／shipbythursday、Prioritizer／Operator Research、**Dr. Eggbot**。Lauren: #pr-reviews＋Cursor automation＋Piece Stack、**verification skill**（CLI＋feature map）を Tater 経由。lander／ウェイトリスト（Resend・PlanetScale）、ミニマルUIでゲスト email＋提供者導線。
4. **ブロッカー**: HLS／画面は成功。初回 OpenAI whisper は他ジョブとCPU競合でほぼ停滞 → **faster-whisper tiny** で同一内容の字幕を生成（パスは指定どおり `seg05.vtt`）。一部デモ中盤・末尾は Whisper ゆれ強め（画面で補完）。X 投稿なし。
