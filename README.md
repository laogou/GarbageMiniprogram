# 垃圾分类小程序
## 云开发
> 不了解小程序云开发请访问[文档](https://developers.weixin.qq.com/miniprogram/dev/wxcloud/basis/getting-started.html)

云函数，云数据库：
- 数据库：存储四种垃圾分类的相关垃圾数据， 创建表commit,sort，product。把sort.json 和product.csv 导入云数据库即可
- 云函数：获取百度识别库的accessToken
[百度AI识别库地址](http://ai.baidu.com/docs#/ImageClassify-API/ebc492b1)
[QQ AI地址](https://ai.qq.com/)

## key 
1. 小程序key 在文件project.config.json->appid 记住创建小程序的时候选择云开发
2. 百度key 主要做拍照识别的cloudfunctions->baiduAccessToken->index->apiKey和secretKey
此处替换为：API Key 和 Secret Key
3. 智能询问采用ai.qq 的智能闲聊接口 key在pages->android->qa->app_id和appKey 


## 常见错误
1. 没有自己部署云函数
2. 数据库没有给与相应的权限，最好给最大权限
3. 需要的key 配置错误。
4. 没有创建数据库名称



 


