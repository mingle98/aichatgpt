# 一、百度文心一言API
基于百度文心一言语言大模型的智能文本对话AI机器人API,支持聊天对话、行业咨询、语言学习、代码编写等功能.

# 二、使用步骤
## 1、接口

***重要提示:建议使用https协议,当https协议无法使用时再尝试使用http协议***

请求方式: POST

```
https://luckycola.com.cn/ai/openwxyy
```
## 2、请求参数
| 序号 | 参数 | 是否必须|说明 |
|--|--|--|--|
| 1 |ques  |是 | 你的问题 |
| 2 |appKey  |是 | 唯一验证AppKey, 可前往官网“个人中心“获取([http(s): //luckycola.com.cn](http://luckycola.com.cn)), 下面具体介绍获取方法|
| 3 |uid  |是 | 账号等唯一标识, 可前往官网“个人中心“获取([http(s): //luckycola.com.cn](http://luckycola.com.cn)), 下面具体介绍获取方法|
| 4 |isLongChat  |否 | 是否支持上下文(值为1或者0),1表示支持上下文,默认值0不支持|


**注意!!!: 如果您还没有appKey和uid,请先请前往官网获取**
官网地址:[http(s): //luckycola.com.cn/](http://luckycola.com.cn/)


## 3、请求参数示例

```json
{
   "ques": "hello",
   // 官网-个人中心-Appkey获取
   "appKey": "643************c3",
   // 官网-个人中心-用户ID
   "uid": "y*************6",
   // 是否支持上下文 值1表示支持,0表示不支持
   "isLongChat": 0
}
```

## 4、接口 返回示例
```json
{
	// 	成功状态码
	"code": 0,
	// 	成功提示
	"msg": "AI接口返回成功",
	"data": {
		// 	AI回答结果
		"result": "您好，您似乎输入了一个文本字符串。如果您需要帮助或有任何问题，请随时告诉我，我将竭诚为您服务。",
		"countMsg": "无穷",
		// 当前是否是上下文对话模式,1表示是上下文模式,0为非上下文模式
		"longChat": 0
	}
}
```

# 三、 如何获取appKey和uid

### 1、申请appKey:
登录**Luckycola官网**([http(s): //luckycola.com.cn](http://luckycola.com.cn)),进入“[**个人中心**]“,即可进行申请
![在这里插入图片描述](https://img-blog.csdnimg.cn/684861db7426459c8790f65d3e0b0c84.png#pic_center)

### 2、获取appKey和uid
AppKey申请通过后,登录**Luckycola官网**([http(s): //luckycola.com.cn](http://luckycola.com.cn)),进入“[**个人中心**]“即可获取
![在这里插入图片描述](https://img-blog.csdnimg.cn/3112de0520cf4ecfa2edddefc7a15fd2.png#pic_center)


# 四、重要说明
**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!

**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!

**重要提示:** 您的AppKey和uid是重要信息,请务必妥善保存,避免泄漏!
