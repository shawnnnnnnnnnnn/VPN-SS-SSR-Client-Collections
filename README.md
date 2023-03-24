## SS/SSR 简介

### **介绍**

  SS 的全称是 Shadowsocks，是一种加密的传输方式（一种基于 Socks5 代理方式的网络数据加密传输包）；SS 是目前主流的科学上网方式，是目前最稳定最好用的科学上网工具之一。

  SSR（全称 ShadowsocksR ）是 SS 的修改版，也算是增强版，是在SS 的基础上做了些功能的增加和修改。

  有很多的 SS 客户端，但是仅仅有 SS 客户端还不能翻墙，**还得需要在SS 客户端中添加正常可用的 SS 信息，SS 信息可以自己买 VPS 服务器搭建，也可以买别人搭建好的，也有人搭建了免费共享出来的**。网上卖 SS 信息的非常多非常多（不过跑路的也很多，自己当心），但都不是官方提供，SS 官网并不卖服务。

  还有另外一个代理工具:V2Ray，V2Ray 是一个模块化的代理软件包，它的目标是提供常用的代理软件模块，简化网络代理软件的开发。简单来说，它就是一个模块化代理，可以用来科学上网，支持多平台。

- SS 唯一官网（官网不卖服务）:[https://shadowsocks.org](https://shadowsocks.org/)

- 维基百科详细介绍:https://zh.wikipedia.org/wiki/Shadowsocks

- 原理看这个:http://vc2tea.com/whats-shadowsocks

- SSR 维基百科详细介绍:https://zh.wikipedia.org/wiki/Shadowsocks#ShadowsocksR

- 利用AWS 搭建免费 Shadowsocks:[http://lichendi.com/2016/06/07/shadowsocks/](http://lichendi.com/2016/06/07/利用AWS搭建免费shadowsocks)

- Google Cloud 可以免费拿一台 VPS 试用一年:http://51.ruyo.net/p/2144.html

- V2Ray 官网:[https://www.v2ray.com](https://www.v2ray.com/)

- 记录一下 SS 的前世今生，以及一个简单的教程总结

- - https://github.com/JadaGates/ShadowsocksBio

- 免费 SS 账号分享（能不能用，能用多久我就不确定了）

- - [https://free-ss.site](https://free-ss.site/)
  - [https://ss.freess.org](https://t.me/SSRSUB)
  - [https://doub.io/sszhfx](https://t.me/SSRSUB)
  - [https://us.ishadowx.net](https://us.ishadowx.net/)
  - https://tool.ssrshare.us/tool/free_ssr

### 区别

  VPN 也是传输方式，VPN 默认是全局的（也有少数是可以分流的），开启后所有App 软件都会走代理，而且 VPN 的特征值太明显，目前已被 G·F·W 干扰。

  SS 是和VPN 完全不同类型的东西，SS 的客户端是智能代理智能分流，根据规则自动判断，只有被墙了的才会走代理（自己也可以设置代理域名和 IP ），不需要代理的走直连，这样就可以7x24的开启 SS，国内和没被墙的走直连不走代理，国内国外两不误。SS 比 VPN 好用太多了！ 

> *相比传统的 VPN (IKE, IPSec, PPTP…)，Shadowsocks 协议具有更好的灵活性和隐蔽性，且搭建相对简单，因此可以拥有相对传统VPN更快的速度和更高的稳定性；另对比 V2Ray 这种科学上网的集合体，Shadowsocks在服务端更加轻量，单一协议完善程度更高；在移动端有更丰富的客户端选择，兼容性和灵活性更优。 (此段摘自:*https://medium.com/@unbiniliumm/95187ef07ced*)*

### **耗电**

*为什么使用了代理应用后在电量统计中显示耗电很多？*

这是移动操作系统的一个特殊机制，Surge、Quantumult、Shadowrocket等等所有的 SS 客户端开启后会接管全局的（几乎）所有通信，所以所有的网络方面电量消耗都会被算在 SS 客户端头上，实际使用中不会感到 SS 客户端对电量有明显影响，「设置-电池」中看到它的电池用量，绝大部分都是网络所消耗的电量，并不是 SS 客户端消耗的电量，SS 客户端就是背锅侠。

### 客户端

##### 推荐客户端

- iOS: Surge 4, Quantumult X, Quantumult, Loon, Shadowrocket

- Android: Clash for Android, Surfboard

- macOS: Surge for Mac, ClashX, Clash for Windows

- Windows: Clash for Windows

- Linux: Clash

  *(下方有下载地址)*

##### iOS 客户端 (全区可下载,包括中区)

- [Loon](https://testflight.apple.com/join/23LA2tmX) (支持Surge 3的 RULESET 规则)
- [Outline](https://apps.apple.com/cn/app/outline-app/id1356177741) (支持SS)
- [Kitsunebi](https://testflight.apple.com/join/IdFRwmNy) (支持SS/Vmess)
- [Potatso Lite](https://testflight.apple.com/join/NkF46PRd)
- [A.BIG.T IV](https://testflight.apple.com/join/3aArQFMQ)
- [BananaNet](https://testflight.apple.com/join/v5x8B81b)
- [NetShuttle](https://testflight.apple.com/join/742YC03J)

##### iOS 客户端 (仅国区下架,其他区可下载)

- [Surge 4](https://apps.apple.com/us/app/id1442620678) 免费 + 内购 $49.99 (支持SS/Snell/Vmess) [官网购买](https://nssurge.com/buy_now) [教程](https://zhuangzhuang.cf/tags/#Surge)
- [Quantumult X](https://apps.apple.com/us/app/quantumult-x/id1443988620) $7.99 (支持SS/SSR/Vmess) [教程](https://www.notion.so/kopshawn/Quantumult-X-1d32ddc6e61c4892ad2ec5ea47f00917) [视频教程](https://youtu.be/laqB-SMHO1w)
- [Quantumult](https://apps.apple.com/us/app/quantumult/id1252015438) $4.99 (也叫:圈, 支持SS/SSR/Vmess) [教程](https://github.com/JasonLee-Go/Quantumult/wiki/Quantumult-Unofficial-Manual)
- [Quantumult Bundle](https://apps.apple.com/us/app-bundle/quantumult-x-upgrade/id1482985563) $9.99 (Bundle包,包括Quantumult X和Quantumult)
- [Loon](https://apps.apple.com/us/app/loon/id1373567447) $2.99 (支持SS/SSR/Vmess) [视频教程](https://youtu.be/v3gHdE5UEw8)
- [Shadowrocket](https://apps.apple.com/us/app/shadowrocket/id932747118) $2.99 (也叫:小火箭, 支持SS/SSR/Vmess/Trojan/Snell/Lua) [教程](http://laob.me/2300)
- [Pharos Pro](https://apps.apple.com/us/app/pharos-pro/id1456610173) $1.99 (支持SS/SSR/Vmess/Trojan)
- [Kitsunebi](https://apps.apple.com/us/app/kitsunebi-proxy-utility/id1446584073) $4.99 (支持SS/Vmess)
- [Pepi](https://apps.apple.com/us/app/pepi/id1283082051) $1.99
- [Potatso 2](https://apps.apple.com/us/app/id1162704202) $2.99
- [Potatso Lite](https://apps.apple.com/us/app/id1239860606) Free
- [Ranger NetworkTool](https://apps.apple.com/us/app/ranger-networktool/id1330474376) $1.99
- [Wingy](https://apps.apple.com/us/app/wingy-http-s-socks5-proxy-utility/id1178584911) $0.99
- [ShadowPocket](https://apps.apple.com/us/app/shadowpocket/id1354988493) $1.99
- [AnyFlow](https://apps.apple.com/us/app/anyflow-a-super-cool-network-tool/id1176894911) $4.99
- [Shadowfish](https://apps.apple.com/us/app/shadowfish/id1220680757) $0.99
- [Alice](https://apps.apple.com/us/app/alice-network-proxy-utility/id1135320992) $1.99
- [Bedrock](https://apps.apple.com/us/app/bedrock/id1362340186) $3.99
- [Mume VPN](https://apps.apple.com/us/app/mume-vpn/id1144787928) $0.99
- [‎寒梅 · Mume Red](https://apps.apple.com/us/app/id1453275281) Free
- [A.BIG.T](https://apps.apple.com/us/app/surfing-advanced-proxy/id1051326718) Free
- [‎Skarp](https://apps.apple.com/us/app/skarp/id1300469689) Free
- [FastSocks](https://apps.apple.com/us/app/id1388244800) Free
- [ShadowLink](https://apps.apple.com/us/app/shadowlink-shadowsocks-tool/id1439686518) Free
- [NetShuttle](https://apps.apple.com/us/app/netshuttle-shadowsocksr-tool/id982708939) Free
- [Oriole](https://apps.apple.com/us/app/id1245170216) Free
- [Brook](https://apps.apple.com/us/app/brook-brook-shadowsocks-vpn-proxy/id1216002642) Free
- [Fugu2](https://apps.apple.com/us/app/fugu-2/id1215255916) Free

##### macOS 客户端

- [Surge for Mac](http://nssurge.com/) $49.99/$69.99/$99.99 (支持SS/Snell/Vmess)
- [ClashX](https://github.com/yichengchen/clashX/releases) Clash的Mac图形客户端 (支持SS/Snell/Vmess) [教程](https://docs.nameless13.com/clashr)
- [ClashX Pro](https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution_groups/public) 支持开启”增强模式的”ClashX
- [Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases) Clash的Windows/macOS图形客户端,简称:CFW (支持SS/Snell/Vmess/Trojan) [教程](https://docs.cfw.lbyczf.com/) [视频教程](https://youtu.be/21prqwxBg94)
- [ClashXR](https://github.com/WhoJave/clashX/releases) Clash客户端(支持SS/Snell/Vmess/SSR) [教程](https://docs.nameless13.com/clashr)
- [Clashy](https://github.com/SpongeNobody/Clashy/releases) Windows /Mac/Ubuntu适用的Clash客户端
- [Clash 内核](https://github.com/Dreamacro/clash/releases) 一个Go语言开发的多平台代理客户端 (支持SS/Snell/Vmess/Trojan)
- [ShadowClash](https://github.com/TheWanderingCoel/ShadowClash)
- [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases) (支持SS/SSR/Snell/Vmess/Trojan)
- [Mellow](https://github.com/eycorsican/Mellow/releases) (支持SS/Vmess)
- [ShadowsocksX](https://github.com/shadowsocks/shadowsocks-iOS/releases)
- [ShadowsocksX-NG](https://github.com/shadowsocks/ShadowsocksX-NG/releases) (支持SS)
- [ShadowsocksX-NG-R8](https://github.com/qinyuhang/ShadowsocksX-NG-R/releases) (支持SS/SSR)
- [ShadowsocksX-NG-R8](https://github.com/paradiseduo/ShadowsocksX-NG-R8/releases)
- [ShadowsocksX-NG-R](https://github.com/leadscloud/ShadowsocksX-NG-R/releases)
- [ShadowsocksX-NG-R](https://github.com/wzdnzd/ShadowsocksX-NG-R/releases)
- [electron-ssr](https://github.com/qingshuisiyuan/electron-ssr-backup/releases)
- [Outline](https://apps.apple.com/cn/app/outline-secure-internet-access/id1356178125) Free
- [Reborn](https://github.com/langyanduan/Reborn/releases)
- [Shuttle](https://github.com/sipt/shuttle/releases)
- [SsrConnectPro](https://apps.apple.com/cn/app/ssrconnectpro/id1376924741) ¥3.00
- [GoAgentX](https://pan.lanzou.com/i0dskef)
- [非官方GoAgentX](https://github.com/mithril-global/GoAgentX/releases)
- [Flora](https://github.com/huacnlee/flora-kit/releases)
- [SpechtLite](https://github.com/zhuhaow/SpechtLite/releases)
- [Buff](https://www.plutox.top/)

##### Windows 客户端

- [Clash for Windows](https://github.com/Fndroid/clash_for_windows_pkg/releases) Clash的Windows/macOS图形客户端,简称:CFW (支持SS/Snell/Vmess/Trojan) [教程](https://docs.cfw.lbyczf.com/) [视频教程](https://youtu.be/21prqwxBg94)
- [Clash for Windows 中文版](https://github.com/kallydev/clash_for_windows_pkg_zh-cn/releases)
- [ClashR for windows](https://t.me/yxbjx/411954) Clash客户端(支持SS/Snell/Vmess/SSR) [教程](https://docs.nameless13.com/clashr)
- [Clash 内核](https://github.com/Dreamacro/clash/releases) 一个Go语言开发的多平台代理客户端 (支持SS/Snell/Vmess/Trojan)
- [ClashR 内核](https://github.com/BROBIRD/clash/releases) 支持SS/Snell/Vmess/SSR的Clash客户端 [教程](https://docs.nameless13.com/clashr)
- [ClashR 内核](https://github.com/frainzy1477/clashrdev/releases) 支持SS/Snell/Vmess/SSR的Clash客户端 [教程](https://docs.nameless13.com/clashr)
- [Clashy](https://github.com/SpongeNobody/Clashy/releases) Windows /Mac/Ubuntu适用的Clash客户端
- [ClashCS](https://github.com/Krazysdaki/ClashCS-Beta/releases) A Beta version Clash GUI built by C#
- [Clash-Web-Bat](https://github.com/pcysanji/Clash-Web-Bat/releases) [文档](https://github.com/pcysanji/Clash-Web-Bat/blob/master/README.md)
- [ClashCMD](https://github.com/tindy2013/clashcmd/releases) [文档](https://github.com/tindy2013/clashcmd/blob/master/README.md)
- [ClashWeb](https://github.com/lzdnico/ClashWeb/releases) [文档](https://github.com/lzdnico/ClashWeb/blob/master/README.md)
- [ShadowClash](https://github.com/TheWanderingCoel/ShadowClash)
- [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases) (支持SS/SSR/Snell/Vmess/Trojan)
- [Netch](https://github.com/netchx/Netch/releases) (支持SS/SSR/Vmess)
- [Mellow](https://github.com/eycorsican/Mellow/releases) (支持SS/Vmess)
- [Shadowsocks](https://github.com/shadowsocks/shadowsocks-windows/releases) (简称:SS)
- [simple-obfs](https://github.com/shadowsocks/simple-obfs/releases) (SS的插件)
- [Shadowsocks 2.3.1](https://github.com/shadowsocks/shadowsocks-windows/releases/tag/2.3.1)（XP 系统可用）
- [ShadowsocksR](https://github.com/shadowsocksr-backup/shadowsocksr-csharp/releases) (简称:SSR)
- [ShadowsocksR](https://github.com/HMBSbige/ShadowsocksR-Windows/releases) (HMBSbige 修改版)
- [ShadowsocksR 4.7.0](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/ShadowsocksR_4.7.0_Windows.7z) (@breakwa11 破娃最后一版)
- [ShadowsocksR](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/ShadowsocksR_rixCloud_Windows.7z) (SSR,rixCloud, Inc. 修改版)
- [ShadowsocksRR](https://github.com/shadowsocksrr/shadowsocksr-csharp/releases) (简称:SSRR)
- [SSRR](https://github.com/SoDa-GitHub/SSRR-Windows/releases)
- [ShadowsocksD](https://github.com/SoDa-GitHub/SSD-Windows/releases) (简称:SSD)
- [electron-ssr](https://github.com/qingshuisiyuan/electron-ssr-backup/releases)
- [SScap](https://sourceforge.net/projects/sscap)
- [SSTap](https://github.com/mayunbaba2/SSTap-beta-setup)
- [SocksCap](https://www.sockscap64.com/sockscap-64-free-download)
- [Outline](https://raw.githubusercontent.com/Jigsaw-Code/outline-releases/master/manager/Outline-Manager.exe)
- [x2tap](https://github.com/hacking001/x2tap/releases)
- [Shuttle](https://github.com/sipt/shuttle/releases)
- [flora](https://github.com/huacnlee/flora-kit/releases)
- [kcptun](https://github.com/shadowsocks/kcptun/releases)

##### Android 客户端

- [Clash for Android](https://github.com/Kr328/ClashForAndroid/releases) Clash的Android图形客户端 (支持SS/Snell/Vmess) [教程](https://wiki.kache.moe/2019/12/10/Andoird-Clash for Android)
- [Clash for Android Google Play](https://play.google.com/store/apps/details?id=com.github.kr328.clash) Clash的Android图形客户端 (支持SS/Snell/Vmess)
- [ClashR for Android](https://github.com/BROBIRD/ClashForAndroid/releases) Clash的Android图形客户端 (支持SS/Snell/Vmess/SSR) [教程](https://docs.nameless13.com/clashr)
- [ClashA](https://github.com/ccg2018/ClashA/releases) Clash的Android图形客户端 (支持SS/Snell/Vmess)
- [ClashAR](https://github.com/WhoJave/ClashA/releases) Clash客户端(支持SS/Snell/Vmess/SSR)
- [Surfboard](https://manual.getsurfboard.com/cn/introduction)（Surfboard支持导入Surge配置,支持SS/Vmess）
- [Surfboard Google Play](https://play.google.com/store/apps/details?id=com.getsurfboard)
- [Pharos](https://github.com/PharosVip/Pharos-Android-Test/releases) (支持SS/SSR/Vmess/Trojan)
- [Kitsunebi](https://github.com/eycorsican/kitsunebi-android/releases)
- [Kitsunebi Google Play](https://play.google.com/store/apps/details?id=fun.kitsunebi.kitsunebi4android)
- [SSRRAY](https://github.com/xxf098/shadowsocksr-v2ray-android/releases) A ShadowsocksR and V2Ray Client for Android
- [Shadowsocks 影梭](https://github.com/shadowsocks/shadowsocks-android/releases)
- [Shadowsocks 影梭 Google Play](https://play.google.com/store/apps/details?id=com.github.shadowsocks)
- [Shadowsocks 影梭 Google Play Beta 版](https://play.google.com/apps/testing/com.github.shadowsocks)
- [Simple Obfuscation](https://github.com/shadowsocks/simple-obfs-android/releases) (影梭的插件)
- [Simple Obfuscation Google Play](https://play.google.com/store/apps/details?id=com.github.shadowsocks.plugin.obfs_local) (影梭的插件)
- [ShadowsocksD](https://github.com/TheCGDF/SSD-Android/releases) (简称:SSD)
- [ShadowsocksR](https://github.com/shadowsocksr-backup/shadowsocksr-android/releases) (简称:SSR)
- [ShadowsocksR 3.4.0.6](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/ShadowsocksR_3.4.0.6_Android.zip) (@breakwa11 破娃最后一版)
- [ShadowsocksR](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/ShadowsocksR_rixCloud_Android.zip) (SSR,rixCloud, Inc. 修改版)
- [ShadowsocksR](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/Maying_3.4.0.8.3.zip) (SSR,魅影修改版)
- [ShadowsocksRR](https://github.com/shadowsocksrr/shadowsocksr-android/releases) (简称:SSRR)
- [shadowsocksRb](https://github.com/shadowsocksRb/shadowsocksRb-android/releases)
- [Maying](https://github.com/congcong0806/congcong0806.github.io/raw/master/files/Maying_1.1.6.zip) (ShadowsocksRR, Java修改版)
- [ShadowIce Google Play](https://play.google.com/store/apps/details?id=com.github.shadowice)
- [Outline](https://play.google.com/store/apps/details?id=org.outline.android.client)
- [NetPatch](https://play.google.com/store/apps/details?id=co.netpatch.firewall)
- [Postern](https://play.google.com/store/apps/details?id=com.tunnelworkshop.postern)（Postern 支持导入 Surge 配置）
- [BifrostV](https://play.google.com/store/apps/details?id=com.github.dawndiy.bifrostv)
- [kcptun-android](https://github.com/shadowsocks/kcptun-android/releases)

##### Linux 客户端

- [Clashy](https://github.com/SpongeNobody/Clashy/releases) Windows /Mac/Ubuntu适用的Clash客户端
- [Clash 内核](https://github.com/Dreamacro/clash/releases) 一个Go语言开发的多平台代理客户端 (支持SS/Snell/Vmess/Trojan)
- [ShadowClash](https://github.com/TheWanderingCoel/ShadowClash)
- [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases) (支持SS/SSR/Snell/Vmess/Trojan)
- [Mellow](https://github.com/eycorsican/Mellow/releases) (支持SS/Vmess)
- [electron-ssr](https://github.com/qingshuisiyuan/electron-ssr-backup/releases)
- [Shadowsocks-qt5](https://github.com/shadowsocks/shadowsocks-qt5)
- [ShadowsocksR](https://github.com/ssrbackup/shadowsocksr) (简称:SSR)
- [Outline](https://raw.githubusercontent.com/Jigsaw-Code/outline-releases/master/manager/Outline-Manager.AppImage)
- [Avege](https://github.com/avege/avege)
- [flora](https://github.com/huacnlee/flora-kit)
- [Shuttle](https://github.com/sipt/shuttle)
- [kcptun](https://github.com/shadowsocks/kcptun/releases)

##### 路由器

- [OpenClash](https://github.com/vernesong/OpenClash/wiki)
- [Clash-Merlin](https://github.com/KOP-XIAO/Clash-Merlin/wiki)
- [Koolshare OpenWrt/LED](https://koolclash.js.org/)
- [KoolClash](https://github.com/SukkaW/Koolshare-Clash/releases)
- [fancyss](https://github.com/hq450/fancyss)
- [Clash for OpenWrt](https://github.com/frainzy1477/clash/releases)
- [ClashR for OpenWrt](https://github.com/frainzy1477/clashr/releases)
- [Luci For Clash - OpenWrt](https://github.com/frainzy1477/luci-app-clash/releases)
- [OpenWRT-Shadowsocks](https://github.com/shadowsocks/openwrt-shadowsocks)
- [Padavan](https://www.right.com.cn/forum/thread-161324-1-1.html)

##### TV

- [Shadowsocks 影梭](https://github.com/shadowsocks/shadowsocks-android/releases) (选择shadowsocks-tv)

##### V2Ray 客户端

- iOS

- - Surge 4, Quantumult X, Quantumult, Shadowrocket, Pharos Pro, Kitsunebi, Loon ↑
  - [i2Ray](https://apps.apple.com/us/app/id1445270056) $3.99

- Windows

- - Clash for Windows ↑
  - [v2rayN](https://github.com/2dust/v2rayN/releases)
  - [V2RayW](https://github.com/Cenmrev/V2RayW/releases)
  - [V2RayS](https://github.com/Shinlor/V2RayS/releases)
  - [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)

- macOS

- - ClashX ↑
  - [V2RayX](https://github.com/Cenmrev/V2RayX/releases)
  - [V2rayU](https://github.com/yanue/V2rayU/releases)
  - [V2RayC](https://github.com/gssdromen/V2RayC)
  - [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)

- Linux

- - [Qv2ray](https://github.com/Qv2ray/Qv2ray/releases)

- Android

- - Clash for Android ↑
  - [v2rayNG](https://github.com/2dust/v2rayNG/releases)
  - [v2rayNG Google Play](https://play.google.com/store/apps/details?id=com.v2ray.ang)

##### Trojan 客户端

- iOS: Surge 4, Shadowrocket, Pharos Pro ↑
- Android: [igniter](https://github.com/trojan-gfw/igniter/releases/tag/v0.1.0-pre-alpha16)
- Windows: [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases)
- macOS: Surge Mac, [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases) [TrojanX](https://github.com/JimLee1996/TrojanX/releases)
- Linux: [Trojan-Qt5](https://github.com/TheWanderingCoel/Trojan-Qt5/releases)

### Telegram 客户端 Proxy 代理设置

https://telegra.ph/Telegram-Proxy-02-15

### **其他**

   iOS 设备上使用 SS 客户端也会显示VPN 图标:是因为使用了 iOS 系统的 VPN Network Extension 接口（以及 NEPacketTunnelProvider 和 NWUDPSession 组件），iOS 9 才开放的此接口，这些新接口让我们可以制作出私密协议的VPN产品，苹果官方称之为 Enterprise VPN。正是因为 iOS 9 之后开放了这个接口和组件才能有今天iOS 上的各式各样的 SS 客户端。

   官方文档:https://developer.apple.com/documentation/networkextension 

   SS/SSR 客户端，在连接SS/SSR 服务器的同时也会在本机开启SOCKS5 和HTTP 连接，用于本机软件和同一局域网内的其他设备连接，所以SS/SSR 信息部分必须和SS/SSR 服务器信息一致。

   本地开启的SOCKS5 与SS/SSR 信息无关的，本机的软件和同一局域网内的其他设备只需要连接此台机器就行了，IP和端口也必须和SS/SSR 客户端上开启的信息一致。

   本机的软件和同一局域网内的其他设备通过SOCKS5 连接到此台机器的SS/SSR 客户端，SS/SSR 客户端再连接到SS/SSR 服务器。

   引用一句 clowwindy 的话:

> *往往不需要政府造墙，网民也会自发造墙*


[感谢TG](https://t.me/LDList/2604)
