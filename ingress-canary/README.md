访问正式版本
```
$ curl http://web.sundayhk.com
hello web prod@!!!
```
访问灰度版本
```
$ curl -H "canary: true" http://web.sundayhk.com
hello web gray@xxx
```

基于Cookie的灰度不支持设置自定义，只有always和never。
灰度优先级顺序：基于Header > 基于Cookie > 基于权重（从高到低）。

