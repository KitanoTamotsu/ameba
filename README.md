## 　　Lesson23.　スクリプトフィルターをワークフローの途中で使う  
#### 開発メモ
### 1.ScriptFilterを後続で使ってみた
　いままで、ScriptFilterはワークフォローの先頭でしか利用していませんでしたがなんとなくフロー途中で使ってみました。
<br>　フローとしてはこんな感じ
<br>
<br>　keyword　→　Randomユーティリティ　→　ScriptFilter　　→　OpenURL
<br>
<br>　アメーバブログのRSSのURLで可変となるID部分は、Randomユーティリティで設定していて
<br>　スクリプトでは$1として利用できます。
<br>　とするとScriptFilterのkeywordは必要なさそうです。
<br>
<br>　試しに???としてみても動きには影響しませんでした。
<br>　最終的にはキーワドをブランクとしています。
### 2.Randomユーティリティ
　普段アメーバブログは見ません。芸能人のブログというイメージがありほとんど興味がありませんでした。
<br>　今回のサンプルとしていくつか選んで.Randomユーティリティのワードリストとしています
<br> 
<br>　アメーバブログのURLで下記のxxxxxxの部分が、アメーバIDですので、
<br>　もしお好きなアメーバブログがあるようでしたらワードリストをカスタマイズしてください
<br>　https://ameblo.jp/xxxxxx/
### 3.カスタマイズ
　今回はScriptFilterを途中でも利用できるということでのサンプルですが、
<br>　今までのLessonから、下記の作り込みができるでしょう
<br>　挑戦してみてください
<br>
<br>　・閲覧しているアメーバブログのURLからIDを取得して、テキストとして保存する
<br>　・Randomユーティリティのワードリストを上記テキストから読み込む
<br>　・Alfredに表示させるRSSの記事一覧を次ページ、前ページとしてコントロールする
<br>
#### 背景
　たまたま、アメーバブログのRSSが、https://ameblo.jp/[アメーバID]/rss20.xmlという汎用的なものだと知りました。
<br>　Lesson14のRSSマニアで作ったScriptFilterがそのまま使えたので、[アメーバID]をランダムに取得出来るようにしてみました。
　
<br>　
#### 取扱説明
### 機能:
　アメーバブログRSSをランダムに表示します
### インストール:
　1.[Alfredworkflow](https://github.com/KitanoTamotsu/ameba/releases/download/1.0/ameba.alfredworkflow.zip)をダウンロード 
<br>　2.ファイルをダブルクリックしてワークフローに登録
### 使い方:
　キーワード『ameba』で起動
<br>
<br>
[トップページに戻る](https://kitanotamotsu.github.io/)

