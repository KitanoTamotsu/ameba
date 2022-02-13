#### 開発メモ
ワークフロー
<br><img width="600" src="https://user-images.githubusercontent.com/40127279/127756932-1f627195-1442-46ef-bf3d-27d4a9bbcf2b.png">

### 1.ScriptFilterを後続で使ってみた
　いままで、ScriptFilterはワークフローの先頭でしか利用していませんでしたがなんとなく
<br>　フロー途中で使ってみました。
<br>
<br>　keyword　→　Randomユーティリティ　→　ScriptFilter　　→　OpenURL
<br>
<br>　アメーバブログのRSSのURLで可変となるID部分は、Randomユーティリティで設定して
<br>　いるので、ScriptFilterのkeyword入力は必要なさそうですね
<br>　試しにkeywordを???としてみても動きには影響しませんでした
<br>　最終的にはキーワドをブランクとしています
<br>　
<br>　<img width="600" src="https://user-images.githubusercontent.com/40127279/127757053-78b122d7-20be-47e5-b4a6-04555fefb269.png">

### 2.Randomユーティリティ
<br>　今回のサンプルとしていくつか選んでRandomユーティリティのワードリストとしています
<br>　ただ普段アメーバブログを見ないので、ほんとうに適当な選択です
<br>　
<br>　アメーバブログのURLで下記のxxxxxxの部分が、アメーバIDですので、
<br>　もしお好きなアメーバブログがあるようでしたらワードリストをカスタマイズしてください
<br>　https://ameblo.jp/xxxxxx/
<br>　
<br>　<img width="480" src="https://user-images.githubusercontent.com/40127279/127757069-e259ddbf-3258-4d9d-95a4-95fcd383176e.png">
　
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
　たまたま、アメーバブログのRSSが、https://ameblo.jp/[アメーバID]/rss20.xmlという
<br>　汎用的なものだと知りました
<br>　Lesson14のRSSマニアで作ったScriptFilterがそのまま使えたので、[アメーバID]をランダムに
<br>　取得出来るようにしてみました
　
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

