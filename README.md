# 🌟 解锁TikTok+换区+发视频+无水印下载+直播(iPhone)

### 目录

* [支持的TikTok功能](#支持的TikTok功能)
* [准备工作](#准备工作)
* [关于换区](#关于换区)
* [操作步骤](#操作步骤)
* [感谢](#感谢)

### 支持的TikTok功能

***

* ★★★推荐：港区TikTok
    * 下载方式：在港区App Store搜索 tiktok 并下载
    * 支持功能：
    * - [x] TikTok换区
    * - [x] 发视频、看视频
    * - [x] 点赞
    * - [x] 评论
    * - [x] 能看不同的Discover话题标签
    * - [ ] 无TikTok直播
    * TikTok版本：v8.2.0
    * iOS系统版本：13.1.2，其他版本请自行测试是否可行
    * **港区下载的TikTok与美区下载的TikTok可共存**
* 美区TikTok
    * 下载方式：在美区App Store搜索 tiktok 并下载
    * 支持功能：
    * - [ ] 换区不太灵
    * - [x] 看视频
    * - [ ] 能否发视频，不确定（我发视频，提示视频在审核中）
    * - [x] 点赞
    * - [x] 评论
    * - [x] 部分账号能看TikTok直播
    * TikTok版本：v13.2.2
    * iOS系统版本：13.1.2，其他版本请自行测试是否可行
    * **美区下载的TikTok与港区下载的TikTok可共存**

### 准备工作

***

* - [x] 港区/美区Appstore下载TikTok
    * 共享账号：
        * 港区Apple ID、密码
            * cyubuchen@tom.com
            * Cyubuchen2019
        * 美区Apple ID、密码
            * cyubuchen@163.com
            * Cyubuchen201906
        * 别登录iCloud!!!
        * 密码若不对，可在微信公众号：`c鱼不沉`内回复`账号`获取

* - [x] 自备[Quantumult](https://apps.apple.com/us/app/quantumult/id1252015438?ls=1)
    * 可在美区App Store获取
* - [x] 自备代理，ss/ssr/vmess等

### 关于换区

***

* 解锁并换区：将`CN`改为想看的国家/地区的2位`大写`英文简写，用Quantumult实现

    * 在`HTTP复写`中，将`CN`的替换值改为`SG`、`MO`、`TW`等即可换区

### 操作步骤

***
* 配置Quantumult：

```
1.开启HTTPS解密并信任Quantumult证书
2.模块：TUN + HTTP(Default)
3.添加订阅：
  分流：https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult.conf
  链接阻止：https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult_URL.conf
  服务器：有机场的填，无机场的跳过这行
4.添加服务器ss/ssr/vmess等（有机场的跳过这，没服务器的随缘(^_-)）
5.添加1条分流规则：
  作用：看美区Appstore下载的TikTok的直播（部分账号无直播功能出现）
  HOST-SUFFIX,pstatp.com,PROXY,resolve-on-proxy
6.⭐️TikTok换区操作：修改HTTP复写中，CN(?=&)的替换值为`MO`、`SG`等
7.开启Quantumult（运行模式：自动分流）
8.观看TikTok
```

**超详细步骤：**

1. 打开`圈Quantumult `  
2. `更多 `--)`模块 `--)`TUN+HTTP(Default) `  
3. 开启**HTTPS解密**并**信任**Quantumult证书，iOS13和iOS12操作略有不同：
    * `设置`--)`HTTPS解密`--)开启`HTTPS解密`--)`生成密钥及证书`--)右上角点`保存`--)`允许`安装描述文件--)`关闭`--)前往手机的`设置`，不在Quantumult了--)看到`已下载描述文件`--)`安装`--)输入手机的解锁密码--)`安装`--)`安装`--)前往手机的`设置`--)`通用`--)`关于本机`--)`证书信任设置`--)找到`Quantumult Custom Root Certificate…`点绿它以信任该根证书--)`继续`  
4. 添加**订阅分流**链接：前往`quantumult`：`设置`--)`订阅`--)右上角`加号`--)`分流`--)`链接`处添加网址`https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult.conf` --)`名称`输入`分流`俩字--)`个性化`戳出对勾--)右上角`保存`--)`左划`--)点选`替换`--)`保存`--)`好`  
5. 添加**订阅链接阻止**：`设置`--)`订阅`--)右上角`添加`--)`链接阻止`--)`链接`添加网址`https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult_URL.conf` --)`名称`输入`阻止`俩字--)`包含主机名`戳出对勾--)`保存`--)`左划`--)点选`替换`--)`好`  
6. 不看美区直播的可跳过此步：`设置`--)`分流`--)搜索`pstatp.com`--)戳进去--)将`行为`Direct改为`Proxy`--)开启`远程解析TUN连接`--)右上角`保存`--)`取消`--)左上角`保存`  
7. 添加**服务器**ss/ssr/vmess等 
    * 有机场的：`设置`--)`订阅`--)右上角`加号`--)`服务器`--)粘你的订阅链接--)`保存`  
    * 没有机场的：`设置`--)`服务器`--)右上角`加号/扫二维码`--)填写你的代理
8. 开启**Quantumult**：前往`Quantumult`的`主页`--)右上角开启`Quantumult`--)`Allow`--)`指纹/密码`--)戳最底端中间的`Quantumult图标`选择节点--)TikTok愉快

### 感谢

* [@lhie1](https://github.com/lhie1/Rules/tree/master/Quantumult)
