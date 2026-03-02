# 読書感想会用：Slidevテンプレート

## 始め方

- `pnpm install`
- `pnpm dev`
- visit <http://localhost:3030>

## 使い方

### 編集方法

`./slides.md`に内容を記載していく。

参照：https://ja.sli.dev/guide/syntax

### ページテンプレート

フロントマターの`layout`で変更。
現状は3種類のみ。

- cover
- section-top
- with-image

参照：https://ja.sli.dev/guide/layout

### 画像など

`assets/images`に格納して使用。

使用例：

```md
<img src="./assets/images/photo-1.jpg" />
```

### コンポーネント

使い回すものは`components`にVueファイルを作成する。

現状は2種類のみ。

- Header.vue
- Point.vue

使用例：

```md
::point
なにかしらポイントを書く。
::
```

参照：https://ja.sli.dev/guide/component
