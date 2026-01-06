# Snake Game

## Run
python3 main.py

## Controls
- Arrow keys to move

## Git 毎回の基本手順（まとめ）
※ `feature/input` の部分は、その作業に合わせてブランチ名を変える（例：feature/render、feature/logic）

```bash
# 0) main を最新化
git switch main
git pull

# 1) 作業ブランチ作成（例：feature/input）
git switch -c feature/input

# 2) 作業 → 変更をコミット
git add .
git commit -m "Describe your change"

# 3) ブランチをGitHubへpush
git push -u origin feature/input

# 4) GitHubでPRを作成してMerge（ブラウザ操作）
# - base: main / compare: feature/input を確認
# - Create pull request -> Merge pull request

# 5) マージ後、main を更新
git switch main
git pull

# 6) 後片付け（任意：ブランチ削除）
git branch -d feature/input
git push origin --delete feature/input
