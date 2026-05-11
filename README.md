# Roblox Creator Project

RobloxゲームのアイデアからLuauコード生成・収益化・成長戦略を管理するプロジェクト。

## ワークフロー

```
1. /idea     → ゲームアイデアをキャプチャ・整理
2. /design   → ゲームデザイン文書を作成
3. /strategy → 実装優先度・ロードマップを策定
4. /code-review → LuauコードをClaudeが生成 → Roblox Studioにコピペ
5. /test-plan → QA・Exploit対策を確認
6. /monetize → 収益化設計
7. /release  → リリースチェックリスト確認
```

## ディレクトリ構成

```
src/          # 生成されたLuauコード（配置先パス付き）
docs/
  ideas/      # ゲームアイデア (YYYY-MM-DD-title.md)
  research/   # 調査レポート   (YYYY-MM-DD-topic.md)
  tasks/      # タスク管理
  design/     # ゲームデザイン文書
assets/       # 画像・アセット参考資料
```

## コマンド

| コマンド | 役割 |
|----------|------|
| `/idea` | ゲームアイデアのキャプチャと整理 |
| `/research` | Roblox最新動向・競合・トレンド調査 |
| `/design` | ゲームデザイン・メカニクス設計 |
| `/code-review` | Luauコード生成・レビュー (Codex連携) |
| `/monetize` | 収益化戦略・Robux設計 |
| `/strategy` | 成長戦略・マーケティング |
| `/test-plan` | QA・Exploit対策・テスト計画 |
| `/perf` | パフォーマンス分析・最適化 |
| `/release` | リリースチェックリスト |

## GitHub管理

- **Issue** — アイデア・バグ・タスクの起票
- **PR** — コード・設計書の変更レビュー
- **Labels** — `idea` / `design` / `code` / `bug` / `monetize` / `research`

## Claude Code 更新

```bash
claude update
```
