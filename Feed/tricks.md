* nodejs 会把同名参数以数组的形式存储，并且 JSON.parse 可以正常解析
* 字符`ı`、`ſ` 经过toUpperCase处理后结果为 `I`、`S`
* 字符`K`经过toLowerCase处理后结果为`k`(这个K不是K)