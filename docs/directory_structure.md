/ (root)
├─ .github/
│   └─ workflows/
│       └─ ci.yml       # CIテスト用ワークフロー (編集しない)
├─ docs/                # 設計・仕様書、外部連携情報などのドキュメント
│   ├─ directory_structure.md
│   ├─ designdoc.md
│   └─ architecture.md
├─ logs/                # コマンド実行ログを保存 (出力を常にリダイレクト)
├─ test/                # テストシナリオやテストコード
│   └─ test_scenarios.md
├─ task.yaml            # タスク管理（スプリントやTodo）
├─ test.yaml            # TDDの終了条件やテストケース
└─ .gitignore           # 不要ファイル・ビルド成果物を除外
