---
last_reviewed: 2026-07-11
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
| Light Gold | ⚠️ **要確認：COO・CGO合意待ち（値がdrift中・暫定値は使用しないこと）** | `B-PASS_Brand_Guidelines.html:24` は `#E8D5A3`、`bull-don.hp/docs/HANDOVER_to_ClaudeCode.md:123` は `#EBD5A3`。1文字差でどちらが正か判定不能（参考事実：現行実装 bull-don.hp は `#EBD5A3` を使用中） |
| Dark Gold | `#9E843F` | 出典間で一致 |
| Gold（背景用） | `rgba(197, 165, 90, 0.15)` | HANDOVER のみに存在（要約表からは欠落していた値） |

## サムシモ ゾーンカラー（`bull-don.hp` の `/business/shimonz` で使用可）

| 名称 | 値 | 出典・備考 |
|---|---|---|
| Orange | `#F97316` | 出典間で一致 |
| Deep Orange | `#EA580C` | 出典間で一致 |
| （3色目） | ⚠️ **要確認：COO・CGO合意待ち（値がdrift中・暫定値は使用しないこと）** | 同名トークンの値がdrift：HANDOVER:132「warm-yellow」`#FCC24B` vs `Samurai_Shimonz_Brand_Guidelines.html:24`「warmYellow」`#FCD34D`（参考事実：現行実装 bull-don.hp は `#FCC24B` を使用中）。加えて同HTML:23「lightOrange」`#FDBA74` はHANDOVER側に対応トークンが存在しない別色（HTML側はオレンジ系4トークン構成）。本ファイル新設作業中に新規検出。brand--02が記録したLight Gold drift とは別件 |
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
