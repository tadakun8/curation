## huskyとは？

- gitイベントをhookして任意のコマンドを走らせたい場合に使用する**npmツール**
    - commit時に、npm scriptのtestコマンドを走らせたいなど

## 注意点

- huskyのバージョンで、v4からv5二では破壊的な変更されている
    - 参考を参照する
### 参考
- [Git で commit 前に 自動でコマンドを実行する #Node.js #husky](https://dev.classmethod.jp/articles/pre-commit/)
    - 説明
    - インストール方法
    - 使い方
- [npm や yarn でインストールした husky が動かない問題の対応方法](https://r17n.page/2021/03/12/fix-husky-hooks-not-working/)
- [husky v5 で消耗している人には simple-git-hooks がお薦め](https://qiita.com/acro5piano/items/10f406c3ecc8ea1d14ce)