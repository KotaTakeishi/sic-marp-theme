# SIC Marp Theme

## 環境構築

```sh
npm ci
```

以下のコマンドでスライドのプレビューを確認することができます

```sh
npm run presentation
```

また、以下のコマンドでPDF・PPTXを出力することができます

```sh
npm run export
```

vscodeの場合は、[Marp for VS Code](https://marketplace.cursorapi.com/items?itemName=marp-team.marp-vscode)をインストールすることで、簡単にプレビューを確認することができます。

## スライドの作り方

`slide.md`にスライドの内容を以下のようなフォーマットで記述します。区切り線（`---`）でページを区切ります。marpの独自記法が沢山あるので、[Marp Basic Example](https://speakerdeck.com/yhatt/marp-basic-example)を読んでおくことをおすすめします。

```md
---
marp: true
theme: sic
paginate: true
---

# 1ページ目

<!-- 1ページ目のスピーカーノートを書くことができます -->

---

# ２ページ目

```

## スライドのテンプレート

`themes/sic.css`の中でスライドのテンプレートを定義しています。mdには`_class`を使ってテンプレートを指定します。自由にカスタマイズしてください。

## 参考資料

- [Marp公式サイト](https://marp.app/)
- [Marp Basic Example](https://speakerdeck.com/yhatt/marp-basic-example)
- [Marp for VS Code](https://marketplace.cursorapi.com/items?itemName=marp-team.marp-vscode)
- [Marp Core built-in themes](https://github.com/marp-team/marp-core/tree/main/themes#metadata-for-additional-features)
- [Marpit Markdown](https://marpit.marp.app/markdown)
