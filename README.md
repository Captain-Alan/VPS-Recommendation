---
title: VPS推荐
date: 2016-09-11 19:50:48
categories: GFW Break
tags: [Geek, VPS]
---

　　Break  GFW时，大家都应该熟悉GoAgent，除此，再就是购买月费或年费的VPN，前者虽然免费但使用人数众多且网速极为不稳定，后者花费些金钱虽然可以获得较为稳定的网络，但随着VPN卖家的用户越来越多，他们也对用户有着一定限制，例如不能下载、不能看1080P，而且多数时候还得要求你家里、宿舍、公司网速在50M以上的带宽才能有比较不错的体验，手机3G、4G有时也连接不稳定，所以当下公用的GFW Breaker都有不少的局限性。

　　虽然VPS的主要目的并不是用于搭建VPN，不过在谈VPS前，Captain还是有必要推荐一些不错的公用VPN。
　　首先，免费的Breaker有倒是有，对于仅要求查查资料的你来说应该也是足够了。如若仅仅是番墙浏览网站而已，免费首选2016年6月份之前的[Lantern](https://program-pocket.oss-cn-hongkong.aliyuncs.com/GFW-Breaker/lantern.exe)，同Shadowsocks一样不支持ping和下载被墙网站的文件；其次是[赛风](http://www.psiphon3.net/zh/index.html)；再就是日本筑波大学协同其他各国大学搭建的Free VPN平台——[VPNGate](http://www.vpngate.net/)，只建议科研工作者使用，忘图利者良知发现，不要占用科研的资源来Download各种东西，最后的，也是同Lantern一样较为快捷的番墙方法——[修改hosts文件](https://serve.netsh.org/pub/ipv4-hosts/)，虽可以访问Google、Twitter，但是有些网站依然是无法访问的。

>  Captain手头已经在用自己的VPN了，所以暂时没有下载好的免费番墙软件包，如若Captain手头有这些安装包会立刻更新出下载链接；另外，Captain手头只有Lantern的可执行文件，没有安装文件，Github上搜索的Lantern现在是要付费的了，大家如果有2016年7月份之前免费的Lantern可执行文件，欢迎在下面留言（Disqus 评论系统的加载需要翻墙）；VPNGate地址在Github上有不需要翻墙便能访问的链接，即VPNGate网站镜像。

　　其次便是付费VPN，对于网速在10M以上带宽的可以选择[二师兄VPN](http://www.2-vpn5.com/home.action?ic=6475297BD0)，对于不愿意繁琐地购买自己的VPS并搭建VPN的可以考虑购买**￥540**的终生套餐

>  ***<u>注意</u>***：二师兄VPN有假的，只要网址中带有***`2sxvpn`*** 便是假的，而且没有终生套餐；而真正的二师兄VPN的网址是会隔一段时间有规律变更的，例如现在是2-vpn5，之后就可能会是2-vpn6。
>  二师兄VPN终生用户，国内用户20Mbps带宽，对于台湾地区ping Google的时间值基本都是50ms左右，ping香港Google则是30ms左右；下载线路（日本俩，美国仨）是允许下载的，其余（台湾10，香港2，日本3、美国俩）都是不允许下载的，切忌下载后封号没人会提前告诉你的，当然有时卖家也还是很好说话的；另外终生用户可以三个终端同时登陆，移动端具体情况还得看现有的网络带宽，例如3G多数连不上VPN，可以考虑使用Shadowsocks，4G连接VPN基本没有问题。

　　再说一下移动端番墙，如果想要老手机番墙，或者3G手机番墙，基本没有特别好的方案，公用的VPN本来就是一堆人分用固定带宽，本身机器连接网络环境的前提都不具备何谈愉快地番墙墙，不过要推荐比较稳定的方案，有还是有的：可以以高价选购高端VPN，共用的人少，甚至可以单独为你搭建一条线路；选择不错的VPS，自己搭建VPN或者Shadowsocks，即使便宜也可以有不错的效果，只要使用人数可以由你控制，网速怎能不稳定，至少Captain的P6就可以稳定地访问Facebook、Twitter，这也是Captain为什么租用VPS搭建番墙服务器的原因之一。对于网络环境（WiFi）优秀的用户或者4G用户，可以使用公用的VPN、甚至免费的VPN（Lantern、赛风、[GreatFire](https://github.com/greatfire/wiki)），基本都可以满足你的上网需求了。
　　对于追求安全性能的用户而言，绝对不要使用公用VPN（包括付费的公用VPN），泄露个人信息是绝对的，绝对会泄露的，绝对会的，重要的事情必须说三遍；对于国内企业和在国内的外资企业，香港的VPS首当推荐，具体内容请看本文。

<!--  more  -->



## VPS推荐

　　VPS, 即Virtual Private Server, 虚拟私人服务器。租VPS好处就是既可以独享服务器的网络线路，又可以在服务器上搭建自己的网站，也可以通过搭建公用VPN赚点外快。

　　通过VPN、COW或Shadowsocks客户端连接VPS服务端的网速是有多种影响因素的：其一，**`机房地理位置`**，香港的肯定比台韩新日美欧要快，华南地区速度排序就是HK > TW > SG > JP > KR > US > EU；其二，**`线路`**，现在有CN2直连的线路，当然比一般线路快；其三，**`自身使用的网络供应商`**，国内不同的供应商连接不同机房的线路是不同的，番墙转的弯多少也不一样；其四，**`机房带宽`**，香港的带宽一直很小，基本都是1~10Mbps，常见的都是2Mbps或3Mbps，而台湾是100Mbps，日本带宽是Gbps为单位的，但服务器带宽大不意味着你的速度快，毕竟得遵循短板原理，本地区的互联网服务商提供的带宽不足也是会极大影响到用户体验的；其五，**`价格`**，想要好的VPS稳定的网络环境，当然$是必须的，无论是向本地区网络服务商购买网络，还是VPS购买，都是money决定了格调；其六，是否使用网络单向/双向服务器**`加速软件`**，Captain使用的是FinalSpeed，提升效果明显。

### 最壕最好用最稳定

　　先介绍***<u>最壕最好用最稳定</u>***的VPS供应商：***www.rackspace.com***，这家`rackspace`是面向企业的云计算提供商，价格嘛~~ 仅管理费就得**50美元**/month，还需要配置费，最便宜的是**33美元**/month，而且还按流量收费，最小带宽最便宜的是**0.2美元**/GB，一个月下来，对于游戏玩家，用得稍微少点也得过**100美元**/month，之前在一个讨论区见人账单**$300**/month。

### 最速度

　　除最壕VPS外，再从最速度方面列举出合适的VPS供应商，说到speed，对于中国用户肯定就属香港台湾日本三地最快了，当然，大体速度排序依然是上面所说的，为了给下面的VPS介绍留些余地，同时又满足性价比，所以这一小节只列举HK最优秀的VPS，并给出各自最便宜价格。

1.  [`UFOVPS`](https://www.ufovps.com)  https://www.ufovps.com  沙田机房电信CN2直连线路  最便宜￥59/month 300G流量  3Mbps带宽，速度极佳，Captain在广东地区ping值在25ms左右，时常达到18ms 20ms，不过带宽只有3Mbps，另外，其美国机房最便宜**￥35**/month 供君参考；『*高速优选 且稍贵  资金稍够推荐作为主力VPS*』

2.  [`8云`](http://www.8xen.com/)  http://www.8xen.com/  **￥29**/month起步，Captain所见最便宜的香港CN2节点之一，有两款入门型号可选，一个2Mbps只有50GB流量，另一个是1Mbps无流量限制，建议南方的孩子或者对流量需求不多的孩子选择第二个，带宽对你们的速度体验影响较小，而北方的而且没有太多流量要求的鞋子们选择第一个；

3.  [`新世界`](http://vpssj.net/)  http://vpssj.net/  最便宜**￥79**/month  不限流量；『*贵且高速*』

4.  [`阿里云香港B区`](https://ecs-buy.aliyun.com/)  https://ecs-buy.aliyun.com/ 仿AWS的弹性云服务器 **￥1**/GB  **￥0.30**/小时  据说是『*流量计费*』的最好选择，反正我不用~；

5.  [`HostUS`](https://my.hostus.us/cart.php?a=confproduct&i=6) 直达链接  https://my.hostus.us/cart.php?a=confproduct&i=6  最便宜**$25**/Yr（约**167元**）  月流量500G；『*略慢且便宜 性价比最高 满足绝大多数情况使用*』

6.  [`HostHatch`](https://hosthatch.com/)  https://hosthatch.com/  **$30**/Yr起（约**200元**）或 **2.67美元**/month；『*较快且便宜 性价比高*』

7.  [`枫叶主机`]( https://www.fyzhuji.com)  https://www.fyzhuji.com  CN2线路  VPS最低**￥60**/month，虚拟主机挂网站10G流量**￥60**/Yr，也提供国内外中转的Shadowsocks **￥150**/Yr 全国范围的速度都是极快的；『*高速优选  挂博客首选  对中国线路优化极好  甚至有俄罗斯主机*』

8.  [`GigsGigsCloud`](http://www.gigsgigscloud.com/)  http://www.gigsgigscloud.com/  最低**$6**/month（约￥40）拥有香港和马来西亚机房，Captain在广东的香港机房的ping值在30ms所有，甚至有达到时18ms；『*高速优选 性价比高*』

9.  [`莲花VPS · LotuServer`](http://www.lotuserver.com/)  http://www.lotuserver.com/  沙田机房  **￥99+10**/Yr起步 1G硬盘 500G流量；『*高速优选 性价比高 硬盘小 不适合架大型网站*　架小博客没问题』


### 最实惠

　　最实惠莫过于免费了，不过不是无限期无限量的免费，而是对新用户而言的，毕竟世界上没有免费的午餐，当然如果真心想吃也是可以在舔到的。例如[Amazon AWS](https://aws.amazon.com)的EC2，可**免费使用一年**，不过每月只有15GB流量；google的[GCE](https://cloud.google.com)和[DigitalOcean](https://www.digitalocean.com/?refcode=4daef23f81a9)都可免费使用两个月；类似DigitalOcean赠送**$10**（可用两个月），[Vultr](http://www.vultr.com/?ref=6983220-3B)注册新用户时会有不定额度的美金余额存储于你的账户，这两家为了防止恶意注册，封号很严，所以不要使用重复信息进行多次注册。

1.  [`Vultr`](http://www.vultr.com/?ref=6983220-3B)  新用户使用优惠码注册可获得一定的金额（2016年夏送**20美金**，验证&follow&发布Twitter又奖励3美元），这家的VPS最便宜为**$5**/month，价格和DigitalOcean一样，不过Vultr有日本的机房，速度比DO洛杉矶机房快很多，且流量达1T；『*速度稳定  甚至超过Linode  推荐给资金不足的朋友 优惠特别多  2016夏新用户只需充**10美元**即可用半年*』；

2.  [`搬瓦工 · BandwagonHost`](https://bandwagonhost.com/)  搬瓦工本来是有很多极为便宜的VPS的（**3.99美元**/年），但是用的人多了，还怕抢不完ip么？现在最亲民的是**$19.9**/年（约**￥132**），而且搬瓦工提供ss安装；『*狠便宜的老牌  建议洛杉矶机房  4.66%优惠码：` IAMSMART50BAR1` *』

3.  [`Kvmla`](http://www.vpser.net/go/kvmla1)  年费**99元**人民币，机房在美国，和DO差不多的ping值，适合挂Shadowsocks + FinalSpeed加速番墙 ，由于连接慢，不适合挂大型网站；『***￥99***』

4.  [`RamNode`](https://clientarea.ramnode.com)  OpenVZ最廉价的主机年费为**$15**（约**￥100**），机房均在美国，推荐选购西雅图机房，网络速度同搬瓦工不相上下；『***￥100***』

5.  [`VirMach`](https://virmach.com/)  **$7.5**/Yr起步（约**￥50**），便宜是便宜，不过即使是最合适的机房地址，在例举出来的VPS中依然是最慢的，很适合在校生学习Linux；『***￥50***』

6.  `HostUS`、`HostHatch`、`DigitalOcean`  均可进入『*最实惠*』之流，其中学生用户使用学校的Email可以在[Github Education](https://education.github.com/pack)上申请DigitalOcean的学生优惠金**$100**（+注册赠送的**10美元**最多可以连续使用22个月），另外，HostUS和HostHatch连接速度还根据用户使用的网络供应商而有所区别，如电信联通用户连接较好，而移动用户就不那么流畅了。


> Vultr已成为Captain主力VPS，故也推荐大家使用，限时优惠链接：[http://www.vultr.com/?ref=6983220-3B](http://www.vultr.com/?ref=6983220-3B) ，赠送**20美元**，不过，注册时需要使用信用卡或者PayPal，如果使用Visa等信用卡需要支付**$5**进行手续验证，1个月后会退还，推荐使用PayPal需要充值**5美元**，存储在账号中，所以新用户最多可以有**28美金**存在于Vultr账号，由于Vultr支持月费的同时也支持按时计费，所以充值**30多元**足够使用半年的了。机房选择日本，再安装FinalSpeed，消耗两倍流量，但速度体验提升不少，可达到国内访问的速度效果。

### 最老牌

1.  [`Linode`](https://www.linode.com/?r=de15b88a486da4c4804c5f935eab2cd5b9fdb56f)  国际老牌VPS供应商，以VPS界高富帅闻名，最便宜的是**$10**/month(约**￥66**)，中国用户推荐东京机房，其性能优异，Gpbs级别的大水管，网速快，不过东京机房已经长期售罄了，可以考虑新加坡机房；『*对于搭建VPN销售给他人使用的情况，可以考虑入手Linode东京机房，需要守株待兔*』

2.  [`棉花糖 · Sugarhosts`](http://www.sugarhosts.com/)  最低**5.95美元**/month（约39元人民币）  500GB流量  有香港机房硬盘有两种支持方式，SSD和机械；

3.  [`GoDaddy`](https://sg.godaddy.com/zh/hosting/web-hosting)  世界上拥有最多域名的公司，同时也有VPS业务，最便宜的价格是按年结算时**28人民币**/month，且年费用户获赠免费域名，机房推荐新加坡；

4.  [`Amazon AWS`](http:aws.amazon.com)  的CE2、[`Google Compute Engine`](https://cloud.google.com/compute/)  、[`Windows Azure`](https://azure.microsoft.com/zh-cn/)  , 由于EC2提供用户免费使用一年，所以在本文章之后，Captain会专门写一篇关于AWS的EC2的使用心得，与君分享；

5.  [`VPS.NET`](http://www.vps.net)  同样也是高富帅VPS服务商的代表，最近一年才开始有平民方案的，**$5**/month起步，当前只有欧美洲的机房供选择；

6.  [`Host1Plus`](http://www.host1plus.com/)  主打大西洋周边国家，**$2**/month起步，拥有美国、巴西、南非、德国的机房；

7.  [`中華電信 · hicloud`](http://hicloud.hinet.net/)  台湾著名的网络供应商，Mini款每日**4圆新台币**，即每日**0.84元**人民币，且每日1GB流量，台湾的带宽比香港的大，百兆带宽，优势明显，而且延迟低，ping值基本在50~70ms；『*对于搭建VPN销售给他人使用的情况，可以考虑入手hicloud高一级别的VPS*』

8.  [`OneasiaHost`](http://www.oneasiahost.com/)  新家坡的主机服务商，**$12**/quarter（约**￥80**）起步，每月200G流量；



## 优惠链接&优惠码

　　接下来，给大家列出各家VPS供应商的新用户注册优惠链接，直接通过官方链接的官网注册不会送金额：

1.  [`Vultr`](http://www.vultr.com/?ref=6983220-3B)  http://www.vultr.com/?ref=6983220-3B  **$20**金额，需要用户PayPal充值**5美金**或者信用卡暂存**5美金**；

2.  [`DigitalOcean`](https://www.digitalocean.com/?refcode=4daef23f81a9)  https://www.digitalocean.com/?refcode=4daef23f81a9  **$10**金额  Github学生验证**100美金**：https://education.github.com/pack  也就是说，**学生可以免费使用近两年**；

3.  [`Linode`](https://www.linode.com/?r=de15b88a486da4c4804c5f935eab2cd5b9fdb56f)  https://www.linode.com/?r=de15b88a486da4c4804c5f935eab2cd5b9fdb56f  **$10**金额，**20美元**优惠码：`PodcastInIt20`，在验证邮箱后完善个人信息时填在Promotion Code，  第一次注册后要求充值5美金；


　　有些优惠码是有条件赠送的给用户的，并不是所有用户都可以使用，而是新用户注册时使用的，且优惠码是由Captain爬来，并没有一一检验真实性，当然，Captain的钱包也不够我一个一个地买VPS〒_〒。以下是一些优惠码，按需选择。

1.  HostUS KVM主机八折优惠码：`LETKVM20` 
2.  HostUS OpenVZ主机八五折优惠码：`ZHUJICEPING` 
3.  UFOVPS九折优惠码：  `UFOVPS90%` 
4.  Host1Plus 八折优惠码：`CS30OFF` 
5.  VPS.NET 10美金优惠码：`GIVEME10` 
6.  搬瓦工 · BandwagonHost　4.66%优惠码：`IAMSMART50BAR1` 
7.  Godaddy　35%优惠码：`CJCRMN35`



##  支付方式

　　国内外的VPS服务商都提供了**`信用卡`**和**`借记卡`**支付方式，甚至有的要求在注册时提供信用卡卡号和卡背面后三位的CVV码，而也有些要求在注册时最少充值**$5**，也有的是在购买VPS时才允许注册用户信息。国内的银联信用卡、借记卡不一定符合所有国外VPS厂商的要求，可能只限制使用VISA、MasterCard，例如Amazon Shop便是不允许使用银联信用卡，海淘用户一般是使用Visa信用卡。如果对此行为反感的鞋子们请绕道免费VPS，当然，免费VPS也有要求提供信用卡或借记卡信息，如AWS EC2、GCE均需要录入银联借记卡或者VISA、MasterCard的信息。

　　除信用卡、借记卡支付外，绝大多数都会提供**`PayPal`**支付，在PayPal官网注册信息并绑定信用卡或者借记卡便可以消费了，PayPal用途挺广泛的，绝对不会少于支付宝，所以在支付宝不能使用的情况下推荐优先使用PayPal，例如Vultr。

　　有些VPS厂商专门考虑中国用户的需求，提供了**`支付宝`**支付方式，例如搬瓦工、HostUS、Host1Plus、Sugarhosts、Kvmla、Godaddy。










