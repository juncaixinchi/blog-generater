---
title: Common Http Code
date: 2019-1-2 19:50:27
tags:
---

### 常见的HTTP Code

<!-- more -->

+ 2**开头 （请求成功）表示成功处理了请求的状态代码。

  - 200 （成功） 服务器已成功处理了请求。 通常，这表示服务器提供了请求的网页。

  - 206 （部分内容） 服务器成功处理了部分 GET 请求。

+ 3** 开头 （请求被重定向）表示要完成请求，需要进一步操作。 通常，这些状态代码用来重定向。

  - 301 （永久移动） 请求的网页已永久移动到新位置。 服务器返回此响应（对 GET 或 HEAD 请求的响应）时，会自动将请求者转到新位置。

  - 302 （临时移动） 服务器目前从不同位置的网页响应请求，但请求者应继续使用原有位置来进行以后的请求。

  - 304 （未修改） 自从上次请求后，请求的网页未修改过。 服务器返回此响应时，不会返回网页内容。

+ 4**开头 （请求错误）这些状态代码表示请求可能出错，妨碍了服务器的处理。

  - 400 （错误请求） 服务器不理解请求的语法。

  - 401 （未授权） 请求要求身份验证。 对于需要登录的网页，服务器可能返回此响应。

  - 403 （禁止） 服务器拒绝请求。

  - 404 （未找到） 服务器找不到请求的网页。

  - 414 （请求的 URI 过长） 请求的 URI（通常为网址）过长，服务器无法处理。


+ 5**开头（服务器错误）这些状态代码表示服务器在尝试处理请求时发生内部错误。 这些错误可能是服务器本身的错误，而不是请求出错。
 
  - 500 （服务器内部错误） 服务器遇到错误，无法完成请求。

  - 501 （尚未实施） 服务器不具备完成请求的功能。 例如，服务器无法识别请求方法时可能会返回此代码。

  - 502 （错误网关） 服务器作为网关或代理，从上游服务器收到无效响应。

  - 503 （服务不可用） 服务器目前无法使用（由于超载或停机维护）。 通常，这只是暂时状态。

  - 504 （网关超时） 服务器作为网关或代理，但是没有及时从上游服务器收到请求。