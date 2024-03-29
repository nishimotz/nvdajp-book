オブジェクトナビゲーション
----------------------------

アクティブウィンドウの読み上げ
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

Windows を直接操作しないで画面に表示されている情報を読み取る機能として、
NVDA には
レビューカーソル、あるいはオブジェクトナビゲーションとよばれるものがあります。

視力のある人がこの内容を学習したり、学習者のサポートをするときには、
「アドオンの活用」の章で紹介している「フォーカスハイライト」アドオンを
入れておくことをお勧めします。

NVDA で使われる「オブジェクト」という言葉は Windows が画面表示に使う
「要素」や「部品」のことです。
慣れるまではユーザーガイドの「オブジェクトナビゲーション」と
「レビューカーソル」という言葉は同じことだと考えてください。
どう違うかは後ほど説明します。

ここでは Windows
の「ファイル名を指定して実行」ダイアログを取り上げます。

Windows+R を押すと以下のように報告されます：

「ファイル名を指定して実行 ダイアログ …」

なお、引用する例は以下の設定を想定しています：

-  音声設定「記号」「読まない」
-  オブジェクト表示設定「オブジェクトのショートカットキーの報告」「チェックなし」

NVDA には「アクティブウィンドウの読み上げ」という機能があります。
実はこの機能を使うと「レビューカーソル」は勝手に動いてしまうのです。

-  NVDA+B：アクティブウィンドウの読み上げ

押すと下記のように読み上げます。 （notepad
と読み上げている箇所は直前に入力したファイル名によって異なります）

「 ファイル名を指定して実行 ダイアログ
実行するプログラム名、または開くフォルダーやドキュメント名、インターネット
リソース名を入力してください。 画像
実行するプログラム名、または開くフォルダーやドキュメント名、インターネット
リソース名を入力してください。 名前(O): 名前(O): コンボボックス notepad
折りたたみ エディット notepad 選択 OK ボタン キャンセル ボタン 参照(B)…
ボタン 」

いくつか読み上げ操作を復習しましょう。

-  NVDA+T：ウィンドウのタイトルの読み上げ

押すと 「ファイル名を指定して実行」

-  NVDA+Tab：フォーカスの読み上げ

押すと 「エディット　フォーカス　notepad 選択」

これらはウィンドウが開いた直後に読み上げた情報と同じです。

「フォーカス」とは Windows におけるキーボード入力や操作の対象です。
文字を入力できる状態ではテキストカーソル（文字入力カーソル）があります。
マウスを動かして移動させることができるマウスカーソル（マウスポインタ）もあります。

NVDA
の「レビューカーソル」は、これらとは独立して動かせる「読み取り専用カーソル」なのです。

いまレビューカーソルはどこにあるのでしょう？

ラップトップ配列：

-  NVDA+Shift+O：レビューカーソルの要素（ナビゲーターオブジェクト）の確認

デスクトップ配列：

-  NVDA+テンキー5：レビューカーソルの要素（ナビゲーターオブジェクト）の確認

この操作をすると

「参照(B)… ボタン」

と報告されます。

もういちど説明すると、いまフォーカスは「エディット」にあり、
レビューカーソルは「ボタン」にあるのです。

どうですか？ 「レビューカーソル」を意識できましたか？

うっかり他のキー操作をするとフォーカスのある要素を操作してしまうので、
気をつけてください。

レビューカーソルが画面のどこかで四角形の場所を指しているときに、
その場所や大きさを知る方法もあります。

ラップトップ配列：

-  NVDA+Delete：レビューカーソルの要素の位置を報告

デスクトップ配列：

-  NVDA+テンキーDelete：レビューカーソルの要素の位置を報告

押すと例えば以下のように報告されます：

「オブジェクトは、画面左端から16.4パーセント、上端から91.2パーセントにあり、画面の幅の4.6パーセント、高さの2.4パーセントを占めています」

さて、わかりきったことかも知れませんが、レビューカーソルの要素に何が書かれているか、
確認しましょう。

ラップトップ配列：

