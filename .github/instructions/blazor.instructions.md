---
applyTo: "SocOps/**/*.cs, SocOps/**/*.razor"
description: "SocOps プロジェクトにおける C# と Blazor WebAssembly の実装規約。"
---

# C# / Blazor 開発指示

**開発チェックリスト**: 変更後は対応プロジェクトで `dotnet build`、テストプロジェクト存在時は `dotnet test`、`Services`/`Models`/`Program.cs`/`_Imports.razor` 変更時またはファイル3個以上は `SocOps/SocOps.csproj` に対して実行してください。

- .NET 10 Blazor WebAssembly、nullable 参照型、暗黙的な using と互換性を保ち、`SocOps` 名前空間で `Models`（ドメイン）、`Services`（ロジック）、Razor コンポーネント（UI）に分離してください。
- Razor コンポーネントは `[Parameter]` と `EventCallback` を使用し、ゲームルールや状態遷移は既存の `Services` に集約してください。
- 非同期処理は `async Task` で、JavaScript 相互運用とストレージ操作は `try/catch` で例外を捕捉し、`ILogger` で記録して既定値にフォールバックさせてください。fire-and-forget や例外の握りつぶしは避けてください。
- 既存パターンと `.github/instructions/css-utilities.instructions.md` を優先し、新しい依存関係の追加前に既存ユーティリティの活用を検討してください。
