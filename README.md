# *RUNTEQ_Portfolio*
## **サービス概要**
動画にメモできるサービスになります。<br>
動画に対して時間軸上でメモを追加や、
視聴中に重要な箇所やコメントを記録し、<br>
後で参照したり共有したりできるといった内容になります。
<br>

## **このサービスへの思い・作りたい理由**
TV業界の照明マンは、CUEシート作成に苦労します。<br>
CUEシートは、次の音のタイミングで照明を調整するための進行表のようなものです。<br>
私も照明マンだった頃は苦労しました。<br>
YOUTUBEなどからアイデアを得る際、
動画に直感的にメモを書き込むことができれば、作業効率が飛躍的に向上すると考えました。<br>
そこで、現役の照明マンの助けになるべく、このサービスを作成することにしました。
<br>


## **Why You?**
私は現在も定期的に照明マンとして活動しており、この職業の肉体的な要求と厳しさを身をもって経験しています。長時間にわたる作業が求められる現場の環境は、肉体的にも精神的にも大きな負担となります。そんな照明マンの労働を少しでも軽減し支援することが、このサービスを生み出す動機となりました。<br>
また私自身が音楽が好きで、このサービスのメモ共有を通じて最新の音楽トレンドや人気曲を発見できるかと思います。
<br>


## **ユーザー層について**
動画制作や編集に関わる人々、特に照明マンや動画編集者を主な対象としています。最近では動画編集が個人レベルでも広く行われるようになり、この分野における需要は高いと考えます。この背景から、このユーザー層が特に関心を持つと考えられます。<br>
また、音楽好きな人々も対象としています。メモ共有を通じて新しい音楽に触れる機会を得られるため、この機能は魅力的だと考えます。
<br>

## **サービスの利用イメージ**
動画再生中に時間軸上にメモを追加し、重要なポイントやコメントを記録できる機能を提供します。照明マンは特定のシーンにおける照明効果のアイディアをメモとして残し、動画編集者は編集ポイントや修正が必要な箇所をコメントで記録できます。これにより、後での修正や調整が容易になります。
音楽好きなユーザーは、このサービスを通じて、新しい音楽やトレンドをメモ共有を介して発見する。
<br>


## **ユーザーの獲得について**
Xでの宣伝と前職の方と繋がりがあるので、
お声がけしようと思っています。
<br>

## **サービスの差別化ポイント・推しポイント**
#### ***差別化ポイント：***<br>
直感的な操作性に重点を置いています。照明マンや動画編集者など、プロフェッショナル層が主なユーザーであるため、作業効率の向上は最優先事項だと考えています。複雑な操作を必要とせず、誰もがすぐに使いこなせる直感的なインターフェースを実現することで、効率的な作業が可能になると考えます。<br>

#### ***推しポイント:***<br>
作業効率の向上: 照明マンや動画編集者のプロセスをスムーズにすることで、作業時間を大幅に削減します。<br>
音楽愛好家へのアプローチ: 新しい音楽やトレンドに簡単にアクセスできる点は、音楽好きなユーザーには魅力的だと考えます。
<br>

## **機能候補**
### *MVPリリース時*
#### ***ユーザーアカウント管理:***
ユーザー登録・ログイン機能。
ユーザープロフィールの設定や編集機能。
<br>

#### ***youtubeのデータ取得:***
Youtube Data APIでの取得。
現状、youtubeからデータの取得の実装は出来ています。
<br>

#### ***動画・メモ検索機能:***
動画タイトル・メモの内容で検索欄を分ける。

#### ***動画再生とメモ機能:***
動画を再生しながら、時間軸上にメモを追加する機能。
視聴中に重要な箇所やコメントを記録し、後で参照できる機能。
メモは公開と非表示を選べるようにしたい。
<br>

#### ***メモの管理機能:***
ユーザーが作成したメモの一覧表示や編集、削除ができる機能。
<br>

#### ***投稿したメモをXへのシェア機能***
おすすめの音楽を共有できる。
<br>

#### ***Google OAuthの使用:***
登録の手間を省きたい。
<br>

### *本リリース時*
#### ***動画アップロード機能:***
自分で用意した動画のアップロード機能
<br>

#### ***Youtubeと投稿動画の切り替え:***
操作性の向上

<br>

#### ***メモへのいいね機能:***

<br>


## **機能追加案**
* 動画アクセスランキング・メモ数ランキングで表示できる機能。
* Youtube・投稿した動画へのいいね機能
* Youtubeをデータ取得の際にオートコンプリート機能
* Lineログイン
<br>


## **機能の実装方針予定**
#### ***ユーザーアカウント管理:***
Gem:sorcery
<br>

#### ***Youtubeのデータ取得:***
API: Youtube Data API<br>
Youtube APIを使用
Youtube Data APIを利用して、動画の情報やメタデータを取得する。
<br>

#### ***動画再生:***
ライブラリ: react-player (React)<br>
Webプレーヤーを使用して動画を再生する。
動画のURLを取得し、Webプレーヤーを埋め込んで表示する。
<br>

#### ***メモ機能:***
ライブラリ: Reactを使用して実装<br>
Reactを使用して、動画の再生時間と連動してメモを表示・追加する。
<br>

#### ***動画アップロード機能:***
Gem: CarrierWave (Rails)<br>
ユーザーが自分で用意した動画をアップロードできる機能を提供する。
<br>

#### ***Google OAuthの使用:***
Gem: omniauth-google-oauth2 (Rails)<br>
ユーザー登録・ログイン時にGoogle OAuthを使用して、手間を省いた認証システムを提供する。
<br>


## **技術スタック**
#### ***フロントエンド:***
* React
* Next.js
* TypeScript
* Tailwind

#### ***バックエンド:***
* Rails(7系)
* ruby（3系）

#### ***データベース***
* PostgreSQL

#### ***環境構築***
* Docker

#### ***CI/CD***
* Github Actions

#### ***WebAPI:***
* Youtube data API
  
#### ***インフラ:***
* フロントエンド：Vercel
* バックエンド：Heroku
* データベース：S3

現状実務でTypeScriptを触っているのですが、
完全に理解できているわけではないので、
Railsで一度作りきってから、順次移行していきたいと思います。
