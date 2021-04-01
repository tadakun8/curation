## jsconfig.jsonとは？

- vscodeでjsを書くときに便利にコーディングできるようにする設定ファイル
- create-nuxt-appで作成されたjsconfig.jsonの例
    ```json
    {
    "compilerOptions": {
        "baseUrl": ".",
        "paths": {
        "~/*": ["./*"],
        "@/*": ["./*"],
        "~~/*": ["./*"],
        "@@/*": ["./*"]
        }
    },
    "exclude": ["node_modules", ".nuxt", "dist"]
    }

    ```
- もしかしたらtypescriptの場合はtsconfig.jsonがあるので、jsconfigがいらない気がする

### 参考
- [Vue.jsをVSCodeで書く時はVeturを入れてjsconfig.jsonを書こう](https://qiita.com/nyallpo/items/c50909926e465fabdb55)
    - 何ができるのかのデモ
- [【TypeScript】TSConfigの基礎](https://marsquai.com/a70497b9-805e-40a9-855d-1826345ca65f/1dc3824a-2ab9-471f-ad58-6226a37245ce/b5ce5f32-2afa-41f5-9fae-a3979f5c13df/)
    - typescriptの場合はtsconfig、javascriptの場合はjsconfigとの記載があった