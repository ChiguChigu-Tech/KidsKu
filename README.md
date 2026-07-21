# KidsKu -キズク-

> [!NOTE]
> 本リポジトリは、PKSHA HACKATHON 2025で制作し、3位に入賞したチームプロジェクト「KidsKu」の個人Forkです。  
> Fork元は [endo1322/KidsKu](https://github.com/endo1322/KidsKu) です。プロジェクトにおける私個人の担当・提案内容は、[MY_CONTRIBUTIONS.md](./MY_CONTRIBUTIONS.md) に整理しています。

SNS投稿前の内容をチェックし、子どもにリスクへの「気づき」を与える見守りAIエージェントです。

## サービス概要

[X（旧Twitter）](https://x.com/)で投稿しようとする前に、AIエージェントが投稿内容の安全性を確認します。

- **安全と判断した場合**：そのまま投稿処理を続行
- **注意が必要と判断した場合**：理由と訂正案を、子どもに寄り添ったやさしい表現で提示
- **危険と判断した場合**：何が問題かを丁寧に説明し、子ども自身が気づけるよう促します

## デモ動画（ユースケース）

| 感情的な表現を見直し、伝え方を工夫する | 個人情報を含む投稿を防ぎ、リスクを学ぶ |
| :---: | :---: |
| <video src="https://github.com/user-attachments/assets/0e598577-1cd5-491d-a920-f10b984fbbaa" /> | <video src="https://github.com/user-attachments/assets/3e530573-08e0-4e10-b534-78422dcd92cc" /> |

## 使用技術

本アプリは、Chrome拡張機能として動作するフロントエンドと、LangChain / LangGraphを活用したAIエージェントによるバックエンドで構成されています。

- **フロントエンド**：HTML / CSS / JavaScript（Chrome Extension）
- **バックエンド**：Python（LangChain / LangGraph）

## 個人の担当範囲

GitHub上のIssue・Pull Requestから確認できる私の担当内容、試作、機能提案は、以下に記載しています。

- [MY_CONTRIBUTIONS.md](./MY_CONTRIBUTIONS.md)

主な内容:

- Safe判定時にXへの投稿を続行する処理の実装
- YouTubeコメント監視への対応案・試作
- 保護者向け機能やLLMフィードバック方針の整理

> プロジェクト全体はチームで共同開発したものであり、リポジトリ内には他のメンバーが設計・実装した機能も含まれています。
