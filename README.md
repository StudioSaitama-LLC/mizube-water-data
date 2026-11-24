# MIZUBE water data

Regional extracts of rivers, lakes, canals, coastlines and named harbour / beach / cape / bay points in Japan, derived from OpenStreetMap. The MIZUBE QUEST app downloads only the region it needs to name a waterside from a saved GPS position.

- Data: © OpenStreetMap contributors, licensed under the [Open Database License (ODbL) 1.0](https://opendatacommons.org/licenses/odbl/1-0/). See [ODbL-NOTICE.md](ODbL-NOTICE.md).
- Source: Geofabrik Japan extract (`japan-261118.osm.pbf`, 2026-11-18).
- Processing: Studio Saitama / MIZUBE. Waterways and water areas extracted as-is (no simplification); the country-wide database is split into 0.5° × 0.5° cells, each including features within a 0.05° margin.
- Files are attached to the release named after the data version. `japan-water-regions.json` lists every region with its size and SHA-256.
- Format: gzip-compressed SQLite (`metadata`, `features`, `feature_bounds` R-tree). The `metadata` table describes the geometry encoding.
- This is reference geometry. Neither GPS precision nor correct identification of a water body is guaranteed.

日本の川・湖・水路・海岸線と、名前の付いた港・浜・岬・湾の位置を、OpenStreetMap から取り出して地域ごとに分けたデータ。MIZUBE QUEST が、保存した位置から水辺の名前を出すために、必要な地域の分だけを取る。
