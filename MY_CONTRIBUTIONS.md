# My Contributions

## この文書について

この文書は、PKSHA HACKATHON 2025で制作したチームプロジェクト「KidsKu」における、私個人の担当・提案内容を整理したものです。

プロジェクト全体はチームで共同開発しており、ここではGitHub上のIssue・Pull Requestから確認できる私の活動のみを記載しています。

- Fork元リポジトリ: [endo1322/KidsKu](https://github.com/endo1322/KidsKu)
- 成果: PKSHA HACKATHON 2025 3位入賞

## 担当・貢献内容

### 1. Safe判定時に投稿を続行する処理

AIによる判定結果が `safe` の場合に、確認メッセージを表示したうえでXへの投稿処理を続行する機能を実装しました。

主な対応内容:

- ユーザーによるクリックとプログラムから発行されたクリックを `e.isTrusted` で区別
- プログラムからの再クリックを判定処理の対象外にして、イベントの再帰実行を防止
- Safe判定時にユーザーへ結果を表示し、元の投稿ボタンを再実行
- APIレスポンスの取り扱いと条件分岐を整理

関連リンク:

- [Issue #18: Safeのときに投稿を続行する](https://github.com/endo1322/KidsKu/issues/18)
- [Pull Request #19: Feature/#18](https://github.com/endo1322/KidsKu/pull/19) — マージ済み

### 2. YouTubeコメント監視への対応案・試作

XだけでなくYouTubeのコメント投稿も監視対象にするため、投稿ボタンと入力欄をサービスごとに定義し、共通処理でフックする試作を行いました。

主な試作内容:

- XとYouTubeで異なる投稿ボタン・入力欄のセレクタを整理
- ボタン要素と入力欄セレクタを受け取る共通のフック処理を作成
- `MutationObserver`を用いて、動的に追加される投稿ボタンを検出
- 判定結果を表示するトーストUIの拡張

このPull Requestはマージされていないため、最終成果物へ採用された実装ではありません。ポートフォリオ上では、複数SNSへの展開を検討した試作・技術検証として位置付けています。

関連リンク:

- [Issue #12: Youtubeのコメント監視に対応](https://github.com/endo1322/KidsKu/issues/12)
- [Pull Request #13: Feature/#12](https://github.com/endo1322/KidsKu/pull/13) — 未マージ

### 3. 追加機能とユーザーフィードバック方針の整理

プロダクトの発展案として、以下の機能・方針をIssue上で整理しました。

- 保護者向けレポートWebサイト
- 過去の投稿を含む情報表示
- データベースを用いた禁止用語設定
- Gmail・Slack APIなどを利用した保護者通知
- LLMによる投稿内容へのフィードバック
- 投稿が周囲へ与える印象を子ども自身に考えてもらう、教育的な問いかけ

関連リンク:

- [Issue #6: 追加機能の整理](https://github.com/endo1322/KidsKu/issues/6)
- [Issue #21: XとYoutubeの両方における判定機能](https://github.com/endo1322/KidsKu/issues/21)

## この開発で得た経験

- Chrome ExtensionにおけるContent ScriptとDOMイベントの取り扱い
- 動的Webページに対する`MutationObserver`の利用
- AI判定結果と投稿処理を接続するフロントエンド実装
- 複数サービスへ展開するための処理共通化の検討
- IssueとPull Requestを用いたチーム開発
- 子どもの安全と自律的な学習を両立するプロダクト設計

## 注意

本リポジトリには、チームメンバーが設計・実装した機能も含まれています。プロジェクト全体を私一人で開発したものではありません。
