
curl -H 'gray: true' web.sundayhk.com

curl --cookie 'guangzhou=always' web.sundayhk.com

说明:
  - 基于Cookie的灰度不支持设置自定义，只有always和never。
  - 灰度优先级顺序：基于Header > 基于Cookie > 基于权重（从高到低）。
