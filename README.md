# FileMakerSampleSolutions
FileMaker サンプルソリューション
### :warning: <span style="color:red;font-weight: bold;">FileMaker 19 以降</span>では WebViewer 内の javascript から FileMaker.PerformScript() を実行するようにしています。Web ビューアの設定で <span style="color:red;font-weight: bold;">__[JavaScript による FileMaker スクリプトの実行を許可]__</span> にチェックが入っている必要があります。

### :warning: <span style="color:red;font-weight: bold;">FileMaker 16 - 18 </span>では、fmp:// からスクリプトを実行させる場合は、拡張アクセス権 <span style="color:red;font-weight: bold;">__[fmurlscript]__</span> の設定が必要になります。

## ■ TimestampPicker
iOS 標準のタイムスタンプピッカーの代替インターフェースをコピー&ペーストだけで他のソリューションに実装することができます。  
* 実装手順の動画 https://www.youtube.com/watch?v=d0CGZuOJSjU
### 変更履歴
* v1.3 (2020/05/21)
    * 	FM 19 の JavaScript web viewer integration に対応
* v1.2.5 (2019/05/23)
    * 	fmp URL スキームの変更
* v1.2.4 (2019/01/28)
    * 	カスタム関数 HolidayJ に祝日法の一部改正を反映
    * 	ポップオーバーが表示されているときのキーボード操作を追加 （Esc でキャンセル、Tab もしくは Return で完了してポップオーバーを閉じる、TimestampPicker の場合左右矢印キーでカレンダーと時計の切り替え）
    *  Picker の大きさを3種類利用できるように変更
* v1.2.3 (2018/10/30)
    * 	カスタム関数 HolidayJ に祝日法の一部改正を反映
* v1.2.2 (2018/07/19)
    * 	日付と時刻の2つのフィールドに別れていて1つのピッカーを利用する場合のサンプルを追加
* v1.2.1 (2018/06/20)
    * 	カスタム関数 HolidayJ に祝日法の一部改正を反映
* v1.2 (2018/01/17)
    * 	WebUI_DatePicker 関数の オプション_選択不可日 引数をリストで2つまで渡せるように変更 (今日以前と指定日以降の選択不可という選択期間が限定できるようになりました)
    * 	値を消去するためのボタンを設置
    * 	カードウインドウで利用する場合の処理追加
* v1.1.1 (2017/09/05)
    * Windows の 高DPI に対応
* v1.1.0 (2017/05/10)
    * FileMaker 16 に対応（TimestampPicker16.fmp12 は 16 以降のみで利用できます）
* v1.0.11 (2016/08/27)
    * オーバースクロール効果を無効にして iOS で WebViewer を固定するように変更
* v1.0.10 (2016/06/24)
    * FMPUrlScheme カスタム関数を変更
* v1.0.9 (2016/03/23)
    * 選択不可日が設定されている場合の前月次月/前年次年へのリンクを変更
* v1.0.8 (2016/03/21)
    * フィールド指定の代わりにグローバル変数の指定もできるように変更

## ■ CustomFormatExport
エクスポート順をユーザが自由に指定、ヘッダを付けたりフィールド内の改行の改行形式を垂直タブ以外にしたり文字コードを指定したりと、カスタムフォーマットの csv を書き出すことができます。

* 実装手順の動画 https://www.youtube.com/watch?v=yDWYm2JdhNs

### 変更履歴
* v1.0.4 (2020/05/21)
    * FM 19 の JavaScript web viewer integration に対応
* v1.0.3 (2019/05/23)
    * File-Base スクリプトステップに変更
    * CustomFormatExport18.fmp12 は 18 以降のみで利用できます）
* v1.0.2 (2018/05/10)
    * 出力する encoding に UTF-8 with BOM を追加
* v1.0.1 (2017/09/05)
    * Windows の 高DPI に対応
* v1.0.0 (2017/05/10)

## ■ fmQRcode
QR Code Generator for JavaScript  
https://github.com/kazuhikoarase/qrcode-generator  
を利用して FileMaker の値から QR コードを作成します。
### 変更履歴
* v2.0 (2020/05/21)
    * FM 19 の JavaScript web viewer integration を利用するよう全面的に書き直し（FM19以降のみ）
* v1.1.4 (2019/05/23)
    * fmp URL スキームの変更
    * qrcode.js のバージョンを 2019-02-15 版（v1.4.3）に変更
* v1.1.3 (2017/09/05)
    * qrcode.js のバージョンを 2017/07/28 版に変更
    * UTF-8 に対応
    * Windows の 高DPI に対応
* v1.1.2 (2017/05/10)
    * FileMaker 16 に対応
