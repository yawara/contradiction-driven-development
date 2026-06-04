# 矛盾が露出した境界だけを裁く

> AI slop の時代における矛盾駆動開発（Contradiction-Driven Development）の提唱

AIが無限に生成する時代に、人間の有限な判断を「矛盾が露出した境界」へ集中させる——そんな開発方法論を論じたエッセイと、その公開サイトのリポジトリ。

🔗 **https://yawara.github.io/contradiction-driven-development/**

## 概要

教皇レオ14世のAI発言、Linus Torvalds の態度、arXiv の endorsement 制約を補助線に、要求・実装・テスト・設計・人間の意図のあいだに現れる「矛盾」を介入点として捉える開発手法 **Contradiction-Driven Development (CDD)** を定式化する。

## 構成

| ファイル                                                                       | 役割                                          |
| ------------------------------------------------------------------------------ | --------------------------------------------- |
| [essay.md](essay.md)                                                           | エッセイ本文（トップページ / `permalink: /`） |
| [\_layouts/default.html](_layouts/default.html)                                | レイアウト・CSS・テーマソング再生ダイアログ   |
| [\_config.yml](_config.yml)                                                    | Jekyll 設定（`hard_wrap` など）               |
| [contradiction.mp3](contradiction.mp3)                                         | テーマソング（BGM）                           |
| [.github/workflows/jekyll-gh-pages.yml](.github/workflows/jekyll-gh-pages.yml) | ビルド & デプロイ                             |

## 公開の仕組み

GitHub Pages + Jekyll。`main` へ push すると GitHub Actions が自動でビルド・デプロイする。

## 特徴

- 日本語長文向けのミニマルなレイアウト（ダークモード固定 / Webフォント不使用）
- 読み込み時に「テーマソングを再生しますか？」ダイアログ → 同意で BGM をループ再生
