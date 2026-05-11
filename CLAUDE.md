# Roblox Creator Project

Robloxゲーム開発: アイデア管理・Luauコード生成・収益化・成長戦略。

## ワークフロー
ClaudeがLuauコードを生成 → ユーザーがRoblox Studioにコピペして実装。
ローカル実行環境なし。コードの動作確認はRoblox Studio上で行う。

## 必須ルール
1. **Codexレビュー必須**: コード生成後は `codex:rescue` でレビューを実施してから提出
2. アイデアは `docs/ideas/YYYY-MM-DD-title.md`、調査結果は `docs/research/` に記録
3. 重要な設計決定は必ず関連エージェントに諮問してから実装
4. コードはコピペしやすいよう**ファイル単位**で出力し、配置先パスを明記する

## コード出力規約
- 配置先パスを必ず冒頭に記載: `-- 配置先: ServerScriptService/Server/FeatureName.luau`
- strict Luauアノテーション付き
- RemoteEventsは必ずサーバー側でバリデーション（クライアント信頼なし）
- コメントはWHYのみ（何をするかは命名で表現）

## エージェント
- `roblox-researcher` — Roblox動向・競合調査
- `game-designer` — ゲームメカニクス・UX設計
- `luau-developer` — Luauコード生成・API活用・最適化
- `monetization-expert` — Robux設計・GamePass・DeveloperProduct
- `growth-strategist` — プレイヤー獲得・リテンション・コミュニティ
- `qa-tester` — Exploit対策・テスト計画
- `perf-optimizer` — パフォーマンス最適化

## ファイル規約
- アイデア: `docs/ideas/YYYY-MM-DD-title.md`
- 調査: `docs/research/YYYY-MM-DD-topic.md`
- 設計書: `docs/design/feature-name.md`
- 生成コード: `src/[Server|Client|Shared]/FeatureName.luau`