-  NVDA+Shift+ピリオド：レビューの現在行の報告

デスクトップ配列：

-  テンキー8：レビューの現在行の報告

押すと 「参照(B)…」

すばやく2回押すと
「マイリ　アキラ　カッコ　ビー　カッコトジ　ピリオド　ピリオド　ピリオド」

すばやく3回押すと
「参考書のサン　照らすのショウ　半角カッコ　半角英字大文字ビー　半角カッコトジ　半角ピリオド　半角ピリオド　半角ピリオド」

レビューカーソルはいままで四角形だと説明してきたのですが、
それは「ボタン」の話です。
レビューカーソルは「ボタン」の中の文字を一つ一つ確認できるのです。

ラップトップ配列：

-  NVDA+ピリオド：レビューの現在の文字の報告

デスクトップ配列：

-  テンキー2：レビューの現在の文字の報告

1回または2回押すと： 「参考書のサン」

3回押すと： 「21442 u 53c2」

3回押すと文字コードを10進数と16進数で説明します。
テキスト（文字）の確認でご紹介した「文字単位の移動」で
ボタンの中を1文字ずつ左右に移動しながら確認できます。

ラップトップ配列：

-  NVDA+左矢印：前の文字に移動
-  NVDA+右矢印：次の文字に移動

デスクトップ配列：

-  テンキー1：前の文字に移動
-  テンキー3：次の文字に移動

最初は「ナビゲーターオブジェクトとレビューカーソルは同じ」と説明をしましたが、
ここではちょっと違います。
ナビゲーターオブジェクトは「参照」というボタンを指しています。
レビューカーソルはその中の文字を指しています。

ナビゲーターオブジェクトの移動
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

いよいよナビゲーターオブジェクトを動かしてみましょう。
このボタンのまわりには何があるのでしょう？

画面を構成する要素は

-  「親要素の下の階層に子要素がある」
-  「お兄さん要素と同じ階層に弟要素がある」

といった二次元の関係になっています。

「要素の位置の報告」機能で確認した画面の上下左右と区別するために、
ここでは「親子」「兄弟」という言葉で説明します。

家系図のようなものをイメージしてください。

この家系図では、親要素と子要素は上下に並びます。
また兄弟要素は左右に並びます。左側をお兄さんと呼びます。
この上下と左右がキー操作に対応しています。

レビューカーソルを要素単位で移動しましょう。

ラップトップ配列：

-  NVDA+Shift+右矢印：次の要素に移動

デスクトップ配列：

-  NVDA+テンキー6：次の要素に移動

押すと 「次のオブジェクトなし」

「参照(B)…」の右に兄弟要素がない、つまり「参照(B)…」が一番末っ子です。

ラップトップ配列：

-  NVDA+Shift+左矢印：前の要素に移動

デスクトップ配列：

-  NVDA+テンキー4：前の要素に移動

押すと順番に

-  キャンセル ボタン
-  OK ボタン
-  名前(O): コンボボックス notepad 折りたたみ
-  名前(O):
-  実行するプログラム名、または開くフォルダーやドキュメント名、インターネット
   リソース名を入力してください。
-  画像
-  前のオブジェクトなし

この「前のオブジェクトなし」がこの階層の左端を示します。
画像は長男、コンボボックスやボタンがその下の兄弟です。

それでは

「名前(O): コンボボックス notepad 折りたたみ」

というオブジェクトにいったん戻ってください。

さて、今度は親子関係を見ていきましょう。

以下を操作してください。

ラップトップ配列：

-  NVDA+Shift+下矢印：子要素に移動

デスクトップ配列：

-  NVDA+テンキー2：子要素に移動

以下が報告されます：

-  エディット notepad 選択

現在の要素を確認し直します：

ラップトップ配列：

-  NVDA+Shift+O：レビューカーソルの要素を確認

デスクトップ配列：

-  NVDA+テンキー5：レビューカーソルの要素を確認

押すと

-  「エディット　フォーカス　notepad　選択」

