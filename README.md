# zfaka-payjz

## 基于ZFAKA二次开发，添加PayJZ支付渠道

### 关于ZFAKA，请移步：[ZFAKA](https://github.com/zlkbdotnet/zfaka)

免费、安全、稳定、高效的发卡系统，值得拥有!
演示地址：http://faka.zlkb.net/

### 关于PayJZ

+ PAYJZ 旨在解决需要使用交易数据流的个人、创业者、个体户等小微支付需求，帮助开发者使想法快速转变为原型，PAYJZ 自身不做收单和清算，只做微信支付个人接口对接的技术服务，具体详情请去官网了解
+ 注册链接：[PAYJZ官网](https://payjz.cn/ref/ndkedl)

### 为什么对接PayJZ

原本ZFAKA对接了很多支付方式，经过尝试后发现存在以下问题：

+ 二清类：大多数个人支付方式都采取这种方式，最大的风险就是结算方跑路
+ 监听类：此类方法也非常多，需要下载APP或者PC端软件24小时监听，最大风险是不稳定，丢单等情况时有发生

### 修改了哪些内容

1. 保留其他所有支付方式接口
2. 增加了PayJZ支付接口

### 支持哪些支付接口

1. 用户扫描二维码、二维码识别、收银台支付接口模式
2. H5支付接口，允许用户在手机浏览器打开网页，支付时调起微信进行支付，域名必须备案。

### PayJZ微信支付演示地址
[PAYJZ 支付演示](https://fk.payjz.cn/)

## 开始打补丁

补丁只针对特定版本，目前已经支持最新1.4.4

### 开始打补丁

clone zfaka源代码，或直接下载release版本，目前版本号为1.4.4

```
cd [你的网站路径]
git clone -b 1.4.4 https://github.com/zlkbdotnet/zfaka
cd zfaka
git clone https://github.com/hiyouli/zfaka-payjz
patch -p1 < ./zfaka-payjz/v1.4.4-payjz.patch
```

完成
然后正常安装使用即可

### 交流

Q群：48240181
