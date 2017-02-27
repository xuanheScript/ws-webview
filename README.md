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

| func | value | type | return | required/optional | comment |
| --- | --- | --- | --- | --- | --- |
| getUserInfo | undefined | undefined | object | optional | 返回用户信息，未登录return {} |
| showGoodsDetail | id | number | undefined | required | 跳转到商品详情 |
| showStoreDetail | id | number | undefined | required | 跳转到商户详情 |
| showCrowdfundDetail | id | number | undefined | required | 跳转到众筹详情 |
| photoGallery | images,index | array,number | undefined | required | 调起图片查看器 images:['url1','url1'] |
| alert | title,message,buttons | string,string,array | undefined | required,optional,optional | buttons:[{text:string,onPress:func}] |
| loadding | action,title | string,string | undefined | required,optional | action:PropTypes.oneOf(['show','hide'] |
| pushLogin | undefined | undefined | undefined | optional | 跳转到登陆 |
| pushWebView | url | string | undefined | required | 打开一个内部webview地址,url:demo/test1?id=1 |
| popWebView | undefined | undefined | undefined | optional | 关闭当前的webview导航 |
| openWebView | url | string | undefined | required | 打开一个外部webview地址,完整的url |
| toast | text | string | undefined | required | 注:使用子方法，不能直接使用 例: toast.show('');toast.info('');toast.warn('');toast.error('') |
