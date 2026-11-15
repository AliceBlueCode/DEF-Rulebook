# DEF-Rulebooks

[DEF](https://github.com/AliceBlueCode/DEF) の TRPG モードで使うルールブックとシナリオを集めたリポジトリです。
コードは入っていません（ルールシステムの実装はプラグインとして、別に読み込みます）。

## 使い方

1. このリポジトリを手元に取ってきます。

   ```bash
   git clone https://github.com/AliceBlueCode/DEF-Rulebooks.git
   ```

2. DEF の `.env` に、取ってきた場所を書きます（`;` 区切りで複数書けます）。

   ```dotenv
   TRPG_RULEBOOK_REPO_PATHS=/path/to/DEF-Rulebooks
   ```

3. DEF を起動し直すと、TRPG モードのルールブックの一覧に出ます。

## 中身

| フォルダ | 内容 | ライセンス |
|---|---|---|
| `def_original/` | DEF(仮)ルールと、サンプルのシナリオ | CC BY-SA 4.0 |
| `template/` | 新しいルールブックを作るためのテンプレートと、形の説明（`SCHEMA.md`） | CC0 1.0 |

ライセンスはフォルダごとに分かれています。各フォルダの `LICENSE` を見てください。
`template/` は CC0 なので、テンプレートから作ったルールブックは、作った人が自分のライセンスで公開できます。

## フォルダの形

```text
<フォルダ>/
  manifest.json      利用条件・クレジット・外部への送信とオンラインの可否
  LICENSE
  rulebooks/<id>.json
  scenarios/<id>.json
```

1つのリポジトリに1つのルールブックだけを入れる形（直下に `manifest.json` を置く）も、DEF は読めます。

## 載せないもの

権利者の許しの無いルールのデータは、このリポジトリに入れません。

---

# DEF-Rulebooks (English)

Rulebooks and scenarios for the TRPG mode of [DEF](https://github.com/AliceBlueCode/DEF). This repository holds data only;
rule-system code is loaded separately as plugins.

1. `git clone https://github.com/AliceBlueCode/DEF-Rulebooks.git`
2. Set `TRPG_RULEBOOK_REPO_PATHS=/path/to/DEF-Rulebooks` in DEF's `.env` (separate several paths with `;`).
3. Restart DEF. The rulebooks appear in the TRPG mode rulebook list.

Licenses are per folder: `def_original/` is CC BY-SA 4.0, `template/` is CC0 1.0. See each folder's `LICENSE`.
Rule data without the rights holder's permission is never added here.
