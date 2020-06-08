## [Fetch](https://developer.mozilla.org/zh-CN/docs/Web/API/Fetch_API)

### Fetch 接口
- fetch():用于获取资源
- Headers:相当于 reponse/request 的头信息
- Request:相当于一个资源请求
- Response:相当于请求的响应

### Fetch mixin
- Body：提供了关联 response/request 中 body 的方法，可以定于它的文档类型以及如何被处理


### 注
- HTTP 错误时 fetch() 不会标记为 reject，即使时404或500。状态会被标记为resolve但 resolve的返回值 ok 会设置为false。仅当网络故障时或请求被阻止时，才会标记为reject。
- 默认情况下 fetch 不会从服务器发送或接收任何cookies，要发送cookies 必须设置 credentials 选项。
    - credentials
        - incluede:发送包含凭据的请求
        - same-origin：请求URL 与调用脚本同源时发送凭据
        - omit：不发送凭据
