# イントロダクション

## JavaScript の歴史

### 不遇の時代を経てきた JavaScript

- 1990年代といえば、ダイナミック HTML という、JavaScript を使った Web サイトの作成手法が流行した。

### 復権のきっかけは Ajax、そして HTML5 の時代へ

- HTML5 では、マークアップ機能が充実されただけでなく、アプリ開発のための JavaScript API が強化された。
- HTML5 によって、ブラウザネイティブな機能だけ実現できる範囲が格段に広がった
- スマホ・タブレットの普及による RIA の衰退
  - RIA: Rich Internet Application。Flash や Silverlight などのプラグインを使った Web アプリケーションのこと。
- SPA の台頭
  - SPA: Single Page Application。ページ遷移を伴わない Web アプリケーションのこと。
  - 初回のアクセスでは、まずページ全体を取得する。以降のページ更新は基本的に JavaScript で行う。
  - JavaScript だけで処理しきれない、サーバーサイドの処理は Ajax などの非同期通信を利用して実装する。

## フレームワークとは？

### フレームワークの本質

- フレームワークとは、問題に対する定石（イディオム）、または設計面での方法論を「再利用可能なクラス」という形でまとめたものをいう

- ライブラリ
  - ユーザーコードから呼び出されるべきもの
- フレームワーク
  - ユーザーコードがフレームワークによって呼び出される
- ライブラリとフレームワークの違い
  - ライブラリは、ユーザーコードがライブラリを呼び出す
  - フレームワークは、フレームワークがユーザーコードを呼び出す
  - IoC（Inversion of Control）: ユーザーコードがフレームワークにコントロールを渡すこと

### フレームワーク導入の利点

1. 開発生産性の向上
2. メンテナンス性に優れる
3. 先端の技術トレンドにも対応しやすい
4. 一定以上の品質が期待できる

## Angular の特徴

- フルスタックのフレームワークである
  - HTML ベースのテンプレートエンジン
  - コンポーネント/テンプレート間のデータバインディング機能
  - コンポーネント/サービス間の依存関係を解決する DI コンテナ
  - 文書ツリーを操作するためのディレクティブ
  - 表示すべき値を加工するためのパイプ
  - ビジネスロジックを実装するためのサービス
  - URL に応じてページを振り分けるルーティング機能
  - 単体テスト/システムテストを支援するテストフレームワーク
- コンポーネント指向である
  - コンポーネントとは、ページを構成する UI 部品のこと
    - ビュー（HTML テンプレート）
    - ロジック
    - コンポーネントを構成するメタ情報
- モダンな技術をふんだんに取り入れている
  - TypeScript
    - C# によく似た構文を持つ、JavaScript の拡張言語
  - SystemJS
    - モジュールを動的にロードするためのライブラリ
  - RxJS
    - JavaScript で非同期処理を実装するためのライブラリ
  - Zone.js
    - 非同期処理のコンテキストを管理、操作するためのライブラリ
- 開発言語には TypeScript がおすすめ
- ドキュメント/周辺ライブラリが充実している

### Angular のバージョン

- AngularJS（1.x）: 2010年10月リリース
- Angular（2.x 以降）: 2016年9月リリース
  - Angular 2 は、AngularJS とは全く別のフレームワーク
  - Angular 2 以降は、Angular という名前でリリースされている
  - 基本的に AngularJS との互換性はない

[!NOTE]
- Angular3 は存在しない。Angular 2 から Angular 4 に直接進化した。

- Angular のバージョンポリシー
  - セマンティックバージョンニングを採用
