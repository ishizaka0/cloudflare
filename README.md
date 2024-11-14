以下に日本語訳を記載します：

---

# Cloudflare  
Cloudflare公式のWordPressプラグイン  

| No. | 更新対象 | 名前 | ステータス | 更新 | バージョン | 最新バージョン | WordPressテスト済み | PHPバージョン | プラグインホームページ | WordPress公式URL | 備考 |  
| --- | -------- | ---- | ---------- | ---- | ---------- | -------------- | ------------------- | ------------- | --------------------- | --------------- | ---- |  
| 4   | ー        | Cloudflare | アクティブ | なし | 4.12.8    | 4.12.8         | 6.2.6              | 7.2          | [Cloudflare](https://blog.cloudflare.com/new-wordpress-plugin/) | [リンク](https://wordpress.org/plugins/cloudflare/) | ー |  

# CloudflareのWordPressプラグイン  

![ビルドステータス](https://github.com/cloudflare/Cloudflare-WordPress/workflows/PHP%20Composer/badge.svg)  

CloudflareのWordPressプラグインは、CloudflareのすべてのメリットをWordPressダッシュボードに取り込み、WordPress専用に最適化されたデフォルト設定をワンクリックで適用することができます。  

このプラグインをWordPressサイトで有効化すると、ページ読み込み速度が2倍になるパフォーマンス向上、DDoS保護、WordPress専用ルールセットを備えたウェブアプリケーションファイアウォール（WAF）、無料SSL、SEO向上といった利点が得られます。  

## 目次  

[概要](#description)  
[インストール](#installation)  
[サポート](#support)  
[機能](#features)  
[FAQ](#faq)  
[コントリビューション](#contributions)  
[変更履歴](#changelog)  

## 概要  

CloudflareのWordPressプラグインは、WordPress専用に開発された設定をワンクリックで適用できる機能を提供します。Cloudflareの無料プラグインを利用することで、ページ読み込み速度を向上させ、SEOを改善し、DDoS攻撃やWordPress特有の脆弱性からウェブサイトを保護します。  

## 機能  

### ワンクリックでWordPress向け最適化設定を適用  

WordPressに最適化された設定をワンクリックで適用することで、Cloudflareのパフォーマンスとセキュリティを簡単にセットアップできます。適用される推奨設定については、[こちら](https://support.cloudflare.com/hc/en-us/articles/227342487)をご覧ください。  

### ウェブアプリケーションファイアウォール（WAF）ルールセット  

CloudflareのWAFは、すべての有料プランで利用可能で、WordPressの脅威や脆弱性を軽減するために専用ルールセットを備えています。CloudflareのWAFにより、常に最新の脅威からもウェブサイトを保護できます。  

### サイト更新時のキャッシュ自動パージ  

WordPressの外観を変更する際、CloudflareのプラグインはCloudflareキャッシュを自動で更新します。この機能により、最新のコンテンツを常に訪問者に表示できます。  

### ページ/投稿/カスタム投稿タイプ編集時の個別URLキャッシュ自動パージ  

ページや投稿、カスタム投稿タイプを更新すると、CloudflareのWordPressプラグインが自動的にキャッシュを更新します。  

### その他の機能  

- Universal SSLが有効な場合のリダイレクトループを防ぐためのヘッダーリライト。  
- Cloudflare.comダッシュボードにアクセスせずに、プラグイン内からCloudflareの設定を変更可能（キャッシュパージ、セキュリティレベル、Always Online™、画像最適化など）。  
- 訪問者数、節約された帯域幅、ブロックされた脅威などのアナリティクスを表示。  
- HTTP/2およびサーバープッシュのサポート。  

## インストール  

1. CloudflareプラグインをWordPress管理画面からインストールします。以下のURLから「ダウンロード」をクリックするか、GitHubリポジトリからプラグインをダウンロードしてください：<https://wordpress.org/plugins/cloudflare/>  
    - GitHubからダウンロードした場合、「プラグイン」→「新規追加」→「プラグインのアップロード」でCloudflare-WordPress-master.zipファイルをアップロードします。  
2. プラグインをインストール後、WordPressプラグイン管理画面で有効化します。  
3. 旧プラグインからアップグレードする場合、以前に入力したAPIキーがある場合、自動的にログインされます。  
4. 初めてプラグインをインストールする場合、有効化後に設定画面でCloudflareのユーザー名とAPIキーを入力してください。APIキーの取得方法は[こちら](https://support.cloudflare.com/)をご覧ください。アカウントをお持ちでない場合、作成オプションが表示されます。  
5. プラグインにログイン後、「デフォルト設定を適用」ボタンをクリックしてください。この操作により、WordPressに最適化された特定のCloudflare設定が有効になります。設定の詳細は[こちら](https://support.cloudflare.com/hc/en-us/articles/227342487)をご覧ください。  
6. これで設定完了です！Cloudflareネットワーク上でウェブサイトが最適化されました。ウェブサイトの読み込み速度向上、帯域幅の節約、ハッカーやスパマー、ボットからの保護が期待できます。  

## FAQ  

### プラグインを使用するにはCloudflareアカウントが必要ですか？  

はい。プラグインをインストールおよび有効化する際、初回ユーザーはメールアドレス（Cloudflareアカウント作成用）とAPIキーを入力する必要があります。この情報はプラグインのすべての機能を利用するために必要です。  

### 「デフォルト設定を適用」をクリックすると、どの設定が適用されますか？  

適用される推奨設定の詳細は[こちら](https://support.cloudflare.com/hc/en-us/articles/227342487)をご覧ください。  

### Varnishが有効でもプラグインは動作しますか？  

はい。Varnishを有効にしている場合でも、Cloudflareはさらにサイトの高速化をサポートします。  

## サポート  

### ナレッジベースをご覧ください  

サポートチケットを送信する前に、ナレッジベースをご確認ください：<https://support.cloudflare.com/hc/en-us/sections/200820268-Content-Management-System-CMS->  

### サポートチケットを送信  

CloudflareのWordPressプラグインに関するお問い合わせは、Cloudflareアカウントにログインし、サポートチケットを送信してください。スクリーンショットや詳細を添付してください：<https://support.cloudflare.com/hc/en-us/requests/new>  

## コントリビューション  

このリポジトリへのコミュニティ貢献を歓迎します。[CONTRIBUTING.md](CONTRIBUTING.md)を参照して開始してください。[Issues](https://github.com/cloudflare/Cloudflare-WordPress/issues)ページで解決する課題を見つけることができます。  

## 変更履歴  

変更履歴は[こちら](https://wordpress.org/plugins/cloudflare/changelog/)をご覧ください。  
