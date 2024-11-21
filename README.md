<div align="center">
<h1>adghRuleShura23</h1>
  <p>
    广告过滤规则订阅器，整合不同来源的规则，帮助你快速构建属于自己的规则集
    adghRuleShura23规则列表具有拦截广告、跟踪器、屏蔽危险钓鱼网站、禁用pcdn、GitHub和steam商店加速的功能，能屏蔽番茄小说软件广告
  </p>
<!-- Badges -->
<p>
  <img src="https://img.shields.io/github/last-commit/fordes123/ad-filters-subscriber?style=flat-square" alt="last update" />
  <img src="https://img.shields.io/github/forks/fordes123/ad-filters-subscriber?style=flat-square" alt="forks" />
  <img src="https://img.shields.io/github/stars/fordes123/ad-filters-subscriber?style=flat-square" alt="stars" />
  <img src="https://img.shields.io/github/issues/fordes123/ad-filters-subscriber?style=flat-square" alt="open issues" />
  <img src="https://img.shields.io/github/license/fordes123/ad-filters-subscriber?style=flat-square" alt="license" />
</p>

<h4>
    <a href="#a">项目说明</a>
  <span> · </span>
    <a href="#b">快速开始</a>
  <span> · </span>
    <a href="#c">规则订阅</a>
  <span> · </span>
    <a href="#d">问题反馈</a>
  </h4>
</div>


[English](./README_en.md) | 中文
<h2 id="a">📔 项目说明</h2>

本项目旨在聚合不同来源、不同格式的广告过滤规则，自由的进行转换和整合。
> ⚠️ 新版不再兼容原配置格式，迁移前务必注意
#### 支持的规则格式
- [x] easylist
- [x] dnsmasq
- [x] clash
- [x] smartdns
- [x] hosts

#### 注意事项
1. 仅支持基本规则转换，即域名、通配域名构成的规则，对形如 `||example.org^$popup` 等规则无法转换(合并、去重不受影响) 
2. 接受不可避免的缩限，如 `||example.org^` 将拦截 example.org 及其所有子域，但将其转换为 hosts 格式时，将无法匹配子域名。
3. 规则有效性检测基于域名解析，因此仅支持基本规则。
<h2 id="c">🎯 规则订阅</h2>
**⚠ 本仓库提供规则订阅，我们更推荐 fork 本项目自行构建规则集.**

