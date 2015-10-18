ricty install
=============

## はじめに
macbook に font(ricty) をインストールする

## 環境
- OSX EL Capitan: 10.11
- homebrew: 0.9.5 

## 作業

```
# ricty フォーミュラをインストール
$ brew tap sanemat/font

# ricty をインストール
$ brew install ricty
・
==> Caveats
***************************************************
Generated files:
  /usr/local/Cellar/ricty/3.2.4/share/fonts/Ricty-Bold.ttf
  /usr/local/Cellar/ricty/3.2.4/share/fonts/Ricty-Regular.ttf
  /usr/local/Cellar/ricty/3.2.4/share/fonts/RictyDiscord-Bold.ttf
  /usr/local/Cellar/ricty/3.2.4/share/fonts/RictyDiscord-Regular.ttf
***************************************************
To install Ricty:
  $ cp -fv /usr/local/Cellar/ricty/3.2.4/share/fonts/Ricty*.ttf ~/Library/Fonts/
  $ fc-cache -vf
***************************************************

# 上記の表示に従い、以下のコマンドを実行
$ cp -f /usr/local/Cellar/ricty/3.2.4/share/fonts/Ricty*.ttf ~/Library/Fonts/
$ fc-cache -vf                                                                
```

## メモ
- homebrew tap 機能とは？
  公式以外のフォーミュラ(※1)を取り込む機能
  github アカウントにアップされているフォーミュラも取り込むことができる
  ※1: フォーミュラー = home brew のパッケージのこと
- fc-cache コマンド: build font information cache files 
- mac os version を表示するコマンド
  ```
  $ sw_vers
  ```

資料
----
- [フォント Ricty のインストール（Mac)](http://qiita.com/inouet/items/a7086139e94b80df3084)
- [これは便利！Homebrewに追加されたtapコマンド](http://tukaikta.blog135.fc2.com/blog-entry-204.html)
