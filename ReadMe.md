mi用JavaScriptモードファイル
=======================

 <img width='600' src='http://nodaguti.usamimi.info/img/mi_javascript_mode_window.png' />

#インストール方法

「JavaScript」フォルダを、Library/Application Support/mi/mode/のなかに入れてください。<br/>このフォルダは、miのmi > モード設定... の「モード設定フォルダを開く」を押すと開くことができます。


#Features

### 目にやさしいコントラスト

暗めの背景と明るい文字色を使うことで、長時間のプログラミングの際も目が疲れません。


### 大半のキーワードを登録済み

もうdocument.getElementsByClassNameなんていちいち入力しなくても大丈夫。

予約語はもちろんのこと、Array, Dateといった組み込みのオブジェクトのプロパティ/メソッド名や、DOMのほとんどのプロパティ/メソッド名を予め登録してあるので、コード入力中にescもしくはCtrl+スペースを押すだけでコードの補完候補が現れます。

さらに、予約語の場合は文字色が黄色になるため、誤って予約語を使用することを避ける事ができます。


### 関数を見出しとして自動設定

関数名、メソッド名を見だしリストに自動的に登録します。

コード内でのインデントが適切に再現されるので、どのオブジェクトのメソッドかが一目瞭然。また、引数が表示されることで、コーディング中に素早く引数の種類・順番を確認することができます。

さらに、関数名はキーワードに登録されるので、まるで高機能IDEのように、自作関数名までコード補完機能の対象となります。
  
 
### 自動インデントの強化

mi標準の自動インデント機能（改行時に前の行と同じだけインデントする）に加え、function, Object, for, while, if, do ~ whileの記述を発見すると、次の行は自動的にインデントが1段深くなります。


### 拡張子の自動判定

末尾が.jsで終わるファイルはもちろんのこと、JavaScriptコードモジュールで用いられる.jsmファイルにも対応しています。


### 便利なツール群を搭載

- JSDocのコメントを挿入

    [JSDoc](http://www12.atwiki.jp/aias-jsdoctoolkit/)のコメントをカーソルの位置に挿入します。

- JSDoc Toolkitでドキュメントを作成

    表示中のファイルのドキュメントを作成します。toolkitの位置は、デフォルトではホームディレクトリとなっていますが、「ツール設定」画面より変更することができます。


# Known Issues

- 候補ウィンドウにおいて、文字色と背景色が同じ白のため文字が見えない。

    mi側のバグによるものです（[#712](http://proj.mimikaki.net/mi/ticket/712)）。

- キーワードの「無効にする」にチェックが入っているのにも関わらず候補ウィンドウに表示される。

    mi側のバグによるものです（[#713](http://proj.mimikaki.net/mi/ticket/713)）。