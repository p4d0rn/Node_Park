* nodejs 会把同名参数以数组的形式存储，并且 JSON.parse 可以正常解析

* 字符`ı`、`ſ` 经过toUpperCase处理后结果为 `I`、`S`

* 字符`K`经过toLowerCase处理后结果为`k`(这个K不是K)

* `jsonwebtoken`模块的一个trick

  ```js
  jwt.verify(token, secret, {algorithm: "HS256"});
  ```

  当`secret`为`''`或`undefined`，若`token`的`header`指定的`algorithm`为`none`，则无签名算法。

  （若`secret`不为空，即使`token`的`header`指定空算法也没用）