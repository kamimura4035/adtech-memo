# adtech-memo

## 広告全体の概要
* 広告業界の登場人物はざっくり２人だけ（一番コアの部分はここ）
  * 媒体
  * 広告主
* 媒体と広告主について
  * 広告主
    * お金が欲しい
      * 「自分が買って！っていろんな人に直接いっても限界があるなぁ」
      * 「もっとたくさんの人に知ってもらって、たくさんの人に買ってもらいたいな...」
      * 「多くの人がみそうなところに「この商品買って」って書いておけばいいんじゃないか？」
      * 「多くの人がみそうなところ（つまりメディア）に広告を出すか！」
  * 媒体
    * お金が欲しい
      * 「広告主からもっといっぱいお金が欲しいよ〜」
      * 「もっと人をあつめて、広告効果が高いメディアになるぞ」
      * → 集客人数、視聴率、PVなどの指標をあげて収益をあげていく
* お金の流れは
  * 広告主 から 媒体 へ
  * 広告主が、媒体に対してお金を払って広告を掲載させてもらう
* 媒体の種類
  * 人が集まればなんだって媒体になる！
    * マスコミ四媒体
      * 新聞、雑誌、ラジオ、テレビ
    * 他の媒体（一部）
      * 屋外
      * 交通
      * DM
      * インターネット ← これがweb広告！
    * 有名人
      * 芸能人
      * インフルエンサーなど...
  
## web広告について
* 登場人物はやっぱり2人
  * 広告主
  * 媒体（webサイト、アプリ）→ もっと抽象化して「枠（インベントリ）」と呼ぶことが多い
    * google
    * twitter
    * facebook
* web広告のざっくりした流れ
  * 媒体は枠を売り、広告主は買った枠に広告を出す
* 代理店はなにしてるの？
  * 「代理」をしてるだけ
  * 媒体に変わって、広告枠を売る → 実際枠を売っているのはアドネットワークやSSP
  * 広告主に変わって、広告枠を買って広告を出す → 実際枠を買っているのはアドネットワーク、DSP
* じゃあ本当は代理店は何してるの？
  * 広告主に対して「効果が望めそうな広告プラン」を提案＆受注する
    * プランはいろいろある
      * 化粧品をうるならこのプラン
      * 不動産ならこのプラン
      * など、扱う商品によって適切なプランがある
  * 受注した内容を広告配信サービスに配信依頼（アドネットワーク、DSPなど）
    * 依頼時に必要項目
      * 予算
      * クリエイティブ（代理店内で発注したりする）
      * 期間
      * セグメント
      * ... etc
  * 配信された広告の結果（click, imps, cvなどいろいろ）をreportとして出す
    * それを広告主と共有する


## 広告業界の歴史
* 大前提
  * 一般的な需要と供給の関係
    * 供給 < 需要 --- 消費者は競ってその商品を手に入れようとするため、市場価格は上がる
    * 供給 > 需要 --- 売れ残って市場価格は下がる
  * 広告業界に置ける需要と供給とは
    * 供給は枠
    * 需要は広告
  * 広告業界に置ける需要と供給の関係
    * 供給 < 需要 --- 主は競ってその枠を手に入れようとするため、市場価値が上がる
      * 主がかわいそう
    * 供給 > 需要 --- 枠が売れ残って市場価格は下がる
      * 媒体がかわいそう
  * つまり
    * 両者がかわいそうにならないように、業界は発展してきた

