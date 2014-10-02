####Androidにおける単位について  

**(Pixels) px**   
実際の画面上のPixelがそのままの単位になります。  
たとえば、480px X 800pxの画面であれば、  
1pxは画面の1/480という事になります。  

**(Density-independent Piexels) dp**   
ディスプレイ解像度の物理的な密度に応じた抽象単位になります。  
160dpi(dots per inch)を基準にした単位で、1dpは160dpiの画面で1pixelになります。  
dpとpixelの比率は画面密度(dpi)によって変化しますが、必ずしも正比例ではありません。  

**(Scale-independent Pixels) sp**   
画面上のサイズはユーザのフォントサイズ設定に準じます。  

##アイコン大きさ一覧  

|アイコン| mdpi | hdpi | xhdpi | xxhdpi |
|:--|:-:|:-:|:-:|:-:|
|DPI|160|240|320|480|
|倍率|1.0|1.5|2.0|3.0|
|ランチャー|48 x 48<br>42 x 42|72 x 72<br>64 x 64|96 x 96<br>84 x 84|144 x 144<br>126 x 126|
|アクションバー<br>ステータスバー<br>タブ|32 x 32<br>24 x 24|48 x 48<br>36 x 36|64 x 64<br>48 x 48|96 x 96<br>72 x 72|
|ダイアログ|32 x 32<br>24 x 24|48 x 48<br>36 x 36|64 x 64<br>48 x 48|96 x 96<br>72 x 72|
|リストビュー|32 x 32<br>24 x 24|48 x 48<br>36 x 36|64 x 64<br>48 x 48|96 x 96<br>72 x 72|
|通知|24 x 24<br>22 x 22|36 x 36<br>33 x 33|48 x 48<br>44 x 44|72 x 72<br>66 x 66|

##素材つくり  

|mdpi|hdpi|xhdpi|xxhdpi|
|:-:|:-:|:-:|:-:|
|0.5倍|0.75倍|1倍|1.5倍|

##デザインパターン
**基本的な高さは48dpを使用する**  
![metrics_48.png](https://qiita-image-store.s3.amazonaws.com/0/38558/506b1111-f295-5258-e922-75315563fde2.png "metrics_48.png")  

**ViewとViewの間は8dp 隙間は4dpを指定する**  
![metrics_closeup.png](https://qiita-image-store.s3.amazonaws.com/0/38558/d70230bd-e809-40c7-126b-145cb1226f33.png "metrics_closeup.png")  


![metrics_forms.png](https://qiita-image-store.s3.amazonaws.com/0/38558/4f9514f3-2232-21b5-f015-c407ea99b58a.png "metrics_forms.png")  

###ActionBarの高さ       
|Qualifier|Dimension|
|:--|:-:|
|縦向き|48dp|
|横向き|40dp|
|タブレット|56dp|

###Text Size
|Type|Dimension|
|:--|:-:|
|Micro|12sp|
|Small|14sp|
|Medium|18sp|
|Large|22sp|

##画像の名前
**a-z,0-9,_**　のみしか使用できません。  
画像作成者は基本的にこの名前を使用して下さい。  
9patch画像は画像の名前の後に **.9** を付けてください。  

###一般的な画像

|Asset Type|Prefix|Example|
|:--|:--|:--|
|Action bar|**ab_**|ab_stacked.9.png|
|Button|**btn_**|btn_send_pressed.9.png|
|Dialog|**dialog_**|dialog_top.9.png|
|Divider|**divider_**|divider_horizontal.9.png|
|Icon|**ic_**|ic_star.png|
|Menu|**menu_**|menu_submenu_bg.9.png|
|Notification|**notification_**|notification_bg.9.png|
|Tabs|**tab_**|tab_pressed.9.png|

###アイコン

|Asset Type|Prefix|
|:--|:--|:--|
|Icons|**ic_**|
|Launcher icons|**ic_launcher**|
|Action bar icons|**ic_menu**|
|Status bar icons|**ic_stat_notify**|
|Tab icons|**ic_**|
|Dialog icons|**ic_dialog**|

###ボタンの状態
|State|Suffix|Example|
|:--|:--|:--|
|Normal|**_normal**|btn_order_normal.9.png|
|Pressed|**_pressed**| btn_order_pressed.9.png|
|Focused|**_focused**|btn_order_focused.9.png|
|Disabled|**_disabled**|btn_order_disabled.9.png|
|Selected|**_selected**|btn_order_selected.9.png|
  　
##参考リンク
###Graphic Generators
>
[Android Asset Resizer](https://github.com/twaddington/android-asset-resizer)  
[Android Asset Studio](http://android-ui-utils.googlecode.com/hg/asset-studio/dist/index.html)  
[Android Button Maker](http://angrytools.com/android/button/)  
[Android Holo Colors IntelliJ Plugin](https://github.com/jeromevdl/android-holo-colors-idea-plugin)  
[Device Art Generator](http://developer.android.com/distribute/promote/device-art.html)  
[Google Play Badges](http://developer.android.com/distribute/googleplay/promote/badges.html)  
[Android DesignPattern](http://android-design.teamegg.co.jp/)

[参考URL](http://petrnohejl.github.io/Android-Cheatsheet-For-Graphic-Designers/)  
Thanks for Petr Nohejl.  
Copyright © 2013 Petr Nohejl, www.petrnohejl.cz  

