<!-- (generate pdf file) $ yarn build:pdf -->
# Resume

## Profile

|key|value|
|----|----|
|Name|嶋田 怜央成|
|Birth(Age)|1994/05/30(27)|
|Sex|男性|
|Location|神奈川県横浜市|
|Education|神奈川大学人間科学部卒|
|Mail|shimada.reona@gmail.com|
|Twitter|[@reona_5](https://twitter.com/reona_5)|

## Hobby

- 筋トレ
- サウナ
- ハンドボール
- フェス
- カラオケ
- 料理
- お酒
- シーシャ

## Output

- Blog
https://reona.dev

TypeScript, Next.js でブログ環境を構築

## Skills

- 業務経験あり
  - MySQL
  - PostgreSQL
  - Ruby
    - Ruby on Rails
  - Swift
    - SwiftUI
    - Combine
  - JavaScript
    - Vue.js

- 趣味
  - TypeScript
    - React.js
      - Next.js

## Editor

- NeoVim

## Certification

- 基本情報技術者試験 (2021/06)
- MR 認定試験 (2018/04)

## OSS Contributes

- [AaronLasseigne/active_interaction](https://github.com/AaronLasseigne/active_interaction)
  - [Replace string passed to :unless with proc #509](https://github.com/AaronLasseigne/active_interaction/pull/509)

## Career

### C向けサービスベンチャー (2019/08 - )

- 概要
  - プログラマとしてのキャリアをスタート。
  - 受託開発や他社案件の開発支援（客先常駐なし）、自社の新規サービス開発を行う。

#### プロジェクト

##### B 向け食材・調味料発注アプリ(2020/12 - )

- Ruby on Rails, Vue.js(Vuex) でのバックエンド・フロントエンド開発がメイン
  - View 層は半分以上を Rails(haml) が担っており、部分的に Vue がレンダリングされている（リプレイスも担当）
- RSpec
  - 書かれていないテストの追加（機能追加時はテストを追加）
  - Pending の解消(44 -> 0)
  - 警告の解消
- ActionMailer を用いた出荷遅延通知の追加
- 商品サムネイルのスワイプ
- クイック発注でのカートの状態保持(sessionStorage)
- 管理画面(RailsAdmin)
  - CSV Import/Export
  - レコード検索・絞り込み機能
  - 利用申請と得意先の連携解除機能
  - 利用申請削除機能（得意先関連レコードの削除）
- 消費税計算方法の修正(総額表示義務化への対応)
  - 合計(税別) = 8% 合計(税別) + 10% 合計(税別) => 税抜金額合計
  - 合計(税込) = 購入合計(税別) + 8% 消費税合計 + 10% 消費税合計 => 税込金額合計
- KARTE タグ導入によるユーザー解析
  - 閲覧(SPA含む)
  - カート（SPA含む）
  - 購入(カート・1タップ購入・クイック発注)
  - ユーザー
  - 商品詳細
  - お気に入り
    - 商品
    - メニュー
  - 検索
    - 商品・メニュー
    - クイック発注内商品
  - ログイン
- 既に使われていない不要な機能・gem の削除
- Rails バージョンアップ
  - 6.0.3.7 -> 6.1.4
  - 各gem のバージョンアップ
  - Webpacker 4.0.7 -> 5.4.0
- Ruby バージョンアップ
  - 2.6.5 -> 2.7.3

##### C 向け ファンコミュニティアプリ(2021/02 - 2021/04)

- Ruby on Rails (active interaction, active model serializers) による REST API サーバの実装
  - Omniauth を用いたSNSアカウント認証機能の実装
    - Twitter
    - Apple
  - ActiveStorage を用いたアイコンアップロード機能
  - 投稿機能
  - いいね機能
- rswag を用いて RSpec から OpenAPI のスキーマを自動生成

##### 医療脱毛クリニックの顧客管理システム開発(2020/08 - 2020/11)

- 契約関連書類の電子化（ペーパーレス）
  - Ruby on Rails (active model serializers) による REST API サーバの実装（OpenAPI, committee によるスキーマ駆動開発）
    - RSpec でのテストファーストな実装
    - parameter クラスの実装（ActiveModel::Attributes）
    - 契約書類を pdf ファイルとして動的に生成、電子サイン組み込み（wicked_pdf, wkhtmltopdf）
    - 契約書類の雛形となる view テンプレートの作成（erb）
    - ActiveStorage を用いてユーザーと各契約書類を紐付け、書類のサムネイル化
    - ActionMailer を用いた同意書類通知
    - rqrcode を用いた問診票 URL の QR コード生成
    - openapi-generator を用いた API 定義からの API Client 生成
  - Vue.js, TypeScript を用いたフロントエンド開発

##### C 向けメンズ美容サービスの Web/iOS アプリ開発(2020/02 - 2020/07)

- Ruby on Rails (active interaction, active model serializers) による REST API サーバの実装
  - jwt, device を用いたユーザー認証機能の実装
  - faraday, faraday middleware を用いた SNS アカウントによるユーザー認証機能
  - Twitter API
  - Facebook Graph API
  - Google People API
  - Ransack による検索機能の実装
- Swagger によるAPI I/F仕様書の導入提案及び Docker 上での SwaggerUI の環境構築
- MVVM を採用し、Swift (SwiftUI, Combine) によるゼロベースでの UI, MVVM クライアント API 実装を担当
  - XCodeGen によるプロジェクト管理
  - bitrise による CI の導入
  - OAuthSwift を用いた SNS の認可処理の実装
  - Twitter API
  - Facebook Graph API
  - Google Drive API
  - SwagGen 導入によるコード自動生成

##### C 向け通信系サービスの開発支援(2019/10 - 2020/01)

- リリース前のコア機能実装を担当
- Ruby on Rails (active model serializers) による REST API サーバの実装
  - 個人情報入力や決済処理、SIM の付与等を含む契約フローをメインで担当
- フロントエンドは React/Redux
- Swagger による API ドキュメントの管理
- Stripe を用いたサブスクリプション決済機能の実装
- RSpec でのテストファーストな実装
- SendGrid を用いたメール配信機能の実装
- Active Jobs, syoryuken, Amazon SQS を用いたバッチ処理の実装
- Action Mailer の実装
- Rake タスクの実装

##### B 向け業務代行サービスの受託開発(2019/08 - 2019/10)

- 既存機能拡張やバグ改修をメインで担当
- Ruby on Rails / Vue.js 利用した管理者画面の構築
- CanCanCan, Pundit によるユーザー権限の管理


### 某新薬メーカー (2017/04 - 2019/07)

- 概要
  - 医薬情報担当者（MR）として千葉県市原市の個人開業医や小規模病院を対象とするルート営業を担当（通算2年1ヶ月）
  - 5ヶ月間の研修では基本的な社会人マナーをはじめ、薬学知識のインプット(MR 認定試験対策含む)、現場を想定した自社医薬品のプレゼンテーション・ディテール力を身に付けた。
  - 品目別前年同期比支店内トップの実績を獲得(支店MR約100名中1位)
  - 各医薬品卸において自社品目新規採用を表彰頂く。(全5支店中3支店)
  - 独学でプログラミングの勉強を始める。[MENTA](https://menta.work/)で技術的なサポートを受けつつポートフォリオを作成する。（2019/01 - 2019/05）
    - [Lesson](https://github.com/reona5/Lesson)（現在はクローズ）
