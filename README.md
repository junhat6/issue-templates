# Issue テンプレート (PBI / Task)

WE部 勉強会「良い Issue の書き方」の配布物です。考え方は 1 つだけ。

> Why と実現したい体験がはっきりしていれば、どんな How でもいい

## 入っているもの

| ファイル | 中身 |
|---|---|
| `.github/ISSUE_TEMPLATE/01-pbi.yml` | PBI 用のフォーム (ユーザーストーリー / Why / ユーザーに提供する体験 / 補足) |
| `.github/ISSUE_TEMPLATE/02-task.yml` | Task 用のフォーム (親 PBI / Why / How) |
| `.github/ISSUE_TEMPLATE/config.yml` | テンプレートを使わない Issue も立てられる設定 |
| `markdown/pbi.md` `markdown/task.md` | 同じ中身の Markdown 版 (フォームが使えない場所や、記事に貼る用) |

## 使い方

1. 自分のリポジトリに `.github/ISSUE_TEMPLATE/` をそのままコピーして、デフォルトブランチに push する
2. Issue を立てるときに「PBI」か「Task」を選ぶ

### Issue Type について

フォームの `type: PBI` / `type: Task` は、Issue Type を自動で付ける設定です。

- Issue Type は **Organization の設定** で作るもの。個人アカウントのリポジトリでは付かない
- Organization に `Task` は最初からあるが、`PBI` は無いので、Organization の Settings → Planning → Issue types で `PBI` を追加しておく
- Issue Type を使わないなら、各 yml の `type:` の行を消せばよい

## テンプレートを小さくしている理由

- Issue はやるべきことのメモ。欄が多いと立てるのが面倒になって、書き忘れる
- 立てる時点では、細かい仕様はまだ思いつかないことが多い
- 細かい仕様は、Issue のコメントで方針案・質問・メモを分けて詰めていく。PR を出してから「そもそも何で困ってたんだっけ？」とならないように、PR の前に Issue で合意を取る

参考: [IdeaBoost の実際のテンプレート](https://github.com/engineer-first/idea-boost/tree/develop/.github/ISSUE_TEMPLATE) / [蜂須賀大貴「AIでコードは書けるのに、つくりたいものがつくれないあなたへ」](https://www.docswell.com/s/PassionateHachi/KN73NR-2026-10-18-161120)
