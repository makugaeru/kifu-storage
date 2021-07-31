kifPlayer

■概要
------------------------------------
kifPlayerは、ブラウザ上で将棋の棋譜を再生するプレイヤーです。
JavaScript製・レスポンシブで、KIF形式のファイルに対応します。

■使い方
------------------------------------
属性「type="kif"」を持つタグを用意し、中に「KIF形式のテキスト」か「KIFファイルのURL」を貼り付けます。

<script type="kif">
ここに「KIF形式のテキスト」か「KIFファイルのURL」を貼り付ける
</script>

<script type="kif">
http://example.com/example.kif
</script>

■便利な使い方
------------------------------------
◆開始時に任意の手数から始める。

kifタグにstart属性を追加します。
例えば5手目から開始したい場合は、次のようにします。

<script type="kif" start="5">

最終手から開始したい場合は-1としてください。


◆開始時に盤を反転して始める。

kifタグにreverse属性を追加します。

<script type="kif" reverse>


◆特定の名前が後手の場合、開始時に盤を反転して始める。

kifタグにmyname属性を追加して、値に名前を入力してください。部分一致で可・

<script type="kif" myname="example">


■クレジット
------------------------------------
・kifPlayerは誰でも自由に利用できます。(パブリックドメイン)
・KIF形式の仕様 http://kakinoki.o.oo7.jp/kif_format.html
