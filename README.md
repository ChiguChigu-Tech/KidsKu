# KidsKu -キズク-

> [!NOTE]
> 本リポジトリは、PKSHA HACKATHON 2025で制作したチームプロジェクト「KidsKu」の個人Forkです。
>
> プロジェクトにおける私の担当範囲は、
> [MY_CONTRIBUTIONS.md](./MY_CONTRIBUTIONS.md)
> に記載しています。

SNSへの投稿前に内容を確認し、子ども自身にリスクへの「気づき」を与える見守りAIエージェントです。

## サービス概要

[X（旧Twitter）](https://x.com/)で投稿しようとする前に、AIエージェントが投稿内容の安全性を確認します。

- **安全と判断した場合**：そのまま投稿処理を続行
- **注意が必要と判断した場合**：理由と訂正案を、子どもに寄り添った表現で提示
- **危険と判断した場合**：問題点を説明し、投稿を見直すよう促す

単純な禁止語句の検出ではなく、投稿の文脈や意図をAIで判定することで、子どもの自己表現を尊重しながら、安全にSNSを利用できる環境を目指しました。

## デモ動画

| 感情的な表現を見直し、伝え方を工夫する | 個人情報を含む投稿を防ぎ、リスクを学ぶ |
| :---: | :---: |
| <video src="https://github.com/user-attachments/assets/0e598577-1cd5-491d-a920-f10b984fbbaa" /> | <video src="https://github.com/user-attachments/assets/3e530573-08e0-4e10-b534-78422dcd92cc" /> |

## 使用技術

本アプリは、Chrome拡張機能として動作するフロントエンドと、LangChain / LangGraphを活用したAIエージェントによるバックエンドで構成されています。

### フロントエンド

- HTML
- CSS
- JavaScript
- Chrome Extension

### バックエンド

- Python
- LangChain
- LangGraph

## チーム開発

本プロジェクトは、PKSHA HACKATHON 2025において、3日間で企画、設計、実装、デモ作成、発表までを行ったチーム開発プロジェクトです。

プロジェクト全体はチームで共同開発しました。私個人の担当範囲については、[MY_CONTRIBUTIONS.md](./MY_CONTRIBUTIONS.md)をご覧ください。

## 実績

- PKSHA HACKATHON 2025 3位入賞

## 成果物・関連資料

- [最終発表資料（PDF）](https://drive.google.com/file/d/1l9YF5MFiGBKen3rp4fc77tVA7T5WUXnP/view?usp=sharing)
- [個人の担当範囲](./MY_CONTRIBUTIONS.md)
- [Fork元リポジトリ](https://github.com/endo1322/KidsKu)
