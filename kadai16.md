# 講義16 課題提出（kadai16）

- 日付: 2025-09-22  
- 課題名: プルリクエストを作成する（講義16）  

## 目的
- GitHub 上での PR 作成・更新手順の確認と記録  

## 実施手順（再現手順）
1. ローカルでブランチ作成  
   - `git checkout -b kadai16`
2. ファイル作成・編集  
   - `kadai16.text` を作成し内容を記載
3. ステージング・コミット・push  
   - `git add kadai16.text`  
   - `git commit -m "kadai16: add submission file"`  
   - `git push origin kadai16`
4. GitHub 上で PR を作成  
   - タイトル・説明を記付
5. 不要ファイル `test.txt` を削除  
   - `main` ブランチに切り替えて `git rm test.txt`  
   - `git commit -m "不要な test.txt を削除"`  
   - `git push origin main`

## 実施内容（詳細）
- `kadai16.text` を追加し、PR を作た  
- 不要な `test.txt` ファイルを削除  

## 動作確認（期待値）
- GitHub 上で PR が作成されていることを確認  
- PR の Files changed に差分が表示されることを確認  
- main ブランチ上で `test.txt` が削除されていることを確認  

## 学んだこと
- PR は「提案」であり、マージしない限り main に反映されないこと  
- main に直接 push すると即反映されること  
- 同じ「削除」でも、PR経由と直接 push では挙動が違うことを体験した  
- README.md はリポジトリ作成時に自動生成されるファイルであること


