---
last_reviewed: 2026-07-12
---

# bulldon-brand

> **層：運用層（operations）｜事実変化はAIが差分提示→承認後に更新可。**

## このリポジトリについて
ブルドン合同会社およびプロダクト群のブランドガイドライン集。
GitHub Pagesで公開。

**publicリポジトリ**（GitHub Pages・履歴含め全公開）。禁止物は法律層 `../.claude/rules/public-repo-guard.md` を正本とする。

## ファイル構成
- index.html : 入口ページ
- Bulldon_Corporate_Brand_Guidelines.html : 法人ブランド（レンダリング・見せ方）
- B-PASS_Brand_Guidelines.html : B-PASSプロダクトブランド（レンダリング・見せ方）
- Samurai_Shimonz_Brand_Guidelines.html : サムライシモンズブランド（レンダリング・見せ方）
- brand-tokens.md : ブランドトークン正本（色・フォント・コピーの機械可読な値。値の一次情報はこちら）

## 開発ルール
- ブランドカラー・タイポグラフィ・ロゴ使用ルールを定義
- 各プロダクトのデザイン判断時に参照する
- 内容変更時は関係者（COO・CGO）と合意してから更新

## 関連
値の正本は `brand-tokens.md`（本リポ内）。統治規則（ゾーン適用ルール・変更手続き）は `../.claude/rules/brand-design.md` を参照。`bull-don.hp/docs/HANDOVER_to_ClaudeCode.md` 4章は歴史文書（値の正は `brand-tokens.md`）。

## 上位ルール

ワークスペース `../.claude/rules/`（bulldon-workspace）を継承（commit-style / _meta-rules / brand-design / public-repo-guard）。
GAS リポジトリではないため `gas-architecture.md` / `b-pass-design.md` は対象外。全体の正本は `../AGENTS.md`。
