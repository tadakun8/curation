## CommitLintとは？

- コミットメッセージが意図したフォーマットで書かれているかをチェックしてくれるツール
- チーム内でコミットメッセージを統一したい場合に使用する
- npmツール
- 単体では意味をなさないため、[husky](./husky)を入れて使う場合が多い
- コミットルールは次のパターンに従うが、カスタマイズもできる
    - Angularのコミットルールが元になっている

    ```
    type(scope?): subject
    body?
    footer?
    ```

## 導入方法

```
$ npm install --save-dev @commitlint/{cli,config-conventional}

$ echo "module.exports = {extends: ['@commitlint/config-conventional']};" > commitlint.config.js
```

- package.jsonに以下を追加(nameやscriptと同階層)
```json
"husky": {
    "hooks": {
      "commit-msg": "commitlint -E HUSKY_GIT_PARAMS"
    }
}
```
### 公式URL

- [リポジトリ](https://github.com/conventional-changelog/commitlint)
    - commitlintコマンドの使い方
    - typeの一覧
    - 使用できるルールの一覧

### 参考記事

- [commitlint の紹介](https://qiita.com/ybiquitous/items/74225bc4bf0a9ddcd7dd)
    - 簡単なデモ
- [commitlint + husky でConventional Commitを強制する](https://wp-kyoto.net/add-commitlint-with-husky-to-lint-git-commit-message/)
    - 導入方法
    - 設定方ほ
- https://qiita.com/Seika139/items/9c614c0bc5804c0753c6
    - 導入方法
    - 設定方法
- [従来のコミットでコミットを改善する](https://ichi.pro/jurai-no-komitto-de-komitto-o-kaizensuru-125427180186905)
    - カスタマイズの例
- [How to validate github issues / jira issues #237](https://github.com/conventional-changelog/commitlint/issues/237)
    - カスタマイズの方法
    - parserPresetを使用している