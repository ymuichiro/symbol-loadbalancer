# symbol-loadbalancer

## 環境構築

### インストール
* Let's Encrypt
* Nginx

### 手順
* VM の手配 + 80/443 ポート解放
* ドメインの手配 + VM へ連携
* 必要なソフトウェアをインストール
* Let's Encrypt にてSSL証明書作成
* Nginx の default コンフィグへ本レポジトリの内容を反映
* Nginx の起動

## 注意事項
* ip_hash の有効化は必要（同一IPは同一ノードへ振り分け。接続先が死んでいる時は別ノードへ）
* 委任は直接の方が好ましい
* VPS の場合はトラフィック固定プランで（従量だと危険）

以上
