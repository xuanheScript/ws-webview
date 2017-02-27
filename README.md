# ws-webview
ws-webview api说明

## Overview
只作用于文率科技内部webview的api说明，源码只作用于webview内部

## Note
使用前最好先检测api对象是否存在


```javascript
 tyof(ws)!= undefined && ...
```


### ws

| func | value | return | required/optional | comment |
| --- | --- | --- | --- | --- |
| getUserInfo | undefined | object | optional | 返回用户信息，未登录return {} |
| showGoodsDetail | number | undefined | required | 跳转到商品详情 |
| showStoreDetail | number | undefined | required | 跳转到商户详情 |
| showCrowdfundDetail | number | undefined | required | 跳转到众筹详情 |
| photoGallery | array,number | undefined | required | 调起图片查看器 array:['url1','url1'] number:index |
