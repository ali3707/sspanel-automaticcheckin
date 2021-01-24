# sspanel-automaticcheckin
基于项目https://github.com/zhjc1124/ssr_autocheckin 修改，暂未解决登陆人机验证问题。

***其他主题适配请issues***

**Tip:此流量不是手机运营商流量，是科学上网的流量，懂得自然懂。机场地址填机场官网地址，不是填订阅的地址，注意这一点。有问题欢迎issues**


# 用法

1. 下载本仓库，将`sspanel_qd.py`上传到腾讯云函数
2. 配置`sspanel_qd.py`中的`init`(如下)
 ```
 def __init__(self):
        # 机场地址
        self.base_url = 'https://****.net'
        # 登录信息
        self.email = '****@qq.com'
        self.password = '****'
        # Server酱推送
        self.sckey = 'SCU109245Tf34928bcea84db0a*************'
        # 酷推qq推送
        self.ktkey = '**********'
  ```
  3. 配置云函数定时触发
  
# 云函数运行截图
![wRbQAJ.png](https://s1.ax1x.com/2020/09/17/wRbQAJ.png)

# 云函数报错解决
- {"errorCode":-1,"errorMessage":"Invoking task timed out after 3 seconds"} -- 函数运行超时，按下图设置：
  - ![0gIMm6.png](https://s1.ax1x.com/2020/10/11/0gIMm6.png)
  
# 更新
- 20200915-第一个版本，支持签到、Server酱微信推送
- 20200917-修复非editXY主题运行时报错问题，增加酷推QQ推送

# 个人用过的机场推荐
| 名字 | 地址 |
|  ----  | ----  |
| 跑路云 | 国内域名 paoluz.pw  跑路云.co |
| 魔戒 | 魔戒.com mojie.me |

# Clash
- Clash For Android   [点击下载](https://ghproxy.com/https://github.com/Kr328/ClashForAndroid/releases/download/v2.1.5/app-universal-release.apk)
- Clash For Windows   [点击下载](https://ghproxy.com/https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.14.1/Clash.for.Windows.Setup.0.14.1.exe)
- Shadowrocket For IOS/IPAD 
- Clash For Windows - Mac版     [点击下载](https://ghproxy.com/https://github.com/Fndroid/clash_for_windows_pkg/releases/download/0.13.0/Clash.for.Windows-0.13.0.dmg)

