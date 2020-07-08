## kubernetesのAPI機能を拡張する方法

- Admission Webhook  
    - APIリクエストを変更・検証するためのWebhookを追加するための方法
    - APIリクエストにデフォルト値を設定するようなケース
- CRD  
    - 独自Resourceを定義するAPI拡張方法
- API Aggregation
    - kube-api-server以外にcustom api-serverを実装し・拡張するための方法
    - API Serverの処理途中でHookするため、CRDよりも自由度が高い

拡張方法の自由度: Admission Webhook < CRD < API Aggregation