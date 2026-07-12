---
last_reviewed: 2026-07-12
---

# ブランドトークン正本

> **層：運用層（operations）｜事実変化はAIが差分提示→承認後に更新可。**

ブランドカラー・フォント・コピーライティング規則の機械可読な正本。`../.claude/rules/brand-design.md`（統治規則・ゾーン適用ルール・bulldon-workspace）と `bull-don.hp/AGENTS.md`（実装リポ側の短い導線）から参照される。

**値の変更（新しい色の追加・既存値の変更）は「内容変更」としてCOO・CGO合意を要する**（`AGENTS.md`「内容変更時は関係者（COO・CGO）と合意してから更新」）。本ファイルの新設自体は既存に合意済みの値を1箇所へ集約する構造整理であり、新方針の決定ではない（2026-07-11 清水裁定）。

## コーポレートカラー（ブルドンLLC本体）

| 用途 | 名称 | 値 |
|---|---|---|
| 背景（深） | DeepNavy | `#0F1B33` |
| 背景（淡） | Navy | `#1B2A4A` |
| テキスト | White | `#FFFFFF` |
| テキスト（副） | Slate400 | `#94A3B8` |
| テキスト（三） | Slate500 | `#64748B` |
| アクセント（主） | Blue | `#2563EB` |
| アクセント（淡） | LightBlue | `#60A5FA` |
| アクセント背景 | — | `rgba(37, 99, 235, 0.15)` |
| 罫線 | — | `rgba(255, 255, 255, 0.08)` |
| 罫線（強） | — | `rgba(255, 255, 255, 0.15)` |

bull-don.hp 実装の CSS 変数名：`--bg` / `--bg-soft` / `--text` / `--text-secondary` / `--text-tertiary` / `--accent` / `--accent-light` / `--accent-soft` / `--line` / `--line-strong`。

## B-PASS ゾーンカラー（`bull-don.hp` の `/business/bpass`、`bull-don.lp` 全体で使用可）

| 名称 | 値 | 出典・備考 |
|---|---|---|
| Gold | `#C5A55A` | 出典間で一致 |
| Light Gold | `#E8D5A3` | 2026-07-12、COO・CGO確認済みで確定（`B-PASS_Brand_Guidelines.html:24`と一致）。従来drift値`#EBD5A3`（`HANDOVER_to_ClaudeCode.md:123`旧記載・bull-don.hp/bull-don.lp実装の旧値）は本値へ統一済み。`bull-don.hp/docs/mockups/*.html`は本番導線に乗らない歴史的モックのため未更新（意図的・HANDOVER本文と同じ歴史記録扱い） |
| Dark Gold | `#9E843F` | 出典間で一致 |
| Gold（背景用） | `rgba(197, 165, 90, 0.15)` | HANDOVER のみに存在（要約表からは欠落していた値） |

## サムシモ ゾーンカラー（`bull-don.hp` の `/business/shimonz` で使用可）

| 名称 | 値 | 出典・備考 |
|---|---|---|
| Orange | `#F97316` | 出典間で一致 |
| Deep Orange | `#EA580C` | 出典間で一致 |
| Warm Yellow | `#FCD34D` | 2026-07-12、COO・CGO確認済みで確定（`Samurai_Shimonz_Brand_Guidelines.html:24`「warmYellow」と一致）。従来drift値`#FCC24B`（`HANDOVER_to_ClaudeCode.md:132`旧記載・bull-don.hp実装の旧値）は本値へ統一済み。なお同HTML:23「lightOrange」`#FDBA74`はHANDOVER側に対応トークンが存在しない別色（HTML側はオレンジ系4トークン構成。統合対象外） |
| Orange（背景用） | `rgba(249, 115, 22, 0.15)` | HANDOVER のみに存在（要約表からは欠落していた値） |

## フォント

| 用途 | フォント | CSS 変数 |
|---|---|---|
| 装飾・英字大見出し | Oswald | `--font-display` |
| 本文・日本語 | Noto Sans JP | `--font-body` |
| メタ情報・数字・英字小ラベル・コード | JetBrains Mono | `--font-mono` |

すべて `next/font/google` で読み込む。

## コピーライティング

- 体言止め・断定調を基本。過度な敬語・冗長な修飾を避ける。
- 「〜できます」ではなく「〜可能」「〜対応」等で締める。LP と同等トーンで統一。

## 関連

- ゾーン適用ルール（どのページでどの色を使ってよいか）の正本は `../.claude/rules/brand-design.md`（bulldon-workspace）。
- 実装向けの歴史的経緯・旧モック仕様は `bull-don.hp/docs/HANDOVER_to_ClaudeCode.md`（歴史文書・値の正は本ファイル）。
