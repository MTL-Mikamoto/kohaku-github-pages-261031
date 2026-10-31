# MTL Kohaku-Entry 技術コラム

Jetson Orin Nano・MTL-MC300・EtherCAT・DDモーターによる8軸構成と模倣学習を紹介する静的サイトです。

## 構成
- index.html：本文・構成図
- assets/system-config.png：システム構成の画像
- assets/teaching-example.png：教示データの例（位置とトルク）
- assets/system.jpg、assets/adaptation.jpg：動画のポスター画像
- assets/demo-system.mp4：システム全景のデモ
- assets/demo-adaptation.mp4：位置変更時のデモ
- assets/product-reference.png：製品の参考画像
- .nojekyll：静的ファイルとして配信

## ローカルで見る
index.html をブラウザーで開いてください（assets フォルダーは同じ場所に置きます）。動画は音声なし・ブラウザー対応のH.264形式です。

## GitHub Pagesで公開する
Settings → Pages → Build and deployment → Source を「Deploy from a branch」、Branch を main、フォルダーを「/(root)」にして Save します。

## 記事の前提
- 250µsはEtherCATの通信周期です。AIの推論周期・カメラの撮影周期とは区別しています。
- 全8軸の個別割り当てとMTL-MC300の台数は記載していません。図は機能構成図です。
- モデルの学習は、Jetsonとは別のPCで行いました。
- 公開サイトでは、動画を含む掲載ファイルが閲覧・取得できます。
