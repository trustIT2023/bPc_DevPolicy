# クラウド

> [!IMPORTANT]  
> **クラウドとしてMicrosoft Azureを採用**

## 基本概念

- [かんたん理解 正しく選んで使うためのクラウドのきほん Amazon Web Services・Azure・Google Cloudを横断的に理解しよう](https://www.amazon.co.jp/%E3%81%8B%E3%82%93%E3%81%9F%E3%82%93%E7%90%86%E8%A7%A3-%E6%AD%A3%E3%81%97%E3%81%8F%E9%81%B8%E3%82%93%E3%81%A7%E4%BD%BF%E3%81%86%E3%81%9F%E3%82%81%E3%81%AE%E3%82%AF%E3%83%A9%E3%82%A6%E3%83%89%E3%81%AE%E3%81%8D%E3%81%BB%E3%82%93-Amazon-Services%E3%83%BBAzure%E3%83%BBGoogle-Cloud%E3%82%92%E6%A8%AA%E6%96%AD%E7%9A%84%E3%81%AB%E7%90%86%E8%A7%A3%E3%81%97%E3%82%88%E3%81%86/dp/4839972753/ref=sr_1_5?__mk_ja_JP=%E3%82%AB%E3%82%BF%E3%82%AB%E3%83%8A&crid=PUET3K9M2P62&keywords=%E3%82%AF%E3%83%A9%E3%82%A6%E3%83%89&qid=1688738827&s=books&sprefix=%E3%82%AF%E3%83%A9%E3%82%A6%E3%83%89%2Cstripbooks%2C345&sr=1-5)

## 3大クラウド比較

Azure、Google Cloud Platform (GCP)、および Amazon Web Services (AWS) は、現在市場で最も支配的な三大クラウドサービスプロバイダーです。これらのプラットフォームを比較することで、ビジネスやプロジェクトに最適なクラウドソリューションを選択する際の参考になります。

### 比較表

| 特性/プラットフォーム      | Microsoft Azure        | Google Cloud Platform (GCP) | Amazon Web Services (AWS) |
|--------------------------|------------------------|-----------------------------|---------------------------|
| 市場のシェア           | 高                      | 中                           | 最高                      |
| 主な強み               | エンタープライズ統合     | データ分析、機械学習         | 汎用性、機能の豊富さ        |
| サービス範囲           | 広範                     | 広範                         | 最広範                    |
| プライシング           | 競争力あり                | 競争力あり                   | 競争力あり                |
| ユーザーインターフェイス | 直感的                   | 直感的                       | 複雑                      |
| データセンターの位置   | 全世界                   | 全世界                       | 全世界                    |
| 主要顧客層             | 大企業、エンタープライズ  | テクノロジー重視の企業       | 広範な顧客層               |
| 開発者ツール           | 優秀                     | 優秀                         | 優秀                      |
| 機械学習とAI           | 強力                     | 最先端                       | 強力                      |
| IoTサポート            | 優秀                     | 優秀                         | 優秀                      |
| ハイブリッドクラウド   | 強力                     | サポートあり                 | 強力                      |

### 詳細解説

- 市場のシェア: AWSはクラウド市場において最も大きなシェアを持っており、最も早くからクラウドサービスを提供し始めたため、非常に広範な顧客基盤を持っています。Azureはマイクロソフトのエンタープライズ顧客によって強く支持され、GCPは特にデータ分析と機械学習で急速にシェアを拡大しています。

- 主な強み:
  - Azure: 既存のMicrosoft製品（Office 365、Windows Serverなど）との統合が深く、企業のデジタル変革を強力にサポート。
  - GCP: データ分析と機械学習ツールにおいて特に強く、Googleの独自技術（BigQuery、TensorFlowなど）を活用可能。
  - AWS: 一般的なクラウドニーズに対して最も多くのサービスとツールを提供し、スタートアップから大企業まであらゆる規模の企業に対応。

- プライシング: 三者とも似たような価格設定をしており、実際のコストは使用するサービスの種類や規模によって大きく異なります。各プロバイダーは価格計算ツールを提供しており、見積もりが可能です。

- ユーザーインターフェイス: AWSの管理コンソールは機能豊富である一方で複雑さも指摘されています。AzureとGCPは比較的使いやすいと評価されていますが、直感的な操作性を提供するためにデザインが常に更新されています。

この比較は、各クラウドサービスの強みと弱みを理解するのに役立ちます。最終的な選択は、特定の技術要件や既存のインフラストラクチャ、予算など、プロジェクト固有の要因に基づくべきです。

## クラウド比較その他参考

- [AWS、Azure、GCP それぞれのクラウドの特徴やメリット](https://cloud-ace.jp/column/detail393/)
- [Microsoft azureでできることは何？個人利用の際の使い道も解説](https://itpropartners.com/blog/14277/)
- [3大クラウドサービスをわかりやすく比較](https://cloud-ace.jp/column/detail295/)
- [【徹底比較】AWS・GCP・Azureの違い](https://www.skillupai.com/blog/cloud-comparison/)
- [Azure・AWS 徹底比較](https://www.softbanktech.co.jp/special/blog/it-keyword/2022/0013/)
- [AWSとGCPのメリット4つとデメリットを比較](https://tenshoku-careerchange.jp/column/204/)
- [VPSとAWS。クラウドサービスを比較して分かる両者の違いとは](https://www.winserver.ne.jp/column/vps-aws_distinction/)

## AzureのGCPやAWSと比べた優位性

- AI:ChatGPT,Copilotのサーバー上での実行
- API:WebAPIの提供、
- Office365:グループウェアNo1,Copilotとの融合の利用が可能
- 開発環境:VS CodeやGitHubとの高度な融合性
- RPA:自動化や各種システムとの連携

## 引用文献

> ChatGPT  