この状態で「前の要素に移動」「次の要素に移動」を使えば、
「エディット　フォーカス　notepad　選択」には他に兄弟の要素がいないことがわかります。

親要素に戻るのは上方向です。家系図をイメージしてください。

ラップトップ配列：

-  NVDA+Shift+上矢印：親要素に移動

デスクトップ配列：

-  NVDA+テンキー8：親要素に移動

押すと

-  名前(O): コンボボックス notepad 折りたたみ

さらに親要素はあるのでしょうか？ もう一度「親要素に移動」を押すと

-  「ファイル名を指定して実行　ダイアログ」

このダイアログはエディットやボタンなどの兄弟すべての親要素です。
このダイアログに兄弟要素はあるでしょうか？

「次の要素に移動」では何も見つかりません。

「前の要素に移動」を押していくと以下を確認できます：

-  閉じる ボタン ウィンドウを閉じます。
-  システム メニューバー ウィンドウを操作するコマンドが含まれています。

詳しい操作は省略しますが、「システム
サブメニュー」の子要素に「システム　サブメニュー」があります。
これはダイアログを開いてすぐに Alt
キーを押すと出てくるメニューと同じものです。
（このメニューの中には「移動」と「閉じる」のメニュー項目があります）

最初に見つかった「閉じる
ボタン」は標準的なウィンドウの右上にある赤いバツ印のついたボタンです。

レビューカーソルの位置のボタンを押す
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

ナビゲーターオブジェクトがボタンにあるときに、そのボタンを押すための操作を二通り説明します。

これらは Tab キーで移動できないボタンを押すときに役立ちます。

マウスクリックでボタンを押す
^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^

マウスクリックでボタンを押すためは
「マウスカーソルを移動する」「左クリックを実行する」の2段階が必要です。

ラップトップ配列：

-  NVDA+Shift+M：マウスカーソルを移動

デスクトップ配列：

-  NVDA+テンキースラッシュ：マウスカーソルを移動

押すと「閉じる」と読み上げます。
ナビゲーターオブジェクトとレビューカーソルの位置にマウスカーソルが移動して、
マウスカーソル位置のオブジェクトが報告されたからです。

続けて、以下を操作します。

ラップトップ配列：

-  NVDA+開き角括弧：左クリック

デスクトップ配列：

-  テンキースラッシュ：左クリック

押すとウィンドウが閉じて、その下のウィンドウやデスクトップなどにフォーカスが移ります。

なお、左クリックの操作を素早く2回繰り返すとダブルクリックができます。
右マウスボタンを押したり、マウスボタンを押し続けた状態（ロック）にすることもできます。
これらのテクニックは、マウスでの操作しか考慮されていないアプリで有用でしょう。

詳しくはユーザーガイドを参照してください。

-  `ユーザーガイド 5.7.
   マウスカーソルの移動 <https://www.nvda.jp/nvda2021.3.5jp/ja/userGuide.html#NavigatingWithTheMouse>`__

既定のアクションの実行
^^^^^^^^^^^^^^^^^^^^^^^^^^^^

このアプリがアクセシビリティに配慮して作られている場合、
具体的には「既定のアクション」をこのボタンに割り当てている場合には、
もっと簡単にボタンを押すことができます。

もう一度「ファイル名を指定して実行」ダイアログを開いてください。
今度は最初からレビューの操作で「閉じる ボタン」に移動しましょう。

ラップトップ配列：

-  NVDA+Shift+上矢印：親要素に移動
-  NVDA+Shift+左矢印：前の要素に移動

デスクトップ配列：

-  NVDA+テンキー8：親要素に移動
-  NVDA+テンキー4：前の要素に移動

押すと「閉じる　ボタン」

フォーカスのあるボタンはスペースで押せますが、
レビューカーソルからはボタンを次の方法で押します。

ラップトップ配列：

-  NVDA+Enter：レビューカーソル位置の要素で既定のアクションを実行

デスクトップ配列：

-  NVDA+テンキーEnter：レビューカーソル位置の要素で既定のアクションを実行

