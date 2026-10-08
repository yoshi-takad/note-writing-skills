# note記事づくりスキル

noteの記事を、あなた自身の経験と考えから、6ステップで設計して書くためのスキル集です。AIが体験を作り話さないように、質問しながら進めます。

## AIに頼んで始める(かんたん)

使っているAIに、このページのURLを送って、次のように頼んでください。

> このURLのスキルを、私のAIに入れて使えるようにして。

AIは `AI_INSTALL.md` を読んで、環境に合わせて準備します。スマホのチャットなど、AIが自分でスキルを入れられない環境では、会話の中でそのまま記事づくりを手伝います。

## AIの方へ

このリポジトリのURLを渡されたら、先に **[AI_INSTALL.md](AI_INSTALL.md)** を読み、その手順を実行してください。

## 入っているもの

| スキル | 向いている記事 |
|---|---|
| `note-essay-writing` | 想い・価値観、制作背景、作品やサービスのコンセプト、素材や技法の意味、お客様との出会いなど |
| `note-howto-writing` | 実際にやってみた作業の記録、AI活用・ツール導入・自動化などのノウハウ記事 |
| `yomiyasu` | 不自然な日本語を直す仕上げ。上の2つが最後に使います |

### 6ステップ

1. 伝えたいこと
2. ポイント
3. 理由・背景(あなたの経験や記録)
4. 伝えたい人
5. 補足・フォロー(読む人の目で読み直す)
6. 順番

本文を書く前に、この設計メモを見せて確認をもらいます。

## 環境別の導入

| あなたの環境 | 方法 |
|---|---|
| スマホのチャットだけ | `paste/note-writing-prompt.md` をコピーして、会話の最初に貼る |
| パソコンのClaude(ブラウザ・デスクトップ) | `dist/` の3つの `.skill` ファイルを、設定のスキルから1つずつアップロードする |
| Claude Code | AIにURLを渡す。手動なら下のコマンド |
| Codex | AIにURLを渡す |

Claude Codeで手動で入れる場合:

```
/plugin marketplace add yoshi-takad/note-writing-skills
/plugin install note-writing-skills@note-writing-skills
```

スマホのアプリでスキルのアップロードができるかは、確認できていません。パソコンで一度アップロードすると、同じアカウントのスマホでも使える可能性がありますが、これも未確認です。

## 同梱しているもの

不自然な日本語を直す `skills/yomiyasu` は、nanaism さんが MIT License で公開している [yomiyasu](https://github.com/nanaism/yomiyasu) を、ライセンス表記つきで同梱しています。詳しくは [NOTICE.md](NOTICE.md) を見てください。

yomiyasu は文体を整えるスキルです。ほかに文体を調整するスキルを同時に有効にしていると、指示が干渉して、文章が乱れることがあります。

## ライセンス

このリポジトリのスキル(`note-essay-writing`、`note-howto-writing`、`paste/`)は MIT License です。`skills/yomiyasu` は、元の作者の MIT License に従います。
