# 基礎知識学習 第1回

## はじめに

- ライブラリとフレームワーク
  - ライブラリとは
    - 他のプログラムに何らかの機能を提供するコードの集まり。
    - ライブラリは、ユーザプログラムによって「呼ばれる」。
  - フレームワークとは
    - 処理の初期化、実行、終了までの流れを規定したもの。
    - フレームワークは、ユーザプログラムを「呼ぶ」。
    - ハリウッドの原則 / 制御の反転   
  - 参考サイト
    - [ライブラリとフレームワークの違い](http://qiita.com/heroyct/items/779cd66100a051056332)
    
- コーディング規約
  - 参考サイト  
    - [Javaコーディング規約](https://future-architect.github.io/coding-standards/documents/forJava/Java%E3%82%B3%E3%83%BC%E3%83%87%E3%82%A3%E3%83%B3%E3%82%B0%E8%A6%8F%E7%B4%84.html)
  
## CHAPTER01

1. Androidとは
    - 世界で最も普及しているスマートフォン用のOS。  
  [Smartphone Volumes Expected to Rebound in 2017 with a Five-Year Growth Rate of 3.8%, Driving Annual Shipments to 1.53 Billion by 2021, According to IDC](http://www.idc.com/getdoc.jsp?containerId=prUS42334717)
    - オープンソースライセンス。（Apache License 2.0）
      - WebKitのライセンスはLGPL。
      - LinuxカーネルとライブラリはGPL。
    - Google Play
      - 開発したアプリを公開するマーケット。
      - 登録手数料25ドルが必要。

2. Androidアプリケーションの開発
    - Androidプラットフォーム  
    [プラットフォーム アーキテクチャ](https://developer.android.com/guide/platform/index.html)
    - Androidアプリケーション開発に必要なもの  
    [システム要件](https://developer.android.com/studio/index.html#Requirements)
    - Intel HAXMについて

3. Android Studioのインストール
    - 6/28に実施済み。
    - マニュアル「1.Android Studioのセットアップ」を参照。

## CHAPTER02
  - 6/28に実施済み。
  - 以下のマニュアルを参照。
      - 2.Android Studioプロジェクトの作成
      - 3.Android Studioエミュレータの作成.pdf
      - 4.HP ProBook 430 G3 Notebook PC BIOSの設定
      - 5.ASUS ZenPad 10 実機デバッグの設定


## CHAPTER03

1. Androidのプロジェクト
    - Android Studioの基本画面
        - プロジェクトツールウィンドウ
        - ツールウィンドウ
        - エディタウィンドウ
    - プロジェクトの構成要素
      - app
          - manifests
          - java
          - res
      - Gradle Scripts

2. 画面を作成する
    - レイアウトエディタの画面
        - Paletteペイン  
        部品をビューと呼ぶ。
        - Designペイン
        - Propertiesペイン
        - Component Treeペイン
    - ビューの配置  
    ビューをDesignペインに配置することで画面を作成する。
        
3. アクティビティについて知る  
画面を構成するクラスをアクティビティと呼ぶ。
    - ボタンを追加する
    - ボタンを押した時の処理を記述する
    - アプリを実行してみる

4. 画面を追加する
    - 画像リソースを登録する
        - drawableフォルダ
    - 画像を画面に配置する

5. アクティビティの詳細
    - アクティビティとは  
    Androidの1つの画面に対応するもの。ビューの配置やイベント処理を記述する。
    - アクティビティのライフサイクル
        - 開始  
        onCreate() > onStart() > onResume()
        - 終了  
        onPause() > onStop() > onDestroy()
        - 再開  
        onStop() > onRestart() > onStart()
        - 強制終了  
        onStop() > onCreate()  
        onDestroy() > onCreate()

## CHAPTER04

1. じゃんけんアプリの構成
2. プレイヤーの手を選択する画面の作成
3. じゃんけんの結果画面を作成しよう
4. ConstraintLayoutの設定方法
    - ConstraintLayoutとは
        - Android Studio 2.3からのデフォルトのレイアウト。
        - ビューに対して「制約」を設定することで複雑なレイアウトを直感的に作成することができる。
        - 様々な画面サイズを持つAndroid端末において最適に表示される。
        - 参考サイト  
        [Androidアプリの新レイアウト「ConstraintLayout」をCheck It Out！](https://codezine.jp/article/detail/10228)
    - オートコネクト
    - Infer Constraints
5. インテントによる画面遷移
    - 新しく画面（アクティビティ）を開く時に使用する。
    - 遷移先の画面に渡すデータを格納する。
6. 共有プリファレンスによるデータの保存
    - 共有プリファレンスとは
        - Mapのようにキーと値のペアでデータを設定ファイルに保存するもの。
        - アプリケーションの設定値など少量のデータ保存に使用する。
        - 保存できるデータ型は以下のとおり。
            - String
            - boolean
            - int
            - long
            - float

## GitHub演習

1. 課題提出用リポジトリの作成
2. Fork（フォーク）
3. Clone（クローン）
4. プログラム修正
5. Commit（コミット）
6. Push（プッシュ）
7. Pull Request（プルリクエスト）


## 宿題

- CHAPTER04の残り
- CHAPTER05

