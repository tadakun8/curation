## CommitLintとは？

- コミットメッセージが意図したフォーマットで書かれているかをチェックしてくれるツール
- チーム内でコミットメッセージを統一したい場合に使用する
- npmツール
- 単体では意味をなさないため、[husky](./husky)を入れて使う場合が多い
- コミットルールは次のパターンに従う
    - Angularのコミットルールが元になっている

    ```
    type(scope?): subject
    body?
    footer?
    ```
    
### 公式URL
- [リポジトリ](https://github.com/conventional-changelog/commitlint)
- [ドキュメント](https://qiita.com/ybiquitous/items/74225bc4bf0a9ddcd7dd)

### 参考記事
- https://wp-kyoto.net/add-commitlint-with-husky-to-lint-git-commit-message/
- https://qiita.com/Seika139/items/9c614c0bc5804c0753c6