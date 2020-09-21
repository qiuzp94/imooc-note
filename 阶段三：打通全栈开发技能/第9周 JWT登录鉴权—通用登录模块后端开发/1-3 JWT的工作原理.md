## 什么是JWT
**JWT**的全称是**J**SON **W**eb **T**oken,一个JWT由三部分构成:Header,Payload,Signature。


一个例子
### Header

```
{
    "alg":"HS256",
    "tyo":"JWT"
}
```

### Payload

```
{
    "sub":"2020-9-20",
    "name":"zzz",
    "admin":true
}
```

### Signature

```
HMACSHA256(
    base64UrlEncode(header) + "." +
    base64UrlEncode(payload),
    secret
)

```

## JWT特点
* 防CSRF(主要是伪造请求,带上Cookie)
* 适合移动应用
* **无状态，编码数据**

## JWT工作原理
 ![JWT工作原理.png](https://i.loli.net/2020/09/20/Elhi4YXytCPdn3z.png)

  