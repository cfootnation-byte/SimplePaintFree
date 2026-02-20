
<h1 align="center">SimplePaint</h1>

<p align="center">
  AIベースのイラスト＆ウェブトゥーンアシスタントツール
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version" />
  <img src="https://img.shields.io/badge/platform-Windows%2010%2B-0078D6?logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/license-Proprietary-red" alt="License" />
  <img src="https://img.shields.io/badge/Qt-6.7-41CD52?logo=qt" alt="Qt" />
</p>

<p align="center">
  <a href="../README.md">한국어</a> | <a href="README_en.md">English</a> | <b>日本語</b>
</p>

---

## 紹介

SimplePaintは、線画から彩色、陰影までAIが自動化するイラスト＆ウェブトゥーン制作ツールです。
ご自身のAPIキー（Gemini、Flux）を使用してAI機能を無料でご利用いただけます。

---

## ドキュメント

<table>
  <tr>
    <td align="center" width="50%">
      <h3>🎨 AI機能</h3>
      <p>陰影生成 · ベース色生成 · キャラクターシート · 線画生成 · 領域分離</p>
      <a href="AI_FEATURES_ja.md"><b>詳しく見る →</b></a>
    </td>
    <td align="center" width="50%">
      <h3>🖥️ インターフェース＆基本機能</h3>
      <p>メニューバー · ツールバー · レイヤーシステム · ブレンドモード</p>
      <a href="INTERFACE_ja.md"><b>詳しく見る →</b></a>
    </td>
  </tr>
</table>

---

## APIキー設定

SimplePaint Freeはご自身のAPIキーを使用します。AI機能を使用するには以下のAPIキーが必要です：

| API | 用途 | 発行元 |
|-----|------|--------|
| Flux (BFL) | 陰影生成、ベース色生成、線画生成 | [Black Forest Labs](https://api.bfl.ml/) |
| Gemini (Google) | キャラクターシート生成、領域分離、色分析 | [Google AI Studio](https://aistudio.google.com/) |

アプリ起動後、**設定 → API Settings**でキーを入力してください。

---

## システム要件

| | 最小スペック | 推奨スペック |
|---|------------|------------|
| OS | Windows 10 (64-bit) | Windows 11 (64-bit) |
| CPU | Intel i5 | Intel i7 |
| RAM | 8GB | 16GB+ |
| GPU | 2GB VRAM | 4GB VRAM (NVIDIA) |
| Storage | 5GB | 10GB |

---

## インストール

1. [Releases](../../releases)ページから最新のインストーラーをダウンロードします。
2. ダウンロードしたインストーラーを実行します。
3. インストールウィザードの案内に従ってインストールを完了します。
4. SimplePaintを起動し、APIキーを設定します。

---

## ライセンス

Copyright (c) 2026 SimplePaint. All rights reserved.

本ソフトウェアはプロプライエタリソフトウェアです。
ソースコードは公開されず、インストーラーによる使用のみ許可されます。
無断複製、修正および再配布は禁止されています。
