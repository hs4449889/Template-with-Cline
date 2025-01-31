# セットアップ


# 運用ガイド

このリポジトリでは、以下の方針でプロジェクトを進めてください。

## 1. TDDとログ出力

- **タスク分割**  
  `task.yaml` にタスク内容を細分化し、進捗を管理します。  
- **テスト定義**  
  `test.yaml` に各タスクのテスト条件を記載し、テストコードは `test/` ディレクトリに配置します。  
- **テスト駆動開発 (TDD)**  
  すべてのテストが合格するまで実装を続け、テスト合格をもってタスク完了とします。  
- **ログ運用**  
  コマンドやスクリプト実行時は、標準出力を `logs/` 以下のログファイルへリダイレクトし、結果を常に確認します。  

## 2. コミット運用

- **タスク単位のコミット**  
  タスクが完了するたびにコミットしますが、**必要最小限のファイル** のみをステージングし (`git add .` は避ける)、不要なファイルは含めないようにします。  
- **コミットメッセージのベストプラクティス**  
  コミットメッセージは[ベストプラクティス](https://chris.beams.io/posts/git-commit/)に従い、簡潔かつ明確にまとめます。  

## 3. ナレッジ管理

- 設計や仕様、外部リポジトリ連携については、`docs/` ディレクトリにドキュメントを蓄積してください。  
- **新しい情報や要件が発生した場合**  
  適宜追記・更新し、常に最新の状態を保ちます。  

## 4. ディレクトリ構造ドキュメント

- **変更が発生した場合の更新ルール**  
  ファイルやフォルダの追加・削除・名称変更があった場合は、`docs/directory_structure.md` を更新し、各ディレクトリやファイルの役割を明示します。  
- **新規参画者向けのメンテナンス**  
  新しく参画するメンバーがすぐに内容を把握できるよう、常にメンテナンスを続けてください。  

## 5. custom instructions
```
TDD & Logging
Use task.yaml for task breakdown and test.yaml for test cases
Redirect all command outputs to logs/*, then review logs
Only finalize tasks when all tests pass
Committing
After each task, commit only necessary files (avoid git add .)
Follow best-practice commit messages
Knowledge Management
Keep design/specs in docs/*, including external repo references
Update as needed to maintain clarity
Directory Docs
Whenever files/structure change, update docs/directory_structure.md with roles/usage
```
