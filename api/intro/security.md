## 安全说明
### public key & private key
商户的 ```public key``` & ```private key``` 非常重要，请勿显示在任何网页代码、网址参数中，以免泄漏发生意外的安全风险。

### signature
为保障接口安全，系统端会对接收到的所有数据，使用 ```signature``` 匹配校验，防止数据被非法篡改。

> 建议商户端对接收到的数据，同样进行 ```signature``` 匹配校验，防止意外的安全风险。

### 操作校验
对于钱包提现、密码更新等敏感操作，建议商户完善安全邮箱，并开启相关操作的二次安全校验。

### HTTPS
部分接口需要提供 notify_url & redirect_url，建议商户对服务器部署 ```https``` 服务，保障数据的通信安全。