广告过滤规则demonicAsura链接：(https://raw.githubusercontent.com/Shura23/adghRuleShura23/refs/heads/v2/rule/easylist.txt) </br>
推荐使用国内加速链接：https://mirror.ghproxy.com/https://raw.githubusercontent.com/Shura23/adghRuleShura23/refs/heads/v2/rule/easylist.txt </br>

### 本项目使用的上游规则列表
| Name                                                                                                        | URL                                                                                                                                           |
| ----------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------- |
| AdGuard DNS filter                                                                                          | https://adguardteam.github.io/AdGuardSDNSFilter/Filters/filter.txt                                                                            |
| AdGuard MobileFilter                                                                                        | https://raw.githubusercontent.com/AdguardTeam/AdguardFilters/master/MobileFilter/sections/specific_app.txt                                    |
| AdAway Default Blocklist                                                                                    | https://adaway.org/hosts.txt                                                                                                                  |
| Anti-AD                                                                                                     |https://raw.githubusercontent.com/privacy-protection-tools/anti-AD/master/anti-ad-easylist.txt
|superbigsteam                                                                                                |https://github.com/superbigsteam/adguardhomeguiz/blob/main/rule/dns.txt  
|冷莫trli AdHosts-pro（For ad-adguardhome）                                                                   |https://github.com/Potterli20/file/releases/download/ad-hosts-pro/ad-adguardhome.txt 
|5whys-min                                                                                                    |https://raw.githubusercontent.com/5whys-adblock/AdGuardHome-rules/main/rules/output_min.txt
|Scam Blocklist by DurableNapkin                                                                              |https://adguardteam.github.io/HostlistsRegistry/assets/filter_10.txt
|ShadowWhisperer's Malware List                                                                               |https://adguardteam.github.io/HostlistsRegistry/assets/filter_42.txt
|someonewhocares                                                                                              |https://someonewhocares.org/hosts/zero/hosts
|1hosts pro                                                                                                   |https://o0.pages.dev/Pro/adblock.txt
|The Block List Project (Tracking)                                                                            |https://blocklistproject.github.io/Lists/alt-version/tracking-nl.txt
|The Block List Project (Ads)                                                                                 |https://blocklistproject.github.io/Lists/alt-version/ads-nl.txt
|Phishing.army                                                                                                |https://phishing.army/download/phishing_army_blocklist.txt
|stopforumspam (Toxic Domains)                                                                                |https://www.stopforumspam.com/downloads/toxic_domains_whole.txt
|The Block List Project (Abuse)                                                                               |https://blocklistproject.github.io/Lists/alt-version/abuse-nl.txt
|bongochong (CPBL Full)                                                                                       |https://raw.githubusercontent.com/bongochong/CombinedPrivacyBlockLists/master/NoFormatting/cpbl-wildcard-blacklist.txt
|developerdan (Tracking Aggressive)                                                                           |https://www.github.developerdan.com/hosts/lists/tracking-aggressive-extended.txt 
|Hagezi Badware Hoster blocking                                                                               |https://gitlab.com/hagezi/mirror/-/raw/main/dns-blocklists/adblock/hoster.txt
|HaGeZi's Fake DNS Blocklist                                                                                  |https://raw.githubusercontent.com/hagezi/dns-blocklists/main/adblock/fake.txt
|Hagezi  ULTIMATE                                                                                             |https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/ultimate.txt
|Ad filter list by Disconnect                                                                                 |https://s3.amazonaws.com/lists.disconnect.me/simple_ad.txt
|Malvertising list by Disconnect                                                                              |https://s3.amazonaws.com/lists.disconnect.me/simple_malvertising.txt
|neodevhost                                                                                                   |https://raw.githubusercontent.com/neodevpro/neodevhost/master/adblocker
|banad jiekouAD                                                                                               |https://raw.githubusercontent.com/damengzhu/banad/main/jiekouAD.txt
|ADRuls                                                                                                       |https://mirror.ghproxy.com/https://raw.githubusercontent.com/jhsvip/ADRuls/main/Combo.txt
|NextDNS Privacy - Sonos                                                                                      |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/sonos
|NextDNS Privacy - Roku                                                                                       |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/roku
|NextDNS Privacy - Alexa                                                                                      |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/alexa
|NextDNS Privacy - Apple                                                                                      |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/apple
|First-party trackers host list                                                                               |https://hostfiles.frogeye.fr/firstparty-trackers-hosts.txt
|bigdargon - hostsVN                                                                                          |https://raw.githubusercontent.com/bigdargon/hostsVN/master/hosts
|abuse.ch URLhaus Host file                                                                                   |https://urlhaus.abuse.ch/downloads/hostfile/
|PolishFiltersTeam - KADhosts                                                                                 |https://raw.githubusercontent.com/PolishFiltersTeam/KADhosts/master/KADhosts.txt
|FadeMind - Hosts Extra (Spam Hosts)                                                                          |https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.Spam/hosts
|BarbBlock                                                                                                    |https://paulgb.github.io/BarbBlock/blacklists/hosts-file.txt
|Winhelp MVPS Hosts                                                                                           |https://winhelp2002.mvps.org/hosts.txt
|The Big List of Hacked Malware Web Sites                                                                     |https://raw.githubusercontent.com/mitchellkrogza/The-Big-List-of-Hacked-Malware-Web-Sites/master/hosts
|Online Malicious URL Blocklist                                                                               |https://raw.githubusercontent.com/mitchellkrogza/The-Big-List-of-Hacked-Malware-Web-Sites/master/hosts
|StevenBlack - Hosts                                                                                          |https://raw.githubusercontent.com/StevenBlack/hosts/master/hosts
|Game Console Adblock List                                                                                    |https://raw.githubusercontent.com/DandelionSprout/adfilt/master/GameConsoleAdblockList.txt
|Spam404 - Adblock List                                                                                       |https://raw.githubusercontent.com/Spam404/lists/master/adblock-list.txt
|Lightswitch05 - AMP Hosts                                                                                    |https://www.github.developerdan.com/hosts/lists/amp-hosts-extended.txt
|Lightswitch05 - Ads and Tracking                                                                             |https://www.github.developerdan.com/hosts/lists/ads-and-tracking-extended.txt
|Lightswitch05 - Tracking Aggressive                                                                          |https://www.github.developerdan.com/hosts/lists/tracking-aggressive-extended.txt
|OISD Big List                                                                                                |https://raw.githubusercontent.com/sjhgvr/oisd/main/domainswild2_big.txt
|FadeMind - hosts.extras/add.2o7Net                                                                           |https://raw.githubusercontent.com/FadeMind/hosts.extras/master/add.2o7Net/hosts
|ethanr - DNS-Blacklists                                                                                      |https://bitbucket.org/ethanr/dns-blacklists/raw/8575c9f96e5b4a1308f2f12394abd86d0927a4a0/bad_lists/Mandiant_APT1_Report_Appendix_D.txt
|Threat-Intel                                                                                                 |https://osint.digitalside.it/Threat-Intel/lists/latestdomains.txt
|jdlingyu - ad-wars                                                                                           |https://raw.githubusercontent.com/jdlingyu/ad-wars/master/hosts 
|Perflyst and Dandelion Sprout's Smart-TV Blocklist                                                           |https://raw.githubusercontent.com/Perflyst/PiHoleBlocklist/master/SmartTV-AGH.txt
|anudeepND - Adservers                                                                                        |https://raw.githubusercontent.com/anudeepND/blacklist/master/adservers.txt
|Matomo.org - Referrer Spammers                                                                               |https://raw.githubusercontent.com/matomo-org/referrer-spam-list/master/spammers.txt
|Matomo - Referrer Spam Blacklist                                                                             |https://raw.githubusercontent.com/matomo-org/referrer-spam-blacklist/master/spammers.txt
|ZeroDot1 - CoinBlockerLists                                                                                  |https://zerodot1.gitlab.io/CoinBlockerLists/hosts_browser
|BlueSkyXN                                                                                                    | https://mirror.ghproxy.com/https://raw.githubusercontent.com/BlueSkyXN/AdGuardHomeRules/master/all.txt
|NextDNS Privacy - Windows                                                                                    |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/windows
|NextDNS Privacy - Xiaomi                                                                                     |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/xiaomi
|NextDNS Privacy - Huawei                                                                                     |https://raw.githubusercontent.com/nextdns/native-tracking-domains/main/domains/huawei
|miaoermua                                                                                                    |https://raw.githubusercontent.com/miaoermua/AdguardFilter/main/rule.txt
|jerryn70 GoodbyeAds                                                                                          |https://raw.githubusercontent.com/jerryn70/GoodbyeAds/master/Formats/GoodbyeAds-AdBlock-Filter.txt
|8680 GoodbyeAds                                                                                              |https://raw.githubusercontent.com/8680/GOODBYEADS/master/dns.txt
|8680 GoodbyeAds白名单                                                                                        |https://raw.githubusercontent.com/8680/GOODBYEADS/master/allow.txt
|FastHost                                                                                                     |https://raw.githubusercontent.com/xiulou23/FastHostSync/main/Hosts
|Adguard移动广告过滤器                                                                                       |https://raw.githubusercontent.com/AdguardTeam/FiltersRegistry/master/filters/filter_11_Mobile/filter.txt
|global anti-scam                                                                                             |https://raw.githubusercontent.com/elliotwutingfeng/GlobalAntiScamOrg-blocklist/main/global-anti-scam-org-scam-urls-pihole.txt
|hole.cert.pl                                                                                                 |https://hole.cert.pl/domains/domains.txt
|PolishFiltersTeam (KADhosts)                                                                                 |https://raw.githubusercontent.com/PolishFiltersTeam/KADhosts/master/KADhosts.txt
|Phishing.army (Extended)                                                                                     |https://phishing.army/download/phishing_army_blocklist_extended.txt
|vdbhb59 (Unified Hosts)                                                                                      |https://hosts.flossboxin.org.in/files/hosts
|frogeye.fr (multiparty-trackers)                                                                             |https://hostfiles.frogeye.fr/multiparty-trackers.txt
|notrack-blocklists (Blocklist)                                                                               |https://gitlab.com/quidsup/notrack-blocklists/-/raw/master/trackers.list
|VeleSila (yhosts)                                                                                            |https://raw.githubusercontent.com/VeleSila/yhosts/master/hosts
|Hagezi  Threat Intelligence Feeds                                                                            |https://cdn.jsdelivr.net/gh/hagezi/dns-blocklists@latest/adblock/tif.txt 

<h2 id="b">🛠️ 快速开始</h2>
### 示例配置

```yaml
application:
  rule:
    #远程规则订阅，path为 http、https地址
    remote:
      - name: 'Subscription 1'               #可选参数: 规则名称，如无将使用 path 作为名称
        path: 'https://example.org/rule.txt' #必要参数: 规则url，仅支持 http/https，不限定响应内容格式
        type:  easylist                      #可选参数: 规则类型：easylist (默认)、dnsmasq、clash、smartdns、hosts

    #本地规则，path为 操作系统支持的绝对或相对路径
    local:
      - name: 'private rule'
        path: '/rule/private.txt'

  output:
    #文件头配置，将自动作为注释添加至每个规则文件开始
    #可使用占位符 ${name}、${type}、${desc} 以及 ${date} (当前日期)
    file_header: |
      ADFS Adblock List
      Title: ${name}
      Last Modified: ${date}
      Homepage: https://github.com/fordes123/ad-filters-subscriber/
    path: rule   #规则文件输出路径，相对路径默认为程序所在路径
    files:
      - name: easylist.txt     #必要参数: 文件名
        type: EASYLIST         #必要参数: 文件类型: easylist、dnsmasq、clash、smartdns、hosts
        desc: 'ADFS EasyList'  #可选参数: 文件描述，可在file_header中通过 ${} 中使用
        filter:                #可选参数: 包含规则的类型，默认全选
          - basic              #基本规则，不包含任何控制、匹配符号, 可以转换为 hosts
          - wildcard           #通配规则，仅使用通配符
          - unknown            #其他规则，如使用了正则、高级修饰符号等，这表示目前无法支持
```

---
本程序基于 `Java21` 编写，使用 `Maven` 进行构建，你可以参照示例配置，编辑 `src/main/resources/application.yml`
，并通过以下任意一种方式快速开始：

#### **本地调试**

```bash
git clone https://github.com/fordes123/ad-filters-subscriber.git
cd ad-filters-subscriber
mvn clean
mvn spring-boot:run
```

#### **Github Action**

- fork 本项目
- 自定义规则订阅 (可选)
    - 参照示例配置，修改配置文件: `src/main/resources/application.yml`
- 打开 `Github Action` 页面，选中左侧 `Update Filters` 授权 `Workflow` 定时执行(⚠ 重要步骤)
- 点击 `Run workflow` 或等待自动执行。执行完成后相应规则生成在配置中指定的目录下

#### **Codespaces**

- 登录 `Github`，点击本仓库右上角 `Code` 按钮，选择并创建新的 `Codespaces`
- 等待 `Codespaces` 启动，即可直接对本项目进行调试

### 如何更新

当源代码存在更新时，(你的)仓库首页会出现如下图提示:
<img src="./screen.png">

此时选择 **Sync fork** 再选择 **Update branch** 即可同步更新.  
(如曾修改过源代码，那么合并可能存在冲突，请谨慎处理)





## ⭐ 感谢支持
<p align='center'>
  <a href="https://github.com/Shura23/adghRuleShura23/stargazers">
    <img src="https://api.star-history.com/svg?repos=Shura23/adghRuleShura23&type=Date">
  </a>
</p>