* v1.1.1 (2017/03/15)
    * 軽微な修正
* v1.1.0 (2017/01/11)
    * 利用している qrcode.js のバージョンを2017/01/04版に変更
    * encoding mode サポート（自動判別）/SVG 対応
* v1.0.10 (2016/08/25)
    * Windows で対象レコードの QR コードを作成する際のサンプルスクリプトを追加

## ■ fmBarCode
JsBarcode  
https://github.com/lindell/JsBarcode  
を利用して FileMaker の値からバーコードを作成します。  
対応するバーコード規格:  
CODE128 | CODE128A | CODE128B | CODE128C | CODE39 | JAN13 | JAN8 | JAN5 | JAN2 | UPC | ITF14 | MSI | MSI10 | MSI11 | MSI1010 | MSI1110 | pharmacode | codabar
### 変更履歴
* v2.0 (2020/05/21)
    * FM 19 の JavaScript web viewer integration を利用するよう全面的に書き直し（FM19以降のみ）
* v1.1.4 (2019/05/23)
    * fmp URL スキームの変更
* v1.1.3 (2017/09/05)
    * Windows の 高DPI に対応
* v1.1.2 (2017/05/10)
    * FileMaker 16 に対応
* v1.1.0 (2017/03/15)
    * 利用している JsBarcode.js のバージョンを v3.5.8 に変更し、結果を SVG でも受け取れるように変更
* v1.0.10 (2016/08/25)
    * Windows で対象レコードのバーコードを作成する際のサンプルスクリプトを追加

## ■ CropImage
Jcrop.js  
http://github.com/tapmodo/Jcrop  
を利用して、画像の任意の領域を切り抜きます。  
初出 : https://community.filemaker.com/message/167587
### 変更履歴
* v2.0 (2020/05/21)
    * FM 19 の JavaScript web viewer integration に対応
* v1.0.3 (2019/05/23)
    * fmp URL スキームの変更
* v1.0.2 (2017/09/05)
    * Windows の 高DPI に対応
* v1.0.1 (2017/05/10)
    * FileMaker 16 に最適化

## ■ SvgToPng
https://github.com/gabelerner/canvg
を利用して、SVG を PNG に変換してオブジェクトフィールドに保存します。  
__注意!__ 画像埋め込み SVG は変換されません。
### 変更履歴
* v2.0 (2020/05/21)
    * FM 19 の JavaScript web viewer integration を利用するよう全面的に書き直し（FM19以降のみ）
* v1.0.5 (2019/05/23)
    * fmp URL スキームの変更
    * canvg.js を 2019-05-18 版に変更
* v1.0.4 (2017/09/05)
    * Windows の 高DPI に対応
* v1.0.3 (2017/05/10)
    * FileMaker 16 に対応
* v1.0.2 (2016/06/24)
    * FMPUrlScheme カスタム関数に該当するステップを変更

## ■ ColorPicker
Colorwheel  
http://jweir.github.com/colorwheel  
を利用したカラーピッカーです。
### 変更履歴
* v1.1 (2020/05/21)
    * FM 19 の JavaScript web viewer integration に対応
* v1.0.5 (2017/05/23)
    * fmp URL スキームの変更
    * カラーホイールのサイズを 300px, 225px で利用できるように変更
* v1.0.3 (2017/08/15)
    * Windows の 高DPI に対応
* v1.0.1 (2017/05/10)
    * FileMaker 16 に対応

## ■ SortViaSortFld
ソート用の番号を用いて任意のソート順で値一覧を作成します。    
bison さんが解説をしてくださっています。
https://bison.theblog.me/posts/833663
### 変更履歴
* v1.0.1 (2017/05/10)

## ■ CheckOverflow
印刷レイアウトでフィールド枠からテキストがはみ出している場合に、収まるようにフォントサイズを小さくします。
### 変更履歴
* v1.0.1 (2015/07/27)
    * FileMaker 14　の場合、フォーカス時に外側の影が付いているとその影を含んだサイズになるので、付けないようにレイアウトの修正

## ■ InfinitySlideControl
無限スライドコントロール  
3枚のスライドコントロールパネルを使って擬似的な無限スライドコントロールを作成します。

## ■ PayPalHere for FileMaker
PayPal Here API  
https://github.com/paypal/here-sideloader-api-samples  
を利用して FileMaker Go から [PayPal Here](https://itunes.apple.com/jp/app/paypal-here/id505911015?mt=8) を呼び出します 。  
PayPal Here の仕様変更等で使えなくなる可能性があります。  
自己責任で使用してください。  
動作確認を PayPal Here 2.2.1 でしています。
