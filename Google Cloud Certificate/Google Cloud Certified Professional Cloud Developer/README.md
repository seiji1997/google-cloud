# Google Cloud Certified Professional Cloud Developer

Professional Cloud Developer試験対策マニュアル<br>
https://blog.g-gen.co.jp/entry/professional-cloud-developer

## **Professional Cloud Developer**

Professional Cloud Developers build scalable and highly available applications using Google-recommended practices and tools. They have experience with cloud-native applications, developer tools, managed services, and next-generation databases. Cloud Developers are also proficient with at least one general-propose programming language and are skilled at producing meaningful and logs to debug and trace code.

- Design highly scalable, available, reliable cloud-native applications
- Deploy applications
- Manage application performance monitoring
- Build and test applications
- Integrate Google Cloud services
## **Case study**

Some of the questions on the Professional Cloud Developer certification exam may refer you to a case study that describes a fictitious business and solution concept. This case is intended to provide additional context to help you choose your answer. We recommend that you review the case study that is used in the exam.

[https://services.google.com/fh/files/blogs/master_case_study_hiplocal.pdf](https://services.google.com/fh/files/blogs/master_case_study_hiplocal.pdf)


## Google Cloud Professional Cloud Developer試験

クラウドネイティブなアプリケーション開発を行うための知識を問うGoogle Cloud 認定資格

GCP上で下記の実装能力と知識力が問われます。

- アプリケーションの高可用性
- スケーラビリティ
- セキュリティ
- マネージドサービスの活用
- サーバーレスの活用
- 運用性の高いアーキテクチャを設計する知見
- CI/CD や開発ツールに関する知識

## 学習方法

1. モダンな開発手法に関する知識を別途、学習する
2. Associate Cloud Engineer 試験 を学習し、取得することで Google Cloud の基本を理解
3. [試験ガイド](https://cloud.google.com/certification/guides/cloud-developer) を確認して試験範囲を理解する
4. 公式ドキュメントを中心に試験範囲を学習する
5. 当記事を読み、試験範囲の詳細を把握し、知らない知識を補填する

## モダンな開発手法について

<details><summary>CI/CD (継続的インテグレーション / 継続的デリバリ)</summary>

DX推進の具体的な取り組みの一つとしてApplication開発があります。また、DX Applicationの特徴の一つにアジャイル開発があります。それを実現するための手段として開発と運用を一体として考えるDevOpsが普及しました。そのためのツールとしてCI/CDが注目を集めています。
CI/CDとは、CI=Continuous Integration、CD=Continuous Delivery
です。特定の技術を示すものではなく、ソフトウェアの変更を常にテストして、自動で本番環境に適用できるような状態にしておく開発手法のことです。
**Continuous Integration**
開発者にとっては自動化のプロセスを指します。アプリケーション開発で言えば、バラバラに稼働している複数のエンジニアのソースコードを継続的に統合し、正常に動作することを確認するために検証する取り組みです。新たなソースコードの変更を定期的に、ビルドおよびテスト（問題がないかを調べるために、クラスや各種モジュールなどの構成する全ての要素に対して実施するテストを自動化：プログラムの不具合を早く見つけてすぐに修復可能）し、共通のリポジトリに統合します。CIを実施しない場合は全て手動で実施しないといけないことから有用性がわかります。
**Continuous Delivery**
ユーザーに継続的にアプリケーションを提供（本番環境にアプリケーションを載せ、顧客がいつでも新たなアプリケーションを利用可能にすること）します。検証済みコードのリポジトリへのリリースを自動化し、コード変更のマージから本番環境に対応するためのビルドのデリバリーまで、全ての段階でテストとコードリリースを自動化します。これにより、運用チームは本番環境にアプリケーションをすぐにデプロイできます。
**CI/CDの背景**
ビジネス環境は常に変化しているので、それに合わせてアプリケーションには変更、差し替え、新規作成、削除などの変化が求められることがあります。
ウォーターホール開発：従来の多くの企業ではウォーターホールモデルでアプリケーションを開発してきました。これは、要件定義、基本設計、詳細設計、テストといった開発工程を上から下へ一方的に流すものです。研修やスケジュール、計画、工数の見積り等がしやすいなどの利点があり、金融業界などの品質を重視する現場で採用されてきました。しかし、ウォーターホール型では要件を固めて工程を進めるため、途中での変更が難しいという欠点があります。ビジネス面やシステム面などの事情で仕様変更が発生した場合、大きな手戻りが発生してしまいます。
DXは「ビジネスを革新する何か」を模索する取り組みといっても過言ではないので、開発するアプリケーションの仕様が明確になっていないケースがあったり、開発を進めながら明らかにしていくことがあったりするため、要件を事前にもれなく定義することが難しくなっています。
     
</details>

<details><summary>DevOps / DevSecOps</summary>
    
    DevSecOpsが重要視されるようになった背景
    
    **1, DevSecOpsの登場した直接的な背景：**
    
    開発期間の短縮とシステムの品質向上は相反する目的ですが、実現するにはOSSやAPIなどの効率的な活用が求められます。ところが、開発期間の短縮と効率化、システムの品質を優先すると、セキュリティの脆弱性のために余力が無くなります。多くのセキュリティの問題は運用時に明らかになりますが、DevOpsのライフサイクルで開発時にフィードバックする場合、開発スピードを犠牲にしなければなりません。したがって、予めセキュリティを考慮した運用のライフサイクルが必要になります。
    
    **2, クラウドによりセキュリティ分野の技術革新が進展したこと：**
    
    企業が展開するビジネスや業務管理などのシステムがクラウド化し、セキュリティの重要度が高まったこと、クラウドによるセキュリティ管理と自動化が進んだこと
    
    システム開発や運用に加えて、以下のようなセキュリティー要件が求められる：
    
    - サステイナブルなビジネスを実現する堅牢なセキュリティ
    - クラウドや仮想化により高度なセキュリティを迅速に実装すること
    - 自動化された脅威の検出、不正の監視、レポーティングで管理負担とコスト軽減
    
    以下の技術革新によって実現
    
    - クラウドに最適化されたファイアウォールや監視ツール
    - 膨大なログを収集と蓄積する仮想化されたストレージ、人工知能による解析
    - 監視や不正アクセス遮断、ポリシーの実行などの自動化
    - 詳細なレポーティング、管理コンソールによる可視化
    
    **Point**
    
    - ソースコードとアプリケーションのセキュリティを確保すること
        
        ソースコードに対して脆弱性診断、静的アプリケーションセキュリティテスト（SAST）、ソフトウェアコンポジション解析（SCA）を徹底する必要があります。
        
        アプリケーションに関しては、動的アプリケーションセキュリティテスト（DAST）、クロスサイトスクリプティング（XSS）など、あらゆるサイバー攻撃を想定してセキュリティに問題がないか確認します。
        
    - 開発及び運用チームの生産性を保つこと
        
        セキュリティの脅威などのログを自動検知したり、ルールやポリシーを設定するなど、なるべる組織体制を整えることが重要です。
        
    - CI/CD
        
        DevOpsの基本にセキュリティ対策を組み込みます。
        
    
    **DevOpsとDevSecOpsの違い**
    
    開発と運用を融合させたDevOpsにセキュリティ対策が入っているかどうかがDevOpsとDevSecOpsとの違いです。DevOpsではビジネス稼働までの時間短縮、品質の向上、コスト削減が主な利点でした、DevSecOpsはさらに経営面（経営面の価値とはBCP(Business Continuity Plan)）から価値が加わります。
    
</details>

<details><summary>テスト駆動開発</summary>>
    
    テスト駆動開発とは、ソフトウェア開発手法の１つで、プログラム本体より先にテストコードを書き、そのテストに通るように本体のコードを記述していく方式です。
    
    test firstと呼ばれる原則に従って開発を進めていく手法で、まず、プログラムの機能や使用に基づいて、そのプログラムが通るべきテスト条件やテストコードを記述していきます。
    
    テストを作成したら、そのテストに合格する最低限のコードで構成されたプログラムを実装します。この段階では、本来の処理を行わず条件を満たす定数を記述したり、同じコードを何度も重複させるなど、どんな方法を使用しても良いので、とにかくテストを通るプログラムを作成します。最後に、テストに通ることを確認しながら、コードの重複などを取り除き、リファクタリングしていきます。
    
    利点
    
    - 開発の途上でも大量のテストを実施する必要があるため、小規模でない限り、手動でテストを行うのは現実的ではなく、テストツールやフレームワークなど何らかのテスト自動化環境を用意してから開発に取りかかるのが、一般的です。
    - 手戻りが起こりづらいです。しかし、その特性上、セキュリティソフトやGUI操作のソフト、並列処理を行うプログラム、開発ツールが自動生成するコードなどには適用しにくいとされています。

</details>

<details><summary>オブザーバビリティ</summary>>
    
    要は観察する能力です。いかに容易にかつ的確に物事を捉えて観察して正解な対処に繋げられるかの指標です。生存者バイアス（あるプロセスを経て得られた事象のみに着目してしまうと、得られなかった事象を見落としてしまうこと）をしっかりと考えて、システム運用に関しても多角的な視点から物事を捉えることが非常に重要になります。
    
    背景
    
    DevOpsとクラウドのコンテキスト
    
    DevOps
    
    - リリースしたサービスが適切に稼働しているか
    - 予期せぬエラーが発生していないか
    - パフォーマンスが劣化していないか
    - UXは向上したか
    - ビジネスにポジティブなインパクトを与えられているか
    
    クラウド
    
    ![スクリーンショット 2022-07-26 14.17.22.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e17798ad-3005-44cb-a531-fa085bf4027c/%E3%82%B9%E3%82%AF%E3%83%AA%E3%83%BC%E3%83%B3%E3%82%B7%E3%83%A7%E3%83%83%E3%83%88_2022-07-26_14.17.22.png)
    
    Retain & Optimize
    
    - モノリシックなアプリケーションを自社のオンプレ環境で動かし、ウォーターホール型の開発手法で数ヶ月から年単位でのリリースサイクルで運用している状態です。クラウド移行前の段階で、DevとOpsがまだ切り離されている状態とも言えます。
    
    Lift & Shift
    
    - クラウド移行の第1段階として、インフラのコスト削減やサーバー調達の短期短縮、オンプレで稼働しているシステムをパブリッククラウドのIaasに移行します。アプリケーションはまだモノリシックな状態であることが多く、DevとOpsの間にも距離があります。
    
    Re-Factor
    
    - その後、クラウドの様々なマネージドサービスやオートスケールを活用することで、システムそのもののアーキテクチャや構成が見直されます。オンプレとは大きく異なり、リソースはエフェメラルなものとして捉える必要が出てきて、運用に大きな変化が現れます。アプリケーションのモジュール化により依存関係が複雑になる傾向があります。
    
    **Re-Architect / Cloud-Native**
    
    - この段階では、サービスはよりスケーラブルに、柔軟なリソースやデプロイを実現するために、コンテナやサーバーレスファンクションといったクラウドネイティブ技術の活用が進みます。結果として、システムの持つ機能が小さな単位のサービスとしてお互いに疎結合するマイクロサービスアーキテクチャが採用され、より複雑な相互依存になります。各サービスの言語やフレームワークは多様になり、ソースコードはコンパクトになります。
    - DevとOpsが緊密に連携し、運用そのものに開発者が当事者として関わることが必須となります。このフェーズでは前述したDevOpsにおけるサービス稼働状態の監視において、監視項目やその手法はもちろん、監視そのものの概念を見直す必要が出てきます。ダイナミックに変化するインフラリソースとライフサイクルの短いコンテナ、サービスの複雑な相互依存関係を前提として環境では、従来の監視は運用できません。さらに近年は可用性やパフォーマンスのサービスレベルが非常にシビアなものとなってます。eコマースでは100ミリ秒のレスポンス低下が7%の売上ダウンにつながる可能性もあると言われています。
    
    **Observability & Monitoring**
    
    Monitoring: 何が起きているのかを見続けること
    
    Observability: 予期せぬことが起きた時になぜそれが起きたのかを把握すること
    
    Observabilityの3つの要素
    
    - メトリクス（何が起きているのか）
    - トレース（どこで問題が起きているのか）
    - ログ（なぜ問題が発生したのか）
    
    従来のシステム監視では、ログに吐き出されるエラーメッセージを監視したり、ログでは判別できない詳細なエラーをAPMで監視したりと、監視ツールそのものが組織に合わせてサイロ化されていました。
    
    Observabilityでは3つの要素をうまく活用して、「どれほど容易に状況を把握し、事象を正確に捉えられるか」「容易に観察することがどれほど担保されているか」がポイントになります。

</details>

<details><summary>EDA: イベントドリブン・アーキテクチャ</summary>
    
    [イベント ドリブン アーキテクチャ | Eventarc | Google Cloud](https://cloud.google.com/eventarc/docs/event-driven-architectures?hl=ja#:~:text=%E3%82%A4%E3%83%99%E3%83%B3%E3%83%88%20%E3%83%89%E3%83%AA%E3%83%96%E3%83%B3%20%E3%82%A2%E3%83%BC%E3%82%AD%E3%83%86%E3%82%AF%E3%83%81%E3%83%A3%E3%81%AF%E3%80%81%E3%83%9E%E3%82%A4%E3%82%AF%E3%83%AD,%E3%81%84%E3%81%9A%E3%82%8C%E3%81%8B%E3%81%AB%E3%81%AA%E3%82%8A%E3%81%BE%E3%81%99%E3%80%82)
    
    データベースを介さないデータ処理が可能であり、従来型のシステム設計とは対照的です。DX時代に増加するリアルタイム性の求められる要件に対応するシステムを構築できるため、必要なデータの取得と、アクションの実行をリアルタイムに実施することが可能です。

</details>


<details><summary>サーバーレス・アーキテクチャ</summary>
    
    常時稼働するサーバー（仮想マシン）を極力使用せずにシステムを構築するアーキテクチャを指します。パブリッククラウドサービスが提供する「イベント駆動型コード実行サービス」ち呼ばれるサービスを構築して使用します。

</details>

<details><summary>マイクロサービス・アーキテクチャ</summary>
    
    近年のDX推進によって、CI/CDによるアジャイル開発への期待が高まっています。しかし、それ以前からそのような動きはありました。2000年代前半から登場したSOA（Service Oriented Architecture：サービス指向アーキテクチャ）です。現在はそのSOAの進化系としてマ**イクロサービスアーキテクチャ**が注目を浴びています。
    
    マイクロサービスでは、アプリケーションの機能を複数の「サービス」として切り分けて部品のように使えるようにしています。サービス間でAPIを連携させて、ネットワーク上で通信しながら1つのアプリケーションを構築します。
    
    例：Uber
    
    GPSやクレジットカード、地図などのサービスをAPIで「手軽に組み合わせて」影響力の大きなビジネスを作り上げた事例として取り上げられる。

</details>


<details><summary>疎結合アーキテクチャ</summary>
    
    あるマイクロサービスの仕様変更が、別のマイクロサービスに影響を及ぼさないようにすること

</details>

<details><summary>ステートレスなアプリケーション、ステートフルなアプリケーション</summary>
    
ステートフル：状態を維持する
ステートレス：状態を維持しない

</details>

## マイクロサービスアーキテクチャ

マイクロサービスの RESTful API 設計における基本的な考え方
https://cloud.google.com/appengine/docs/legacy/standard/java/designing-microservice-api

## IAM

基本的なIAMのリソース階層構造や、Service Account周りの理解を行う
https://blog.g-gen.co.jp/entry/iam-explained

## Cloud Run

- Cloud Run の基本は公式ドキュメントを読み理解しておきましょう。
- Cloud Run はフルマネージドのサーバーレスサービスで、任意のコンテナを実行できるプラットフォームです。
- Cloud Load Balancing の背後に置いて [Web アプリ](https://cloud.google.com/run/docs/triggering/https-request) として動作させることも、 Pub/Sub の push/pull サブスクリプションの背後に置いて [イベントドリブンなプログラム](https://cloud.google.com/run/docs/triggering/pubsub-push) を動作させることも、 Cloud Scheduler によって定期的なジョブとして呼び出すこともできます。
- **[Knative](https://cloud.google.com/knative)** という Google 製のツールがあります。これは「オンプレミス等のプラットフォームで動かす Cloud Run 」と言えます。

## Cloud Functions

- Cloud Functions はフルマネージドのサーバーレスサービスで、任意のコードを動かすことができるサービス (Function as a Service : FaaS) です。Node.js 、 Python 、 Go 、 Java 、 .NET 、 Ruby 、 PHP などに対応しています。
- Cloud Functions のユースケースは Cloud Run のユースケースとよく似ています。これらは Javascript 等で動くフロントエンドサービスのバックエンドプログラムのプラットフォームとして選択することも多いです。

セキュアコーディング

CORS(Cross-Origin Resource Sharing)

- 例えば、フロントエンドのWebサイトのドメイン名とCloud Funstionsに設定するカスタムドメイン名が異なるドメイン名の場合はブラウザのCORSの実装に従い、Access-Control-Arrow-Originのようにレスポンスヘッダを含ませるなどの知識を抑えておきましょう。

[https://qiita.com/att55/items/2154a8aad8bf1409db2b](https://qiita.com/att55/items/2154a8aad8bf1409db2b)

## App Engine

- App Engine はマネージドな Web アプリプラットフォームであり、高度にスケーラブルな構成を簡単に構築できます。開発者は、インフラの構築・運用の工数を省き、アプリケーション開発に集中することができます。
- App Engine に限らず様々なマネージドプラットフォームやコンテナアーキテクチャに共通して言えることですが、アプリケーションはステートレスである必要があります。そのためセッション管理には Redis や Memcached といったインメモリデータベースを利用するというアーキテクチャが、問題文の前提として設定されることが多くなっています。そして Google Cloud では Redis / Memcached のマネージドサービスである Memorystore があり、これもセットで出題されます。

細かいところですが例えば Memorystore を App Engine から利用する場合のアクセス方法を理解しておきます。

- App Engine (Standard) から Memorystore へ接続: サーバレス VPC アクセスが必要
- App Engine (Flexible) から Memorystore へ接続: App Engine が authorized network にいる必要あり

## Cloud Storage

[Cloud Storage(GCS)を徹底解説 - G-gen Tech Blog](https://blog.g-gen.co.jp/entry/cloud-storage-explained)

また記事でも説明されている静的ウェブサイトホスティング機能により Cloud Load Balancing と組み合わせて、ウェブサイトのホスティングに使うことができます。

マルチリージョン の **Cloud Storage + 外部 HTTP ロードバランサー + Cloud CDN 有効化** のようなアーキテクチャにすることで、安価かつフルマネージドな形で世界中の利用者をターゲットとしたウェブサイトを簡単に構築することができます。このような構成にできるということを理解しておきましょう。

## Firestore

- Firestoreはモバイルアプリや Web アプリのバックエンドデータベースとして利用できるマネージドな NoSQL データベースです。

機能( [2種類があり](https://cloud.google.com/datastore/docs/firestore-or-datastore#feature_comparison) )

- 旧称 Datastore から発展した Firestore (Datastore モード)
- Web アプリ・モバイルアプリに最適な Firestore (ネイティブモード)

特にネイティブモードの Firestore について重点的に理解したほうが良いでしょう。

- Firestore ネイティブモードはドキュメント志向データベースであることから、テーブル、カラム、レコードといった概念ではなく、「 **ドキュメント** 」「 **コレクション** 」という概念となっています。この [データモデル](https://firebase.google.com/docs/firestore/data-model) をきちんと理解することを推奨いたします。
- また Firestore ネイティブモードはモバイルアプリを想定しており、モバイル機器のローカル側と Firestore の通信が切れても、ローカル側でデータを保持してアクセスできるようにしておき、 **通信が回復した際に同期** を取るようにすることができます。

また開発担当者の PC のローカル上で稼働する [エミュレーター](https://firebase.google.com/docs/emulator-suite/connect_firestore) も用意されています。

## Compute Engine

Compute Engine のインフラ寄りの内容よりも、アプリケーションのデプロイに関わる点が重視されます。

たとえば VM [メタデータ](https://cloud.google.com/compute/docs/metadata/overview) (インスタンスごとに Key/Value で情報を持たせられる) に、アプリの展開に必要な環境ごとの情報を入れておき、デプロイ処理時 (初期化処理時) にメタデータから情報を読み取って展開に利用する、などのユースケースが出題されます。

またメタデータには「プロジェクトレベルのメタデータ」と「インスタンスレベルのメタデータ」があります。プロジェクトレベルで設定したメタデータは全てのインスタンスから取得でき、インスタンスレベルのメタデータはそのインスタンスからのみ取得できます。

さらにトラブルシュートの方法としてシリアルコンソールを使用したトラブルシューティングについての [ドキュメント](https://cloud.google.com/compute/docs/troubleshooting/troubleshooting-using-serial-console) も目を通しておいてください。

## Monitoring and Logging

[Cloud Loggingの概念と仕組みをしっかり解説 - G-gen Tech Blog](https://blog.g-gen.co.jp/entry/cloud-logging-explained)

[Google Cloud (GCP) Windows VM の Ops エージェント で Cloud Logging に任意のログファイルを収集する方法 - G-gen Tech Blog](https://blog.g-gen.co.jp/entry/opsagent-windows)

## Database

- トランザクション

[https://medium-company.com/トランザクション/](https://medium-company.com/%E3%83%88%E3%83%A9%E3%83%B3%E3%82%B6%E3%82%AF%E3%82%B7%E3%83%A7%E3%83%B3/)

Cloud SQL / Bigtable / Cloud Spanner の [データベースの違い](https://blog.g-gen.co.jp/entry/professional-data-engineer#%E3%81%9D%E3%81%AE%E4%BB%96%E3%81%AE%E3%83%87%E3%83%BC%E3%82%BF%E3%83%99%E3%83%BC%E3%82%B9%E7%A7%BB%E8%A1%8C) を把握しておきましょう。

整合性やトランザクションの有無 (ACID の有無) などをデータのアクセスパターンと照らして選定するはずです。

[Professional Data Engineer試験対策マニュアル。出題傾向・勉強方法 - G-gen Tech Blog](https://blog.g-gen.co.jp/entry/professional-data-engineer#%E3%81%9D%E3%81%AE%E4%BB%96%E3%81%AE%E3%83%87%E3%83%BC%E3%82%BF%E3%83%99%E3%83%BC%E3%82%B9%E7%A7%BB%E8%A1%8C)

## Pub/Sub

Pub/Sub はフルマネージドなメッセージキューイングサービスです。

システムコンポーネント同士を **疎結合にする** ために重要なサービスであり、クラウドらしいアーキテクチャの要となります。

Pull サブスクリプションと Push サブスクリプションの [2 種類がある](https://cloud.google.com/pubsub/docs/subscriber) 点、またストリーミングデータの受け口としても使われる点などから、 Amazon Web Services (AWS) でいう Amazon SQS 、 Amazon SNS 、 Amazon Kinesis を組み合わせた位置付けのサービスとなっています。

Cloud Logging の [シンク機能](https://blog.g-gen.co.jp/entry/cloud-logging-explained#%E3%82%B7%E3%83%B3%E3%82%AF%E3%81%A8%E3%81%AF) と組み合わせて、ログを収集しリアルタイムに別のプログラムに Push するような動かし方も可能です。


## 開発環境

**[Cloud Code](https://cloud.google.com/code)** というツールの存在程度は押さえておきましょう。

## Cloud Build(CI/CD)

Google Cloud で CI/CD パイプラインを構築する際に要になるのは **Cloud Build** です。

Cloud Build はその名の通り、ソフトウェアのビルドのためのサービスですが、 Google Cloud 上の各プラットフォームへのデプロイにも用いることが可能です。ソースコードレポジトリへの Push を検知して Code Build が動き、ビルド・テスト・デプロイを実施させることができます (例: [GKE へのデプロイ](https://cloud.google.com/build/docs/deploying-builds/deploy-gke)) 。

なお Cloud Build には **[ステップ](https://cloud.google.com/build/docs/build-config-file-schema?hl=ja#build_steps)** (step) という概念があります。ステップはその名の通りビルドの各ステップを処理する単位ですが、ステップごとにマネージドなコンテナが起動して処理を行います。

YAML または JSON で記述した構成ファイルに、一つ以上のステップを定義し、実行することでビルドやデプロイを実行するイメージです。各ビルドステップは別々のコンテナで実行されますが `/workspace` 以下に残したファイルは **ステップ間で引き継がれます** 。

## 脆弱性の管理

CI/CD にセキュリティの概念を取り込み、開発・運用にセキュリティ担保の仕組みを継続的に取り込む体制は近年、 DevSecOps とも呼ばれます。

Google Cloud ではこれを実現する仕組みも存在します。

例えば脆弱性があるバージョンのミドルウェアを含んだコンテナがデプロイされないようにしたい場合、Cloud Build でビルド → コンテナイメージは Artifact Registry (試験では前身である Container Registry が選択肢として提示) に格納しますが、ここに対する [コンテナイメージの自動スキャン](https://cloud.google.com/artifact-registry/docs/analysis) を有効化することで、自動的なセキュリティ施策とすることができます。

またスキャンで問題がなかったコンテナイメージにのみ署名を付与し **[Binary Authorization](https://cloud.google.com/binary-authorization/docs/cloud-build)** により署名がないイメージのデプロイを禁止することで、セキュリティ担保の一定の向上が見込めます。

## 監視（Observability）

[Google Cloud(GCP)のCloud Monitoring解説 (基本編) - G-gen Tech Blog](https://blog.g-gen.co.jp/entry/cloud-monitoring-explained)

**Cloud Trace** は、アプリケーションの **分散トレース** を実現する仕組みです。アプリケーションがユーザのリクエストを処理するのにかかる時間を計測したり、マイクロサービス間のレイテンシを継続できるので、 **SLI/SLO の計測** 等に利用できます。アプリケーションに必要なクライアントライブラリを追加し、必要なコードを追加することで利用可能になります。

**Cloud Profiler** はアプリケーションの CPU やメモリなど **リソース使用状況** を継続収集するための仕組みです。アプリケーションの中でソースコードのどの部分が最もリソースを消費しているのかを特定できるので、非効率なアプリケーションの **オーバーヘッドの特定** に利用できます。

**Cloud Debugger** はアプリケーション実行環境にデバッガライブラリをインストールすることでコードごとの **デバッグに活用** できる機能です。

## Cloud Endpoints

**Cloud Endpoints** は公開 API を実装するためのサービスです。Cloud Endpoints を介して API を公開することで **モニタリング、セキュア化、分析、クォータの設定** などが実現できます。

Cloud Endpoints では Nginx ベースの **Extensible Service Proxy (ESP)** と呼ばれるプロキシ機能により機能提供がされます。 ESP は「 Cloud Load Balancing の後ろ」「 VM / GKE などバックエンドアプリケーションの手前」に配置されます。

ドキュメント [Architectural overview of Cloud Endpoints](https://cloud.google.com/endpoints/docs/openapi/architecture-overview) の構成図をよく覚えておいてください。この構成図の中で ESP がどこに配置されているか = Cloud Endpoints の配置場所を分かっているだけでも回答に役立ちます。