# clash pro rules简介


规则转自：Loyalsoldier，在此基础上修改添加

本项目生成适用于 [**Clash Premium**](https://github.com/Dreamacro/clash/releases/tag/premium) 的规则集（RULE-SET）。

## 说明

本项目的规则集（RULE-SET）主要来源于项目 [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat) 和 [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)；[`Apple`](https://github.com/Loyalsoldier/clash-rules/blob/release/apple.txt) 和 [`Google`](https://github.com/Loyalsoldier/clash-rules/blob/release/google.txt) 列表里的部分域名来源于项目 [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)；中国大陆 IPv4 地址数据使用 [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)。

本项目的规则集（RULE-SET）只适用于 Clash **Premium** 版本。Clash Premium 相对于普通版，增加了 **TUN 增强模式**，能接管设备所有 TCP 和 UDP 流量，类似 [Surge for Mac](https://nssurge.com) 的增强模式。更多高级特性请看[官方 wiki](https://github.com/Dreamacro/clash/wiki/premium-core-features)。

### Clash 各版本下载地址

- Clash Premium **命令行**版（兼容 Windows、macOS、Linux、OpenWRT 等多种平台）：[https://github.com/Dreamacro/clash/releases/tag/premium](https://github.com/Dreamacro/clash/releases/tag/premium)
- Clash Premium **图形用户界面**版（ClashX Pro，兼容 macOS）：[https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution_groups/public](https://install.appcenter.ms/users/clashx/apps/clashx-pro/distribution_groups/public)
- Clash Premium **图形用户界面**版（Clash for Windows，兼容 Windows、macOS）：[https://github.com/Fndroid/clash_for_windows_pkg/releases](https://github.com/Fndroid/clash_for_windows_pkg/releases)

## 规则文件地址及使用方式

### 在线地址（URL）

### 无法访问 `raw.githubusercontent.com`的解决方法

- 方法一，修改系统hosts文件，添加151.101.108.133 raw.githubusercontent.com (备注，这是我的IP查询出来的，请自行按照自己网络查询) \
  查询解析的IP地址：`https://ipaddress.com/website/raw.githubusercontent.com`  
- 方法二，如果`raw.githubusercontent.com`无法链接，请使用备选链接`cdn.jsdelivr.net` 

### cdn.jsdelivr.net 无法刷新缓存解决方法
- 将 cdn.jsdelivr.net中的cdn改为 purge
- git bash中执行 \
 `curl https://purge.jsdelivr.net/gh/username/reponame@latest/file.*** `
- 浏览器直接访问 \
` https://purge.jsdelivr.net/gh/snapei/clash-pro-rules@release/xxx.txt `


> 以下地址填写在 Clash 配置文件里的 `rule-providers` 里的 `url` 配置项中。

- **直连域名列表 direct.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/direct.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/direct.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/direct.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/direct.txt)
- **代理域名列表 proxy.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/proxy.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/proxy.txt)
- **广告域名列表 reject.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/reject.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/reject.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/reject.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/reject.txt)
- **Apple 域名列表 apple.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/apple.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/apple.txt)
- **iCloud 域名列表 icloud.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/icloud.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/icloud.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/icloud.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/icloud.txt)
- **Google 域名列表 google.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/google.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/google.txt)
- **局域网 IP 及保留 IP 地址列表 lancidr.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/lancidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/lancidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/lancidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/lancidr.txt)
- **中国大陆 IPv4 地址列表 cncidr.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/cncidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/cncidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/cncidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/cncidr.txt)
- **YOUTUBE 域名列表 youtube.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/youtube.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/youtube.txt)
- **NETFLIX 域名列表 netflix.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflix.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflix.txt)
- **NETFLIX IPv4 地址列表 netflixcidr.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflixcidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/netflixcidr.txt)
- **GFWList 域名列表 gfw.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/gfw.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/gfw.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/gfw.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/gfw.txt)
- **GreatFire 域名列表 greatfire.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/greatfire.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/greatfire.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/greatfire.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/greatfire.txt)
- **非中国大陆使用的顶级域名列表 tld-not-cn.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tld-not-cn.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tld-not-cn.txt)
- **Telegram 使用的 IP 地址列表 telegramcidr.txt**：  
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegramcidr.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/telegramcidr.txt)
- **TIKTOK 域名列表 tiktok.txt**：
  - [https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt](https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt)
  - [https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tiktok.txt](https://cdn.jsdelivr.net/gh/snapei/clash-pro-rules@release/tiktok.txt)  
 
### 使用方式

关于 Clash Premium 使用方式，请查看[官方文档](https://github.com/Dreamacro/clash/wiki/premium-core-features) 或 [Lancellc's GitBook](https://lancellc.gitbook.io/clash/)。

要想使用本项目的规则集，只需要在 Clash 配置文件中添加如下 `rule-providers` 和 `rules`。

#### Rule Providers 配置方式

```yaml
rule-providers:
  reject:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/reject.txt"
    path: ./ruleset/reject.yaml
    interval: 86400

  icloud:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/icloud.txt"
    path: ./ruleset/icloud.yaml
    interval: 86400

  apple:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/apple.txt"
    path: ./ruleset/apple.yaml
    interval: 86400

  google:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/google.txt"
    path: ./ruleset/google.yaml
    interval: 86400

  proxy:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/proxy.txt"
    path: ./ruleset/proxy.yaml
    interval: 86400

  direct:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/direct.txt"
    path: ./ruleset/direct.yaml
    interval: 86400

  cncidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/cncidr.txt"
    path: ./ruleset/cncidr.yaml
    interval: 86400

  lancidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/lancidr.txt"
    path: ./ruleset/lancidr.yaml
    interval: 86400

  youtube:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/youtube.txt"
    path: ./ruleset/youtube.yaml
    interval: 86400
    
  netflix:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflix.txt"
    path: ./ruleset/netflix.yaml
    interval: 86400
    
  netflixcidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/netflixcidr.txt"
    path: ./ruleset/netflixcidr.yaml
    interval: 86400

  gfw:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/gfw.txt"
    path: ./ruleset/gfw.yaml
    interval: 86400

  greatfire:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/greatfire.txt"
    path: ./ruleset/greatfire.yaml
    interval: 86400

  tld-not-cn:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tld-not-cn.txt"
    path: ./ruleset/tld-not-cn.yaml
    interval: 86400

  telegramcidr:
    type: http
    behavior: ipcidr
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/telegramcidr.txt"
    path: ./ruleset/telegramcidr.yaml
    interval: 86400

  tiktok:
    type: http
    behavior: domain
    url: "https://raw.githubusercontent.com/snapei/clash-pro-rules/release/tiktok.txt"
    path: ./ruleset/tiktok.yaml
    interval: 86400



```

#### Rules 配置方式

- 以下配置中的 `PROCESS-NAME` 规则类型**只能**在 **ClashX Pro** 中使用，其余版本均不能使用，需要手动删除。
- 如果希望使用 DNS 来解析未命中域名类型规则的域名，而不是直接走代理，请删除 `cncidr` 行尾的 `,no-resolve`。
- 以下配置中，除了 `DIRECT` 和 `REJECT` 是默认存在于 Clash 中的 policy（路由策略/流量处理策略），其余均为自定义 policy，对应配置文件中 `proxies` 或 `proxy-groups` 中的 `name`。如你直接使用下面的 `rules` 规则，则需要在 `proxies` 或 `proxy-groups` 中手动配置一个 `name` 为 `PROXY` 的 policy。
- 如你希望 Apple、iCloud 和 Google 列表中的域名使用代理，则把 policy 由 `DIRECT` 改为 `PROXY`，以此类推，举一反三。

```yaml
rules:
  - PROCESS-NAME,v2ray,DIRECT
  - PROCESS-NAME,Surge%203,DIRECT
  - PROCESS-NAME,ss-local,DIRECT
  - PROCESS-NAME,privoxy,DIRECT
  - PROCESS-NAME,trojan,DIRECT
  - PROCESS-NAME,trojan-go,DIRECT
  - PROCESS-NAME,naive,DIRECT
  - PROCESS-NAME,Thunder,DIRECT
  - PROCESS-NAME,DownloadService,DIRECT
  - PROCESS-NAME,qBittorrent,DIRECT
  - PROCESS-NAME,Transmission,DIRECT
  - PROCESS-NAME,fdm,DIRECT
  - PROCESS-NAME,aria2c,DIRECT
  - PROCESS-NAME,Folx,DIRECT
  - PROCESS-NAME,NetTransport,DIRECT
  - PROCESS-NAME,uTorrent,DIRECT
  - PROCESS-NAME,WebTorrent,DIRECT
  - RULE-SET,lancidr,DIRECT,no-resolve
  - RULE-SET,cncidr,DIRECT,no-resolve
  - RULE-SET,reject,REJECT
  - RULE-SET,icloud,DIRECT
  - RULE-SET,apple,DIRECT
  - RULE-SET,google,GOOGLE
  - RULE-SET,youtube,YOUTUBE
  - RULE-SET,netflix,NETFLIX
  - RULE-SET,netflixcidr,NETFLIX,no-resolve
  - RULE-SET,gfw,PROXY
  - RULE-SET,greatfire,PROXY
  - RULE-SET,tld-not-cn,PROXY
  - RULE-SET,telegramcidr,PROXY,no-resolve
  - RULE-SET,tiktok,PROXY
  - RULE-SET,proxy,PROXY
  - RULE-SET,direct,DIRECT
  - GEOIP,CN,DIRECT
  - MATCH,PROXY
```

## 致谢

- [@Loyalsoldier/clash-rules](https://github.com/Loyalsoldier/clash-rules)
- [@Loyalsoldier/v2ray-rules-dat](https://github.com/Loyalsoldier/v2ray-rules-dat)
- [@v2fly/domain-list-community](https://github.com/v2fly/domain-list-community)
- [@felixonmars/dnsmasq-china-list](https://github.com/felixonmars/dnsmasq-china-list)
- [@17mon/china_ip_list](https://github.com/17mon/china_ip_list)