* 純広告
  * 概要（たとえ）
    * 古き良きご近所さんづきあい
  * 概要
    * 広告主が、媒体の枠を「直接」買う
  * 例
    * Yahoo TOPの広告など
  * 広告の管理方法
    * 媒体上
      * 概要
        * サイトに直接埋め込む
      * 課題
        * 広告の入れ替えが困難
        * サイト改修が必要。デザインが崩れるかも
        * 複数の広告主の広告を同じ期間に出すことができない
    * アドサーバ
      * 概要
        * サイト上で管理していた広告を、別のサーバで管理するようにした
      * 詳細
        * 媒体サイトは枠にタグを埋め込み、そのタグからアドサーバにリクエストを送る
        * アドサーバはそのリクエストに対して広告を配信する
        * 広告を配信するだけでなく、インプレッション数やクリック数、コンバージョン数などの計測機能もある
      * 例
        * Google Ad Manager(旧 DoubleClick for Publisher)
          * 無料
  * 課題
    * 媒体側
      * 営業が大変
      * 枠が余ることもある
    * 主側
      * 営業が大変
      * 枠が少ない時、広告が表示できない

* アドネットワーク
  * 概要（たとえ）
    * 市場（いちば）
  * 概要
    * 媒体の Webサイトやアプリを多数集めたネットワクーク
      * 大量の広告枠をまとめたもの
    * メリット
      * 主側
        * 営業不要
        * 枠がたくさんあるので広告が表示される回数が増える
      * 媒体側
        * 営業不要
        * たくさんの広告主と繋がれるので枠があまりにくい
    * 例
      * Google
        * GDN(Google Display Network)
          * 媒体はAdSenseで枠を登録
          * 主はAdwordsで広告を入稿
      * Yahoo
        * YDN(Yahoo Display Network)
      * ファンコミュニケーション
        * Nend
      * アイモバイル
        * アイモバイル
    * 課題
      * それでも広告在庫と広告出稿の需要と供給バランスが崩れることがある
        * アドネットワークによって特色があるから

* RTB/DSP/SSP
  * 概要（たとえ）
    * 世界中の市場が一箇所にあつまった、超巨大市場
    * ものすごいスピードで「せり」が行われる
  * 概要
    * アドネットワークは主と枠、両方管理していた
    * RTBは各々に分けている
    * なので、登場人物は2人
    * その二人をつなぐプロトコルがRTB
  * 登場人物
    * SSP
      * 枠の管理
      * 媒体の収益をあげることに尽力
    * DSP
      * 主の管理
      * 効率よく広告を配信することに尽力
  * 流れ
    * 1. SSPのタグが導入されている広告枠があるサイト/アプリへ訪問
    * 2. SSPのタグからSSPサーバへ、どの広告枠を誰が訪問したかが送信される(Ad Request)
      * どの枠か
        * webサイトの場合はドメイン、アプリの場合はアプリID
      * 誰が訪問したか
        * webサイトの場合はクッキー、アプリの場合はIDFA
    * 3. 接続先のDSPに対してRTBプロトコルでリクエストを送る(Bid Request)
      * Bid Requestに何が含まれえるかはiAB党組織がOpenRTBを定義している
      * それにしたがってSSPを作る
    * 4. DSPはBidRequestをうけ、誰がどこにきたのかという情報を元に、対象の枠をいくらで購入するか返す(Bid Response）
      * 買わない、という選択肢もある。0円で入札
    * 5. SSPは入札のあったDSPの中から、最も高い金額で入札されたDSPの配信タグを広告枠に設置する
      * win noticce, lose notice
  * 早い
    * オークションは100ms以内に行われる必要がある
  * 例
    * DSP
      * Criteo
      * RocketFuel
      * Blade(MicroAd)
      * FreakOut DSP(FreakOut)
      * ScaleOut DSP(Supership)
    * SSP
      * Rubicon Project
      * PubMatic
      * Fluct(VOYAGE GROUP)
      * Geniee SSP(Geniee)
      * COMPASS(MicroAd)
    * SSPに似たやつ
      * Google Ad Manager(Google)
        * GDNをRTB経由で買い付けられる
        * ものすごい量の枠
      * Bid Switch(IPONWEB)
        * SSPを束ねてる
        * これに接続すると一気に多くのSSPと接続できる
  * ベンチャー企業ののし上がり
    * 前述の二つのSSPに接続するだけで一気に月間何百億ものインベントリが手に入る
    * ものすごい在庫を抱えた状態。大企業とも対等の存在になれる


