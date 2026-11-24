# MIZUBE 日本の水域データ

© OpenStreetMap contributors

このデータベースはOpenStreetMapを加工した派生データベースです。
Open Data Commons Open Database License (ODbL) 1.0に従って利用・複製・改変・再配布できます。

- ライセンス本文: https://opendatacommons.org/licenses/odbl/1-0/
- 原典・著作権: https://www.openstreetmap.org/copyright
- 元データ配布: https://download.geofabrik.de/asia/japan-261118.osm.pbf
- 元データ時点: 2026-11-18T21:21:02Z
- 加工者: Studio Saitama / MIZUBE
- 加工内容: 水路と水面の抽出、OSM relationの水面組立て、海岸線（natural=coastline）の線としての抽出、名前の付いた港・浜・岬・湾の位置（点。wayは構成点の平均）の抽出、SQLite/R-treeと整数座標への格納。連続する同一座標だけを除き、簡略化・補間・海岸線からの海域推定は行っていません。

配布者は、加工DB本体を受領者が機械可読形式で入手できるようにし、出典とライセンスを維持してください。アプリの共有機能では公開DBのgzip分割ファイル・manifest・この通知を渡します。manifestのparts順にバイト列を連結してgzipを展開すると、元のSQLiteを完全に復元できます。各部分と展開後SQLiteのSHA256をmanifestに記載しています。アプリやストアの条件がODbL上の再利用を制限する場合は、制限のないDBコピーも入手できるようにしてください（ODbL 4.7）。

これは地図の参考データです。名称の欠落、古い形状、不完全なOSM参照、GPS誤差があり得ます。名称や位置の正確性・全国の全水域の網羅を保証しません。測定対象の水域を確定する根拠として単独で使用せず、曖昧な場合は名称未特定として扱ってください。

私有の利用者座標、水温、釣行記録は含みません。featuresテーブルにはOSM地物ID、名称、種別、形状だけを格納し、OSM編集者情報・変更履歴・管理者タグは格納しません。
