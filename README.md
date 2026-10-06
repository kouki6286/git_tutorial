# git_tutorial

Git と GitHub の基本操作を練習するためのリポジトリです。
アプリケーションのコードは入っていません。中身は小さな HTML ファイルだけで、コミット・ブランチ・マージ・プルリクエストなどを試すたびに追加や変更をしてきた練習の記録になっています。

## ファイル一覧

| ファイル | 内容 | 練習した内容 |
| --- | --- | --- |
| `index.html` | 見出し「Git Tutorial」と、学んだコマンド・用語の一覧 | 学習内容のメモ（後述） |
| `home.html` | `home` / `git pull` | GitHub 上で作成・編集し、`git pull` でローカルに取り込む |
| `master.html` | `master` | master ブランチでの作業 |
| `feature.html` | `branch` / `feature` | feature ブランチでの作業 |
| `master2.html` | `master2` | master 側での追加作業 |
| `feature2.html` | `feature2` | feature 側での追加作業 |
| `first.html` | （空ファイル） | 複数ファイルをまとめてコミット |
| `second.html` | （空ファイル） | 同上 |
| `third.html` | （空ファイル） | 単独のファイルをコミット |
| `.gitignore` | `secret.txt` を指定 | Git の管理から外すファイルの指定 |

## `index.html` に書かれている学習項目

`index.html` には、練習で使った Git の操作が順番に書かれています。

1. `git status`：作業ツリーの状態を確認する
2. `git diff`：変更内容の差分を確認する
3. `git commit --amend`：直前のコミットを修正する
4. `git merge`：ブランチを統合する
5. conflict：マージ時の競合を解消する
6. pull_request：GitHub 上でプルリクエストを作る
7. GitHub Flow：ブランチを切り、プルリクエスト経由で master にマージする流れ

## コミット履歴から見た学習の流れ

```
initial commit
 ├─ git status / git diff の追記
 ├─ .gitignore の追加、git commit --amend の練習
 ├─ GitHub 上で home.html を作成・更新 → git pull
 ├─ master.html（master）と feature.html（feature）をそれぞれのブランチで作成
 ├─ feature ブランチを merge、競合（conflict）を発生させて解消
 ├─ pull_request / GitHub Flow の練習（github_flow ブランチ → PR #2 で master にマージ）
 └─ master2.html, feature2.html, first〜third.html の追加
```

## ブランチ

- `master`：メインのブランチ
- 練習中に `feature` や `github_flow` などのブランチを作り、マージしています（現在、リモートに残っているのは `master` と作業用ブランチだけです）。
