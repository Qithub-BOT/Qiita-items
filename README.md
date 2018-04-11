## このリポジトリについて
プログラマのための技術情報共有サービス「[Qiita](https://qiita.com)」の記事を、Qiitaユーザーでコラボレーション（共同作成・編集）するための記事本文Markdownデータのリポジトリです。

## コラボレーションについて
**GitHubに置かれたMarkdownファイルが更新されるとQiitaの該当記事が更新される仕組み**になっており、`github` もしくは `git` を使える Qiita のユーザーであれば誰でも記事の編集・修正が行えます。

1. 編集したいQiitaコラボ記事の記事IDを探します。（Qiita上のURLの末尾の番号）
1. [`items`リポジトリ](https://github.com/Qithub-BOT/items)をローカルに Clone もしくは自分の GitHub に Fork します。
1. Clone／Fork先で新しいブランチを作成します。ブランチ名は「＜Qiita記事ID＞-＜日付 YmdHi＞」のフォーマットにします。
    - Forkした場合は、GitHubのWeb上から編集でき、変更の初回保存（コミット）時にブランチ作成を選びます。

1. 作成したブランチ内の該当記事を編集＆コミットします。
1. 編集が終わったらプルリクエスト（修正の反映依頼。**以下PR**）を行います。
1. QiitaユーザーによるPR内容のチェック後、特に問題がなければQiitaに修正が反映されます。

## チェックについて
PR のあった記事は、[Qiitadon](https://qiitadon.com/ "Qiitaのマストドン・インスタンス") の BOT「[Qithub](https://qiitadon.com/@qithub)」のフォロワーに通知されます。

通知に対し「:thumbsup:」（いわゆる LGTM ）の投票数が 10 件以上得られると承認され、"master" ブランチにマージされると同時にQiitaに反映（記事が更新）されます。

なお、**「Qithub」BOTのフォロワーからの PR の場合はチェックは行われません**ので、こまめに修正を行われたい方は Qiitadon でフォローすることをお勧めします。

## フォーマット

- ファイル名： `<Qiita記事ID>.md`
- 初回投稿先： `https://qiita.com/Qithub/private/<Qiita記事ID>`（限定共有で公開 ※）
- 最終投稿先： `https://qiita.com/Qithub/items/<Qiita記事ID>`
- タイトル　： 本文の１行目がQiita記事のタイトルになります。２行目には改行を必ず入れてください。
- タグ　　　： 本文の３行目がQiita記事に付けられるタグになります。４行目には改行を必ずいれてください。
- メインの記事内容： 本文の５行目から通常のQiita記事のMarkdownで記入してください。記述できる内容もQiitaのMarkdown記法に準拠します。（後述する画像を除く） 

※ 後述するBOTのフォロワーの :thumbsup: が１０以上得られると、Qiita記事のステータスが「限定共有」から「公開」に変わります。



