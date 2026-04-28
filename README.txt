dic.nicovideo-yamada
====================

■ 想定リポジトリ名
GitHub Pagesで公開する場合、リポジトリ名を下記のようにするとURLが少しニコニコ大百科風になります。

  dic.nicovideo-yamada
  dic-nicovideo-yamada
  dic-nico-yamada

例：
  https://ユーザー名.github.io/dic.nicovideo-yamada/

■ 開き方
index.html をブラウザで開いてください。
GitHub Pagesでは、このフォルダの中身をリポジトリ直下に配置してください。

■ 構成
index.html
  YAMADA本記事です。

style.css
  全ページ共通CSSです。用途別にコメントを入れています。

img/yamada-aa.png
  AA風イメージ画像です。

articles/*.html
  関連項目から遷移する暫定記事です。

video/truth.html
  関連動画クリック後のローディング演出ページです。
  URLの ?title=... に応じて表示タイトルが変わります。
  例: video/truth.html?title=山田君、立つ

robots.txt
  検索避け用の補助ファイルです。
  ただしGitHub Pagesのプロジェクトサイトでは robots.txt が必ず検索除外として働くとは限らないため、
  各HTMLにも noindex meta を入れています。

.nojekyll
  GitHub Pagesでファイル名をそのまま配信するための空ファイルです。

■ 検索避けについて
各HTMLの<head>内に下記を追加済みです。
  <meta name="robots" content="noindex,nofollow,noarchive,nosnippet,noimageindex">
  <meta name="googlebot" content="noindex,nofollow,noarchive,nosnippet,noimageindex">

完全なアクセス制限ではありません。
URLを知っている人は閲覧できます。

■ 注意
OneDrive等で共有する場合は、フォルダごと配置・共有してください。
単体HTMLだけを移動すると、CSSや画像の相対パスが切れます。


更新メモ v4:
- パンくずを「トップページ > 秋田県 > YAMADA > 各項目名」形式に統一。
- 掲示板見出しを「（各項目名）について語るスレ」に変更。
- 投稿フォーム風UIを追加（表示のみ・送信不可）。

更新(v5): パンくずのリンクを調整しました。トップページ/秋田県は飾り、YAMADAはindex.html、各関連項目は該当記事へのリンクです。
