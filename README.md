# 🌟 Quantumult看TikTok视频+直播+无水印下载 #

### 支持功能:

***

- [x] TikTok换区

- [x] 看TikTok视频

- [x] 看TikTok直播

- [x] 在TikTok内直接下载无水印视频

### 准备工作:  

***

* ✅ 自备Quantumult

* ✅ 自备proxy

### 操作步骤:

***

1. 打开`圈Quantumult `  

2. `更多 `--)`模块 `--)`TUN+HTTP(Loopback) `  
3. `设置`--)`HTTPS解密`--)开启`HTTPS解密`--)`生成密钥及证书`--)右上角点`保存`--)`允许`安装描述文件--)右上角点`安装`--)输入手机的解锁密码--)右上角点`安装`--)`安装`--)前往手机的`设置`--)`通用`--)`关于本机`--)`证书信任设置`--)找到`Quantumult Custom Root Certificate…`点绿它以信任该根证书--)`继续`  
4. 前往`圈quantumult`：`设置`--)`订阅`--)右上角`加号`--)`分流`--)`链接`处添加网址`https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult.conf` --)`名称`输入`分流`俩字--)`个性化`戳出对勾--)右上角`保存`--)`左划`--)点选`替换`--)`保存`--)`好`  
5. `设置`--)`订阅`--)右上角`添加`--)`链接阻止`--)`链接`添加网址`https://raw.githubusercontent.com/lhie1/Rules/master/Quantumult/Quantumult_URL.conf` --)`名称`输入`阻止`俩字--)`包含主机名`戳出对勾--)`保存`--)`左划`--)点选`替换`--)`好`  
6. `设置`--)`HTTP复写`--)右上角`+`--)`命令`那选`302`--)`匹配`填写`(?<=&watermark=)1&` --) `替换`填写`&` --)`好` --) 右上角`好` --) 右上角加号`+` --) `命令`307 --) `匹配` `(?<=&carrier_region=|&sys_region=)CN(?=.*)` --) `替换`改为你想看的国家/地区简写 --) `好`  
7. 找到以下7条--)逐条`左划`--)`删除这7条`：  
```  (?<=aweme\/v1\/)playwm url 302 play
(?<=&app_version=)([0-9]).([0-9]).([0-9])(?=.*) url 307 2.4.1
(?<=&?version_code=)([0-9]).([0-9]).([0-9]) url 307 2.4.1
(?<=&app_version=)4.4.0(?=.*) url 307 2.4.1
(?<=&?version_code=)4.4.0 url 307 2.4.1
(?<=&carrier_region=)CN(?=.*) url 307 JP
(?<=&sys_region=)CN(?=.*) url 307 JP
```
8. 左上角`保存`  
9. `设置`--)`分流`--)搜索`pstatp.com`--)戳进去--)将`行为`Direct改为Proxy--)开启`远程解析TUN连接`--)右上角`保存`--)`取消`--)左上角`保存`  
10. 添加你的ss/ssr/http/socks/vmess  
    * 有机场的：`设置`--)`订阅`--)右上角`加号`--)`服务器`--)粘你的订阅链接--)`保存`  
    * 没有机场的：`设置`--)`服务器`--)右上角`加号/扫二维码`--)填写你的代理
        * [或从这获取免费的socks5代理](https://github.com/cyubuchen/ProxySpider_spys)
        * 我的小水管，仅供临时测试TikTok使用，随时挂😏
            * `shadowsocks for TikTok test (2019.03.25-2019.06.15)`
            * `address:cyubuchen.ga`
            * `port:543`
            * `password:cyubuchen`
            * `method:aes-256-cfb`
11. 前往`quantumult`的`主页`--)右上角开启`圈`--)`Allow`--)`指纹/密码`--)戳最底端中间的`小圈图标`以选择你的节点--)抖音愉快