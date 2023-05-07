## 官方原版

https://github.com/openwrt/openwrt



## 二次开发

### Lean 版

* https://github.com/coolsnowwolf/lede

### Lienol 版

* https://github.com/Lienol/openwrt



## N次开发

### 基于Lean版编译

> 整合了常用插件

* sirpdboy https://github.com/sirpdboy/openwrt
* firker https://www.right.com.cn/forum/thread-1811791-1-1.html
* lusty https://www.right.com.cn/forum/thread-7667094-1-1.html
* Myan's https://www.right.com.cn/forum/thread-4062018-1-1.html
* jinjin https://www.right.com.cn/forum/thread-4051663-1-1.html
* xuanwumen https://www.right.com.cn/forum/thread-4091453-1-1.html
* zgxwc https://www.right.com.cn/forum/thread-3705778-1-1.html



## 分流规则



### 我的模板

* https://raw.githubusercontent.com/changxiaokang/OpenWrt/main/ProxyGroups/rule/Area_Media_NoAutoPlus.ini



### 节点分类

```ini
# 自动选择
custom_proxy_group=🇭🇰 香港节点`url-test`(香港|HK|Hong Kong|Hongkong)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇨🇳 台湾节点`url-test`(台湾|TW|Taiwan)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇰🇷 韩国节点`url-test`(韩国|KR|Korea|KOR)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇯🇵 日本节点`url-test`(日本|JP|Japan)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇺🇲 美国节点`url-test`(美国|US|United States)`http://www.gstatic.com/generate_204`300,,100
custom_proxy_group=🇸🇬 狮城节点`url-test`(狮城|新加坡|SG|Singapore)`http://www.gstatic.com/generate_204`300,,100

# 手动选择
custom_proxy_group=🇪🇺 欧洲国家`select`(英国|UK|法国|FR|德国|DE|意大利|IT|卢森堡|LU|俄罗斯|RU|乌克兰|UA|摩尔多瓦|MD)
custom_proxy_group=🌍 亚洲国家`select`(越南|VN|印度|IN|泰国|TH|缅甸|MM|迪拜|AE|柬埔寨|KH|菲律宾|PH|土耳其|TR|乌兹别克斯坦|UZ)
custom_proxy_group=🌍 美洲国家`select`(智利|CL|巴西|BR|阿根廷|AR|墨西哥|MX|哥伦比亚|CO|玻利维亚|BO|委内瑞拉|VE)
custom_proxy_group=🇦🇺 大洋洲国家`select`(澳大利亚|AU|新西兰|NZ)
```



### 规则整理

```ini
# 国外媒体
ruleset=📹 YouTube,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/YouTube.list
ruleset=🎥 Netflix,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Netflix.list
ruleset=🎥 Netflix,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/NetflixIP.list
ruleset=📺 Bahamut,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Bahamut.list
ruleset=😍 Pornhub,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Pornhub.list
ruleset=🎵 Spotify,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Spotify.list
ruleset=📺 Twitch,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Twitch.list

# 社交应用
ruleset=🕊 Twitter,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Twitter.list
ruleset=☎ Telegram,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Telegram.list
ruleset=📷 Instagram,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Instagram.list
ruleset=⚙️ TikTok,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/TikTok.list
ruleset=🤙 Line,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Line.list

# 人工智能
ruleset=🧠 OpenAI,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/OpenAi.list

# 游戏平台
ruleset=🎮 Epic,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Epic.list
ruleset=🎮 Sony,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Sony.list
ruleset=🎮 Origin,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Origin.list
ruleset=🎮 Steam,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Steam.list
ruleset=🕹 Nintendo,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Nintendo.list

# 国内媒体
ruleset=📺 Iqiyi,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Iqiyi.list
ruleset=📺 Youku,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Youku.list
ruleset=📺 Bilibili,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/Bilibili.list

# 杂七杂八
ruleset=🍎 Apple,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Apple.list
ruleset=📢 GoogleFCM,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Ruleset/GoogleFCM.list
ruleset=Ⓜ️ Microsoft,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Microsoft.list
ruleset=☁ OneDrive,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/OneDrive.list

ruleset=🐟 漏网之鱼,[]FINAL
ruleset=🛑 广告拦截,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanAD.list
ruleset=🍃 应用净化,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/BanProgramAD.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/GoogleCN.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaIp.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/LocalAreaNetwork.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/ChinaCompanyIp.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/Download.list
ruleset=🎯 全球直连,https://raw.githubusercontent.com/ACL4SSR/ACL4SSR/master/Clash/UnBan.list
ruleset=🎯 全球直连,[]GEOIP,LAN
ruleset=🎯 全球直连,[]GEOIP,CN
```



###  参考资料

* https://github.com/ACL4SSR/ACL4SSR/tree/master/Clash/Ruleset
