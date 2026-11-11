🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md) | [English](README.en.md)

# 🎯 Soc Ops — 交流イベント向けソーシャルビンゴ

新しい人間関係を作ろう。**Soc Ops** で、イベント会場での交流を楽しいゲームに変えましょう。プロンプトに合う人を見つけて、横縦斜めに5つ揃えば勝ち！ネットワーキングがもっと楽しくなります。

<div align="center">

🎮 **[今すぐプレイ](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/)** • 📖 **[ラボガイド](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/)** • 🛠 **[2分で始める](#クイックスタート)**

</div>

---

## ✨ このプロジェクトの特徴

**Soc Ops** は、実践的な .NET フルスタック開発を学べるモダン **Blazor WebAssembly** アプリケーションです：

- 🎨 **洗練されたUI** — カスタムCSSユーティリティとスムーズなアニメーションで最高の体験を実現
- 🤖 **AI駆動** — GitHub Copilot エージェントと連携し、ビンゴの質問を動的に生成
- 🏗️ **良く設計されたアーキテクチャ** — サービス、モデル、コンポーネント層が明確に分離
- 📱 **完全レスポンシブ対応** — デスクトップ、タブレット、モバイルでシームレスに動作
- 🚀 **本番環境対応** — GitHub Pages に自動デプロイ；ローカル実行も簡単

---

## 🚀 クイックスタート

### 必要なもの
- [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) 以上

### ローカルで実行
```bash
cd SocOps
dotnet run
```
ブラウザで **http://localhost:5000** を開いてプレイ開始！

### ビルド
```bash
cd SocOps
dotnet build
```

### クラウド実行：GitHub Codespaces（セットアップ不要）
1. このリポジトリをフォーク
2. **Code** → **Codespaces** → **Create codespace on main** をクリック
3. セットアップ完了後、以下を実行：
   ```bash
   cd SocOps
   dotnet run
   ```

---

## 📚 学んで作る：ラボガイド

このリポジトリは、.NET開発者向けの **インタラクティブな学習体験** として設計されています。各ラボは前のステップを基に構成されています：

| ステップ | テーマ | 学べること |
|---------|-------|----------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | 概要とチェックリスト | プロジェクト構成と目標 |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | セットアップとコンテキスト設計 | Copilot設定とカスタム指示 |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | デザインファーストなフロントエンド | 美しいBlazorコンポーネントの構築 |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | カスタムクイズマスター エージェント | 特殊なCopilotエージェントの作成 |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | マルチエージェント開発 | 複数のAIエージェント間の連携 |

> 📝 **オフライン環境？** ラボガイドは [`workshop/`](workshop/) フォルダでも利用できます。

---

## 🏗️ プロジェクト構成

```
SocOps/
├── Components/       # 再利用可能なBlazorコンポーネント（Card、Board等）
├── Pages/           # ページコンポーネント（Game、Home）
├── Services/        # ビジネスロジック（GameService、QuestionService）
├── Models/          # データ構造（Player、Question、GameState）
├── Layout/          # メインレイアウトとナビゲーション
├── wwwroot/
│   └── css/         # カスタムユーティリティクラス（Tailwind風）
└── Program.cs       # アプリ設定とDI設定
```

---

## 🛠️ 技術スタック

- **フレームワーク：** [Blazor WebAssembly](https://learn.microsoft.com/ja-jp/aspnet/core/blazor)
- **言語：** C# 13
- **ランタイム：** .NET 10
- **スタイリング：** カスタムCSSユーティリティ（外部依存なし）
- **AI連携：** GitHub Copilot エージェント
- **デプロイ：** GitHub Pages（`main` ブランチへのプッシュで自動デプロイ）

---

## 🎮 ゲームの遊び方

1. **イベント会場でゲームを開く**
2. **ビンゴカードから質問を選択**
3. **その説明に当てはまる人を探す**
4. **人を見つけたらマスをチェック**
5. **横縦斜めに5つ揃えば勝ち！**
6. **複数ラウンドで何度でもプレイ**

---

## 📖 ドキュメント

- **[貢献ガイド](CONTRIBUTING.md)** — 改善の提案方法
- **[セキュリティポリシー](SECURITY.md)** — 脆弱性の報告方法
- **[行動規範](CODE_OF_CONDUCT.md)** — コミュニティ基準
- **[サポート](SUPPORT.md)** — ヘルプとイシュー報告

---

## 🤝 貢献方法

改善提案、新機能、ドキュメント改善など、すべての貢献を歓迎します！

1. リポジトリをフォーク
2. 機能ブランチを作成（`git checkout -b feature/amazing-feature`）
3. 変更をコミット（`git commit -m 'Add amazing feature'`）
4. ブランチにプッシュ（`git push origin feature/amazing-feature`）
5. プルリクエストを作成

詳細は [CONTRIBUTING.md](CONTRIBUTING.md) をご覧ください。

---

## 📄 ライセンス

このプロジェクトは [MIT ライセンス](LICENSE) の下で公開されています。

---

## 🎓 こんな方に最適

- **Blazor WebAssembly を学びたい方** — モダンな C# とコンポーネントパターンを習得
- **GitHub Copilot を探索したい方** — エージェント活用法を効果的に学ぶ
- **イベント企画者** — 参加者が楽しめる低障壁の交流ゲーム
- **.NET開発者** — ベストプラクティスを含むフルスタック例

---

**❤️ .NET コミュニティで作られています**
