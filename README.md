# Assignment-Manager-for-YNU-LMS

未提出（再提出）の課題をトップページで簡単に確認できるようにする拡張機能です。 
  
DOM操作(データ取得)は講義ページに**手動でアクセスした時のみ**なので、サーバーに大きな負荷をかけることなく課題管理が可能です。  
  
[クソデカ未提出](https://github.com/OhVIton/BigBigNotSubmitted-YNU-LMS-Firefox)とも共存可能です。

## 使用方法
講義ページを開くと、以下のように未提出または未回答の課題が表示されます。  
この時、課題の情報がブラウザ内に保存されます。
![lecture page](images/photo_00.png)
  
そして、そのデータベースの情報をもとに、LMSのトップページで課題一覧が表示されます。  
追加された情報はRemoveボタンを押すと削除できます。  
また、DEADLINEのリンクにアクセスすると、
![toppage](images/photo_01.png)
以下のようにGoogle カレンダーへの追加もできます
![googlecalendar](images/photo_02.png)

## xpiファイルからインストールする場合（開発者向け） 
Firefox 延長サポート版 (ESR)、Firefox Developer Edition および Nightly バージョンのみ対応
Firefox の設定エディター (about:config ページ) で xpinstall.signatures.required 設定の値を false に変更することで、アドオン署名の強制を無効にしてインストールしてね

これで完了。おめでとう。  
  
## サーバー負荷について
DOM操作(データ取得)はあくまで**講義ページを手動で開いたときのみ**なので、サーバー負荷は一般の利用時と変わらないと推測されます。  
