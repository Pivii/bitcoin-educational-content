---
name: Robosats

description: Robosatsの使い方
---

![cover](assets/cover.webp)

RoboSats (https://learn.robosats.com/) は、ビットコインを法定通貨とプライベートに交換する簡単な方法です。ピアツーピア（P2P）取引を簡素化し、ライトニングホールドインボイスを使用して、保管と信頼の要件を最小限に抑えます。

![video](https://youtu.be/XW_wzRz_BDI)

## 使い方ガイド

> このガイドはBitocin Q&A ( https://bitcoiner.guide/robosats/) から引用しています。彼に全てのクレジットがありますので、そちらで彼をサポートしてください (https://bitcoiner.guide/contribute)；Bitcoin Q&Aは、ビットコインのメンターでもあります。メンタリングについては彼に連絡してください！

![image](assets/0.webp)

RoboSats - シンプルでプライベートなライトニングベースのP2P取引

## スタートする前に

### 知っておくべきこと

| 用語       | 説明                                                                                                                                                                                     |
| ------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Robot        | ロボット：自動生成されるプライベートな取引サポートボット。同じロボットを複数回使用しないでください。プライバシーを低下させる可能性があります。                                                             |
| Token        | トークン：ユニークなロボットを生成するために使用されるランダムな文字列。                                                                                                                              |
| Maker        | メーカー：ビットコインの購入または販売のオファーを作成するユーザー。                                                                                                                                            |
| Taker        | テイカー：ビットコインの購入または販売のオファーを受けるユーザー。                                                                                                                        |
| Bond         | ボンド（保証金）：取引の公正な完了を約束するために両方のピアによってロックされるビットコインの量。ボンドは通常、取引総額の3％で、Hodlインボイスによって提供されます。 |
| Trade Escrow | トレードエスクロー：Hodlインボイスを使用して、売り手が取引額のビットコインを保持する方法。                                                                                              |
| Fees         | フィー：RoboSatsは取引額の0.2％を手数料として課金し、メーカーとテイカーの間で分割されます。テイカーは0.175％を支払い、メーカーは0.025％を支払います。                                                       |

## 事前に準備すべきもの

### ライトニングウォレット

RoboSatsはライトニングベースですから、ボンド資金の提供や、購入者として購入したsats（サトシ）を受け取るためにライトニングウォレットが必要です。RoboSatsを機能させるために使用されている技術により、すべてのウォレットが互換性を持っているわけではありません。ウォレット選びには注意してください。

ノード（node）運営者の場合、「Zeus」が間違いなく最良の選択です。自分のノードを持っていない場合は、シンプルなセットアップとライトニングへのアクセスを提供するクロスプラットフォーム・モバイルウォレット「Phoenix」を強くおすすめします。この使い方ガイドでは、Phoenixを使用して説明しています。

### 少しのビットコイン

取引が行われる前に、買い手と売り手はボンドを資金提供する必要があります。これは通常、非常に小さな額（取引額の約3％）ですが、それでも必須条件です。

RoboSatsを使用して最初のsatsを購入しますか？スタートするために必要なわずかな額を貸してくれる友人を探してみてはいかがでしょうか！一人でやっている場合は、スタートするためのKYCなしのsatsを入手するための他の素晴らしいオプションを活用してください。

### RoboSatsへのアクセス

当然ながら、RoboSatsにアクセスする必要があります！これを行う主な方法は4つです：

1. Torブラウザ経由（推奨！）
2. 通常のウェブブラウザ経由（推奨されません！）
3. Android APK経由
4. 自分のクライアント

Torブラウザに慣れていない場合は、[こちら](https://www.torproject.org/download/) で詳細を学び、ダウンロードしてください。
iOSユーザーが自分の電話からTor経由でRoboSatsにアクセスするための簡単な注意点があります。「Onion Browser」はTorブラウザーではありません。代わりにOrbot + SafariやOrbot + DuckDuckGoを使用してください。

## ビットコインの購入

以下の手順は、2023年5月にバージョン0.5.0を使用してTorブラウザー経由でアクセスしています。Android APK経由でRoboSatsにアクセスするユーザーにとっても、手順は同じです。

執筆時点でRoboSatsは積極的に開発されているため、インターフェースは将来少し変更されている可能性があります。ただし、取引を完了するために必要な基本的な手順が、大きく変わることはないはずです。

> RoboSatsを初めて読み込むと、このランディングページが表示されます。まずは「Start」をクリックしてください。

![image](assets/2.webp)

トークンを生成したら、暗号化されたメモアプリやパスワードマネージャーのような安全な場所に保管してください。このトークンは、取引の途中でブラウザーやアプリが閉じた場合に、一時的なRobot IDを回復するために使用します。

![image](assets/3.webp)

新しいRobot（取引サポートボット）が表示されたら、「Continue」をクリックしてください。

![image](assets/4.webp)

オファーを閲覧するために「Offers」をクリックします。ページの上部で好みに合わせてフィルタリングできます。ボンドのパーセンテージと平均為替レートに対するプレミア価格に注意してください。

- 「Buy」を選択
- and useで「通貨」を選択
- pay withで「支払い方法」を選択

![image](assets/5.webp)

> 取引したいオファーをクリックします。売り手から購入したい金額（選択した法定通貨で）を入力し、最終的に詳細を確認して「Take Order」をクリックしてください。

売り手がオンラインでない場合（プロフィール画像の赤い点で示されます）、これは取引に通常よりも時間がかかる可能性がある旨の警告です。続行して売り手が時間内に進行しない場合、無駄になった時間に対して彼らのボンド額の50％が補償されます。

![image](assets/6.webp)

次に、画面上のインボイスを支払って取引ボンドをロックする必要があります。これはあなたのウォレットで凍結される保留インボイスです。取引の片方を完了できなかった場合にのみ請求されます。

![image](assets/7.webp)

ライトニングウォレットでQRコードをスキャンし、インボイスを支払ってください。

![image](assets/8.webp)

次に、ライトニングウォレットで表示された金額のインボイスを生成し、提供されたスペースに貼り付けてください。

![image](assets/9.webp)

売り手が取引金額をロックするのを待ちます。これが行われると、RoboSatsは自動的に次のステップに移動し、チャットウィンドウが開きます。「Hi」と挨拶し、売り手に彼らの法定通貨の支払い情報を尋ねてください。提供されたら、選択した方法で支払いを行い、RoboSatsでこれを確認してください。RoboSats内のすべてのチャットはPGPで暗号化されており、あなたと取引相手のみがメッセージを読むことができます。

![image](assets/10.webp)

売り手が支払いの受領を確認すると、RoboSatsは自動的に以前に提供されたインボイスを使用して支払いを送金します。

![image](assets/11.webp)

インボイスが支払われると、取引は完了し、あなたのボンドは解除されます。その後、取引の要約が表示されます。

![image](assets/12.webp)

ライトニングウォレットでsatsが着金したことを確認してください。

![image](assets/13.webp)

## 追加機能

ビットコインの購入と販売以外にも、RoboSatsには知っておくべきいくつかの機能があります。
Robot Garage：複数の取引を同時に行いたいが、同じRobosats（取引サポートボット）を共有したくありませんか？問題ありません！「Robot tab」をクリックし、追加のボットを生成して、次の注文を作成または受け取ってください。

![image](assets/14.webp)

### オファーの作成

他人のオファーを受けるだけでなく、自分のオファーを作成して、別のユーザーがあなたに来てくれるのを待つこともできます。

- 「Create」ページを開きます。
- ビットコインの Buy（購入）/ Sell（売却）のどのちらかを指定します。
- 購入 / 売却したい金額と通貨を入力します。
- 使用可能な支払い方法を入力します。
- 受け入れ可能な「市場価格に対するプレミア価格」（%）を入力します。現在の市場価格に対して割引で入札する場合、この数値はマイナスになることがあります。
- 「Create Order」をクリックします。
- メーカーボンドをロックするためにライトニングインボイスを支払います。
- 注文が有効になりました。誰かがそれを受け入れるのをリラックスしてお待ちください。

![image](assets/15.webp)

### オンチェーン支払い

RoboSatsはライトニングに焦点を当てていますが、購入者は自分のsats（ビットコイン）をオンチェーンアドレスに受け取ることもできます。購入者は、自分のボンドをロックアップした後にこのオプションを選択できます。オンチェーンを選択した後、購入者は手数料の概要を確認します。このサービスの追加手数料には以下が含まれます：

- RoboSatsによって発生するスワップ手数料 - この手数料は流動的で、ビットコインネットワークの混雑具合に応じて変動します。
- 支払いトランザクションのためのマイニング手数料 - これは購入者によって設定可能です。

![image](assets/16.webp)

### P2Pスワップ

RoboSatsでは、ユーザーは自分のライトニングウォレットからsatsをスワップしたり、そのウォレットにsatsをスワップしたりすることができます。オファーページの上部にある「swap」ボタンをクリックして、現在のスワップオファーを表示します。

「Swap In」オファーの購入者は、オンチェーンのビットコインをピアに送り、宣言された手数料および/またはプレミア価格を差し引いた後、自分のライトニングウォレットにsatsを受け取ります。「Swap Out」オファーの購入者は、ライトニング経由でsatsを送り、任意の手数料および/またはプレミア価格を差し引いた後、オンチェーンアドレスにビットコインを受け取ります。「Samourai」または「Sparrow Wallet」のユーザーは、スワップを完了するためにStowaway機能を利用することもできます。

RoboSatsのスワップオファーには、RBTC、LBTC、WBTCなど、ビットコインにペッグされた代替品も含まれることがあります。これらのトークンを扱う際に細心の注意が必要です。なぜなら、それぞれに多様なトレードオフ（代償）が伴うからです。ペッグされたビットコインはビットコインではありません！

![image](assets/17.webp)

### 自分のRoboSatsクライアントを実行する

Umbrel、Citadel、Start9のノード（node）運営者は、自分のノードに直接自分のRoboSatsクライアントをインストールできます。そうすることの利点は以下の通りです：

- 驚くほど速いロード時間。
- より安全：実行するRoboSatsクライアントアプリを自分で管理できます。
- 任意のブラウザー/デバイスから安全にRoboSatsにアクセスできます。ローカルネットワーク上にいる場合やVPNを使用している場合はTORを使用する必要はありません：匿名化に必要なtorificationはノードバックエンドが処理します。
- 接続するP2Pマーケットコーディネーターを管理できます（デフォルトはrobosats6tkf3eva7x2voqso3a5wcorsnw34jveyxfqi2fu7oyheasid.onion）

![image](assets/18.webp)

## FAQ

### 騙される可能性はありますか？

購入者として、取引の一環として必要な法定通貨を送金したが、売り手があなたにsatsを送金しない場合、紛争（異議申し立て）を行うことができます。この紛争プロセス中に、法定通貨を送金したことをRoboSatsの仲裁人に証明できれば、売り手のエスクロー資金とその取引ボンドがあなたに送金されます。取引をどのようにキャンセルしますか？

取引ボンドを投稿した後、取引メニュー内の「Collaborative Cancel」ボタンをクリックすることで取引をキャンセルできます。取引相手がキャンセルに同意していれば、手数料はかかりません。しかし、取引相手が取引を完了したいと思っていても、それでもキャンセルを進める場合、取引ボンドを失うことになります。

### RoboSatsは「X」支払い方法に対応していますか？

RoboSatsでは支払い方法に制限はありません。希望の方法でオファーが見つからない場合は、それを使用して自分のオファーを作成してください！

![image](assets/19.webp)

### RoboSatsを使用するとき、RoboSatsは私について何を知ることができますか？

TorまたはAndroidアプリを介してRoboSatsを使用する限り、何もありません！こちらで詳細をご覧ください。

- Torはネットワークのプライバシーを保護します。
- PGP暗号化は取引チャットをプライベートに保ちます。
- アカウントがないことは、取引ごとに1つの取引サポートボットを意味します。これは、RoboSatsが複数の取引を単一のボットに関連付けることができないことを意味します。

ただし、注意点がいくつかあります！ライトニングは送信者としてはかなりプライベートですが、受信者としてはそうではありません。自分のライトニングノードに受け取る場合、ノードIDがインボイスで共有されます。このノードIDは、それを知っている人にとって、オンチェーン活動をリンクしようとする出発点を与えることになります。これは、ユーザーがオンチェーンでの支払いを受け取ることを選択した場合にも当てはまります。

このリスクを軽減するために、ユーザーはライトニング用のプロキシウォレットやオンチェーン用の「Coinjoin」などのソリューションを使用することもできます。

### フェデレーション

現在、RoboSats開発チームによって運営されている単一のRoboSatsコーディネーターがあります。ビットコインでは、あらゆる形態の中央集権化は、特定のサービスを好ましく思わない政府や規制当局にとってより簡単な標的となります。

RoboSatsがオープンソースプロジェクトであるため、誰でもコードを取得して自分のコーディネーターの運営を開始することができます。これはある程度、リスクを単一の標的から分散させるものの、すでに希薄な流動性市場をさらに分断します。

RoboSatsチームはこれを認識しており、フェデレーテッドモデルの作業を開始しました。エンドユーザーとしては、上記の取引フローはあまり変わらないはずですが、新たに現れる異なるコーディネーターを追加または削除するための追加ビューや画面が存在します。

使い方ガイドは以上です https://bitcoiner.guide/robosats/
