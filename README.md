# SGLclientCanOperate

このファイルをダウンロードする後輩へ
Githubの使い方は動画とかで適当に学んでください。その辺に転がってます
YOUTUBEでgithubの使い方で検索すれば何件がでる
ダウンロードではなくcloneをおすすめします。ファイルがバカでかいのでclone以外は厳しい
以下このSGLについての解説
↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓

鍵配送指令書のアルゴリズムを変更してあるので注意
このバージョンに対応して動くのは
SGLServerCanOperateなので注意

DynamicPeerInformationのバグはまだ残ってるので動かすときに注意してください
→鍵交換の時にDynamicPeerInformation.xmlがID順に並んでないとエラーが起きる
例外処理も書かれてないので強制的にストップする
もし3人以上で交換するときはサーバーを立ち上げてクライアント全員がログインしたのを確認してから
DynamicPeerInformation.xmlがID順にならんでいるかをちゃんと確認してから鍵交換に入るとよい

そのほかのバグ
・本当にごくたまにGroupInfomation.Xmlがばぐる
→特定のユーザのIPとかが抜けてたりする
そういうときはサーバが動いているときでも直接編集しても問題ないから手で直すといい

・とにかくXML系のバグが多い
動かないとわかったらxml系のファイルを全部並べておかしい場所を探すこと
だいたいがDynamicPeerInformation.xmlに原因があることがおおいけどね

→XML系のバグについてはこのシステムのデータ保存をxmlからデータベースに変更すれば一発でなくなる
けどもうシステム全体がでかくなりすぎてデータベースを入れ込む気力がない(´;ω;｀)
やれたら頑張ってね


以下SGLのバグの責任と僕個人のぐち
↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓↓
ちなみに上のバグは（にしむらさん）の代と（さのさん）、さらに上の人の代とかがシステムを作った時から残っているエラーです
僕がいくつか直しておきましたが、まだ残ってます。
上の代の人たちの開発力がとにかくなかったようなのは間違いない
コード読んでるとたまにちゃんと書いてる人がいるけどだいたい汚いスパゲティコードになってるので
もう直しようがないです。僕はあきらめました。

※にしむらさんは(さ○)さんとか(いと○)さんとかのしりぬぐいまで頑張ったひとなのでよくやってくれたほうだと思います


ひとつ言っとくと僕が担当したプログラムにはバグはありません
めちゃくちゃがちがちに作りこんであるしユーザのタイプやマシンの変更など数百回は条件を変えてテストしたので
まずエラーはでない
もし出たらほかの先輩たちのバグです。あしからず
とりまSGLはでかすぎるのでもう触りたくないです
はっきり言ってSGLはバージョンも大量にあってどれが動くかわからん
上の人の代の研究を見ると「まじでお前それやる意味ないだろ」ってことやってる人も多いです
一回論文見るとまじで思います。「そのバージョンとかそのアルゴリズムとかそのプロトコル作る意味なくね」って突っ込みたくなる
論文が多々ある。まじでくそ
とにかくもしSGLを触るなら今自分がどのバージョンを使っていて誰と誰が作ったプログラムが入っているのかを把握してから
やらないと大変なことになります

僕の代から僕がうるさいことをいってgithubでバージョン管理をやるようになったけどそれまではひどかった
とにかくそういうことです

