## **一键签到【芥子空间】【葫芦侠】**
更新日期：2021/07/08 

### 免责声明
**其他人使用本仓库的内容，本人不负任何责任。**

---
### 说明
【葫芦侠签到】和【芥子空间】都是用` key值 `来签到
 
 **需要**：两个软件各自的KEY值，和微信公众号【pushplus推送加】（用于完成后推送，可选）

#### 不同的是：
#### **【葫芦侠3楼】**

可获取多个KEY，登陆也不受影响，这个版本不是用账号密码来签到的，因为用账号密码的可以获得key，但是github actions每次都是新的运行环境，无法保存签到后获取的的Key值，没必要每次签到都登陆一次吧，所以就弄成需要key值的。抓包用黄鸟（Http Canary），没有固定证书，随便抓包


提示:此脚本可以签到一些**隐藏**的板块，具体看签到完成后的推送

#### **【芥子空间】**
 
这个有点大问题，只能获取一个key，且证书固定，难以抓包，且只能第三方一键登陆和验证码登陆。
 
这里需要懂得抓包 ，软件用：【黄鸟（Http Canary） + [TrustMeAlready](https://github.com/ViRb3/TrustMeAlready)】

 这里需要xposed环境 是因为后者软件就是xp模块，用来解除证书固定的
 
 不需要root也能解决的方法也有，自行查找
 
 **难以抓包的话，建议不要尝试抓包这个方法了。**

放个链接（这样也能获取芥子空间的key，但是app里已经登陆了的会给你下线）：

 `https://api.bbs.lieyou888.com/user/phone/login/ANDROID/1.1?phone=手机号&vcode=验证码`
 
 【填上相应的号码，复制打开网页就能看见key值了】
 
---
### 简单配置
新建仓库，然后复制我的仓库链接

点击仓库的【settings】 - 【secret】 - -【New repository secret】

芥子空间：key填 ` jzkjk `，value填相对应的变量值

葫芦侠3楼： key填 `hlxk` ， value填相对应的变量值

推送加的**token** ：key填 ` token `，value填相对应的变量值  （此变量可选）

应该没人不会填吧

----

【默认每天凌晨4点50分自动签到】

如果需要，请自己在`.yml`文件修改时间




