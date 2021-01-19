# Jd_Seckill

##### 非常感谢原作者 https://github.com/zhou-xiaojun/jd_mask 提供的代码
##### 也非常感谢 https://github.com/wlwwu/jd_maotai 进行的优化

## 主要功能

- 登陆京东商城（[www.jd.com](http://www.jd.com/)）
  - cookies登录 (需要自己手动获取)
- 预约茅台
  - 定时自动预约
- 秒杀预约后等待抢购
  - 定时开始自动抢购

## 运行环境

- [Python 3](https://www.python.org/)

## 第三方库

- 需要使用到的库已经放在requirements.txt，使用pip安装的可以使用指令  
`pip install -r requirements.txt`

## 使用教程  
#### 1. 网页扫码登录
#### 2. 填写config.ini配置信息 
(1)eid,和fp找个普通商品随便下单,然后抓包就能看到,这两个值可以填固定的 
> 在结算页面F12的Sources内右侧watch，点击加号填入_JdTdudfp，即可看到该参数的内容，edi与fp均在其中

* 第一步：进入京东结算页面

* 第二步：f12打开Sources

* 第三步：右侧的watch，点击加号，填入_JdTdudfp

* 即可看到_JdTdudfp:Object

(2)cookies_string,sku_id,DEFAULT_USER_AGENT(和cookie获取同一个地方就会看到.直接复制进去就可以了) 
>这里注意每次扫码登陆后都需要重新获取cookies_string,其他两个不用  
>sku_id我已经按照茅台的填好 

(3)配置一下时间
 
以上都是必填的.

#### 3.运行main.py 
根据提示选择相应功能即可
