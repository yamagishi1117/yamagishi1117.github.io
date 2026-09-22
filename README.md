# Developer site (GitHub Pages)

AdMob が参照する `app-ads.txt` を **ユーザーサイトのルート**に置くためのリポジトリです。

公開 URL: https://yamagishi1117.github.io/app-ads.txt

## 初回セットアップ

1. GitHub で **新規リポジトリ** `yamagishi1117.github.io` を作成（Public）。
2. このフォルダから push:

```bash
cd /Users/yukiyamagishi/Projects/yamagishi1117.github.io
git init
git add app-ads.txt README.md
git commit -m "Add app-ads.txt for AdMob verification"
git branch -M main
git remote add origin git@github.com:yamagishi1117/yamagishi1117.github.io.git
git push -u origin main
```

3. 数分後: `curl https://yamagishi1117.github.io/app-ads.txt` が 200 になることを確認。
4. App Store Connect の **マーケティング URL** を `https://yamagishi1117.github.io/` に設定。
5. AdMob → **アップデートを確認**。

既存の [app-ads-txt](https://github.com/yamagishi1117/app-ads-txt) リポジトリの内容と同じ行です。AdMob はホスト直下の `/app-ads.txt` を見に行くため、こちらのリポジトリが必要です。