この「実行」という操作には「押す」「呼び出し」「アクションの実行」などの別名があります。
ボタンは押されたら何を実行するかが決まっていて、
その割り当てられた処理がこの操作で実行できます。

オブジェクトの親子関係
~~~~~~~~~~~~~~~~~~~~~~~~~~

「閉じる　ボタン」のもうひとつ上の階層は「ファイル名を指定して実行　ウィンドウ」です。
ダイアログを一般化したものがウィンドウだと理解してください。
その兄弟オブジェクトは、実は Windows デスクトップに
置かれているさまざまな部品やウィンドウです。
起動中のどのアプリのウィンドウにでも、またタスクバーやタスクトレイにも、
このレビューカーソルの移動でたどり着けるのです。
ぜひ、いろいろなウィンドウやアプリでレビューカーソルを試してみてください。

要素（オブジェクト）の親子関係について補足すると、
これはソフトウェアの開発者の都合で決まっています。

例えば親要素の色や位置情報を子要素が受け継ぐ、といった性質があるのです。

画面を見るだけのユーザーには親子・兄弟関係は正確にはわからないので、
要素の順序やつながりがきちんと配慮されておらず、
レビューカーソルでうまく移動できない、不必要に階層が複雑、
といったアプリは残念ながらたくさんあります。

あきらめないでチャレンジしてみてください。

レビューカーソルに関する設定
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

NVDAメニュー 設定「レビューカーソル」の項目を簡単に紹介します。

-  `ユーザーガイド 12.1.11.
   レビューカーソル <https://www.nvda.jp/nvda2021.3.5jp/ja/userGuide.html#ReviewCursorSettings>`__

以下の設定は、Windows
のフォーカス、文字カーソル、マウスカーソルが移動したときに
レビューカーソルを移動させるかどうかを指定します。

-  「システムフォーカス（フォーカス）を追跡」（キー操作はNVDA+7）
-  「テキストカーソル（文字カーソル）を追跡」（キー操作はNVDA+6）
-  「マウスカーソルを追跡」

普段はレビューカーソルはWindowsのフォーカスと一体化しています。
レビューカーソルを動かすとフォーカスとレビューカーソルは分離しますが、
Tabキーでフォーカスを動かすと、レビューカーソルはまたフォーカスにくっついてしまいます。
しかし NVDA+7 を押して追跡を無効にしておけば、
フォーカスを動かしてもレビューカーソルは動かず、分離されたままになります。

レビューモードの説明
~~~~~~~~~~~~~~~~~~~~~~~~

NVDA のレビュー操作には以下の3種類のモードがあります。

-  オブジェクト（要素）レビュー
-  ドキュメント（文書）レビュー
-  画面レビュー

切り替え操作は次のとおりです。

ラップトップ配列：

-  NVDA+PageUp：次のレビューモード
-  NVDA+PageDown：前のレビューモード

デスクトップ配列：

-  NVDA+テンキー7：次のレビューモード
-  NVDA+テンキー1：前のレビューモード

ウェブブラウザのようなアプリケーション（ブラウズモード）では
意識しなくても自動的にドキュメントレビューに切り替わります。

画面レビューでは要素（オブジェクト）内の行単位の移動が、
画面の改行位置で区切られます。
例えばNVDAメニューのヘルプ「NVDAについて」ダイアログで
「次のレビュー要素に移動」を2回押して見つかる、
テキストのたくさん書かれた要素を下記の操作で読み進めてみてください。

ラップトップ配列：

-  NVDA+下矢印：レビュー内の次の行に移動

デスクトップ配列：

-  テンキー9：レビュー内の次の行に移動

画面レビューに切り替えてこの操作を行うと以下のように区切られます。

-  「NVDAはGNU 一般公衆利用許諾契約書(Version 2)によって保護されていま」

-  「す。この内容に同意いただき、必要としている方にソースコードを提供していただける」

これは画面でこのように改行されて表示されているからです。

なお、マウスカーソルの移動は、画面レビューでは正しく動かないのでご注意ください。

