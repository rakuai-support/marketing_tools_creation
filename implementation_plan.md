# Implementation Plan - Marketing Tools Creation

「かわさき楽AIサポート」のマーケティング活動に寄与するため、見込み顧客（経営者・個人事業主）がサービスのメリットを直感的に理解できる「コスト削減シミュレーター」を作成します。また、このツールを活用するための周知メール案も作成します。

## User Review Required

> [!NOTE]
> このシミュレーターは、ウェブサイト（Wix等）に埋め込み可能なHTML/JSウィジェットとして提供します。実際の運用には、貴社のウェブサイトへの埋め込み作業が必要です。

> [!IMPORTANT]
> シミュレーションに使用する「神奈川県の平均時給」などは、最新のデータ（または貴社の基準）に合わせて調整可能な設計にします。

## Proposed Changes

### Marketing Tools

#### [NEW] [cost_simulator.html](file:///c:/Users/utaka/かわさき楽AIサポート/docs/marketing_tools_creation/cost_simulator.html)
- ユーザーが自身の業務時間と時給を入力し、AI導入による削減見込み額を算出するツール。
- **機能**:
    - 入力項目: 1日あたりの事務作業時間、時給（デフォルト設定あり）、稼働日数。
    - 出力項目: 月間/年間の削減可能コスト、削減可能時間。
    - **[NEW] ご褒美変換機能**: 削減額を「生ビール」「温泉旅行」「高級寿司」「フロンターレ観戦チケット」に換算して表示。
    - **[NEW] アニメーション**: 結果表示時に数字がカウントアップする演出や、アイコンが飛び出す動きを追加。
    - **[NEW] 提案書PDF発行**: シミュレーション結果を「上司説得用」の提案書形式（PDF）でダウンロード可能にする。
        - **[UPDATE] 2ページ目追加**: 業種別（飲食、建設、小売、事務など）の具体的なAI活用・削減事例を掲載し、説得力を強化。
    - デザイン: 親しみやすい、かわさき楽AIサポートのブランドカラー（暖色系想定）に合わせたシンプルなUI。

#### [NEW] [sns_posts.txt](file:///c:/Users/utaka/かわさき楽AIサポート/docs/marketing_tools_creation/sns_posts.txt)
- **概要**: LINE, X, Facebook用の投稿文面ドラフト。
- **内容**: シミュレーターへの誘導を目的とし、「損したくない」「夢が広がる」心理に訴求する文面。

#### [NEW] [announcement_email.txt](file:///c:/Users/utaka/かわさき楽AIサポート/docs/marketing_tools_creation/announcement_email.txt)
- 既存顧客およびリード顧客に向けた、新ツール（シミュレーター）公開のお知らせメール文面。
- ターゲット別に内容を微調整（経営者向け）。

## Verification Plan

### Manual Verification
- **各ブラウザでの動作確認**: 作成した `cost_simulator.html` をChrome/Edgeで開き、計算ロジックが正しいか確認する。
- **レスポンシブ確認**: スマホサイズ（幅375px程度）でもレイアウトが崩れないか確認する。
