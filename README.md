## VPS推荐

　　VPS, 即Virtual Private Server, 虚拟私人服务器。租VPS好处就是既可以独享服务器的网络线路，又可以在服务器上搭建自己的网站，也可以通过搭建公用VPN赚点外快，同时，也可以搭建属于自己的云盘（[OwnCloud](https://github.com/owncloud/core)）。

　　通过VPN、COW或Shadowsocks客户端连接VPS服务端的网速是有多种影响因素的：其一，**`机房地理位置`**，香港的肯定比台韩新日美欧要快，华南地区速度排序就是HK > TW > SG > JP > KR > US > EU；其二，**`线路`**，现在有CN2直连的线路，当然比一般线路快；其三，**`自身使用的网络供应商`**，国内不同的供应商连接不同机房的线路是不同的，番墙转的弯多少也不一样；其四，**`机房带宽`**，香港的带宽一直很小，基本都是1～10Mbps，常见的都是2Mbps或3Mbps，而台湾是100Mbps，日本带宽是Gbps为单位的，但服务器带宽大不意味着你的速度快，毕竟得遵循短板原理，本地区的互联网服务商提供的带宽不足也是会极大影响到用户体验的；其五，**`价格`**，想要好的VPS稳定的网络环境，当然$是必须的，无论是向本地区网络服务商购买网络，还是VPS购买，都是money决定了格调；其六，是否使用网络单向/双向服务器 **`加速软件`**，如FinalSpeed双边加速Shadowsocks，能明显提升浏览器访问网页、看视频的效果；其七，**`无线/有线`**，无线的网络环境远差于有线，家用路由器、终端间距离、网络重叠等等都影响着无线的数据传输，例如，同为电信20Mbps，广东地区ping香港CN2线路，有线基本在6～10ms，当无线环境中只有一台终端且网络稳定时ping值为18～37ms。

### 最壕最好用最稳定

　　 ***<u>最壕最好用最稳定</u>*** 的VPS供应商：[www.rackspace.com](http://www.rackspace.com)，`rackspace`是面向企业的云计算提供商。

价格：  
管理费：**$50**/month  
配置费：**$33**/month 起  
按流量收费：**$0.2**/GB 起  

评价：最壕最好用最稳定，即便是同一个机房，别人家的会宕机，而这家是不会的，且有数据备份，属于`Managed Host`，一个月下来，对于游戏玩家，用得稍微少点一个月开支也得过**100美元**，之前在一个讨论区见人账单月开销 **$300**。

### 最速度

　　除最壕VPS外，再从最速度方面列举出合适的VPS供应商，说到speed，对于中国用户肯定就属香港台湾日本三地最快了，当然，大体速度排序依然是上面所说的，为了给下面的VPS介绍留些余地，同时又满足性价比，所以这一小节只列举HK最优秀的VPS，并给出各自最便宜价格。

1. [`Yard VPS`](https://www.yardvps.com/billing/aff.php?aff=2519) [https://www.yardvps.com/](https://www.yardvps.com/billing/aff.php?aff=2519)

	最近发现了这个十分棒的供应商，由于香港的机房，被国内限速严重，台湾的机房更适合大陆环境，而且这家供应商的VPS起价还算实惠，另外，相比前几年，这个供应商的名声好太多了，考虑多方面原因，所以将之列为最速度榜首

	价格：TW **$5.95**/month起   
	配置：1CPU TW 100GB Bandwidth 100Mbps，1GB RAM，50GB Storage   
	测试IP：103.78.122.171（台北）、103.102.160.243（东京）

	测试文件：http://lg.tw.psychz.net/200MB.test （台北）、http://lg.jp.psychz.net/200MB.test （东京）

2. [`UFOVPS`](https://www.ufovps.com)  https://www.ufovps.com  

   机房：香港沙田电信BGP机房，CN2双向直连线路；美国KT机房(Krypt)，接驳CN2中国优化线路（自称中美最快线路之一）  

   价格：HK **￥59**/month，USA **￥35**/month 均为KVM架构   
   配置：HK 300G Bandwidth  3Mbps，1GB Memory，30GB Storage；USA 500GB Bandwidth 100Mbps，512MB Memory，20GB Storage  
   测试IP：118.193.210.100（香港）、98.126.65.220（美国）  

   评价：对于华南地区的小伙伴们来说，体验还是不错滴，两个机房都采取线路优化，尤其香港CN2线路还是值得信赖的；不过带宽只有3Mbps&300GB，同样不支持D(DOS)防御。『*★★★★*』

3. [`8云`](http://www.8xen.com/)  http://www.8xen.com/  

   机房：香港新世界CN2节点、美国加州CN2节点  
   价格：**￥29**/month起步，XEN架构  
   配置：1CPU、512MB Memory、20GB SSD，2Mbps 50GB Bandwidth/1Mbps No Limited Bandwidth起  
   测试IP：43.255.107.1  

   评价：最便宜的香港CN2节点之一；带宽太小，不适合下载较大文件；建议南方的孩子或者对流量需求不多的孩子选择1Mbps，带宽对你们的网站访问体验影响较小；而北方的而且没有太多流量要求的鞋子们选择2Mbps。『*★★★*』

4. [`阿里云香港B区`](https://ecs-buy.aliyun.com/)  https://ecs-buy.aliyun.com/ 仿AWS的弹性云服务器 **￥1**/GB  **￥0.30**/小时  据说是『*流量计费*』的最好选择，反正我不用～『*★★★*』

5. [`枫叶主机`]( https://www.fyzhuji.com)  https://www.fyzhuji.com  

   机房：香港沙田和新立讯机房，以及美国LA和俄罗斯新西伯利亚机房  
   价格：HK KVM架构 **￥60/**month起，LA**￥25**或**45**/month起，俄罗斯**￥35**/month起  
   配置：HK 1CPU、30/10GB Storage，500GB Bandwidth，5/50Mbps，1/0.5GB Memory，前者为沙田CN2线路  
   测试IP：118.193.244.200（沙田）、103.219.192.60（新立讯）、103.219.193.70（LA）、103.219.194.70（LA CN2）、195.43.95.250（Russia）

   测试文件：http://118.193.244.200/100MB.test （沙田）、http://103.219.192.60/100MB.test （新立讯）、http://103.219.194.70/100MB.test （LA CN2）

   评价：新厂家，不支持D(DOS)防御；CN2线路为5Mbps，不过最值得推荐的不是这家的VPS，而是虚拟主机和Shadowsocks，虚拟主机挂网站10G流量**￥60**/Yr起，也提供国内外中转的Shadowsocks **￥40**/Yr起，全国范围的速度都是极快的。『*挂博客首选，对中国线路优化极好，甚至有俄罗斯主机  ★★★★☆*』

6. [`GigsGigsCloud`](http://www.gigsgigscloud.com/)  http://www.gigsgigscloud.com/  

   机房：HGC香港和记电讯机房、马来西亚AIMS机房  
   价格：OpenVZ架构为主 **$18**/Yr（**￥120**）起，但相比该方案，还是建议使用**6美元**/month（**￥40**）的方案  
   配置：**$6**方案  1CPU、512MB、10GB Storage、1TB Bandwidth  
   测试IP：43.251.156.10（HK）、 210.1.226.1（MY）

   测试文件：http://www.gigsgigscloud.com/download/test.zip （HK）

   评价：Cloudlet B对没有对中国线路进行优化，时常会绕远到日本，甚至绕道美国，故推荐选购有优化的Cloudlet C；很多人都说C方案是10Mbps，但其官网并未提及带宽，原来官网写着10Mbps，但很多用户使用说达不到（应该是OpenVZ超额分配导致），所以现在没有写带宽了；B方案，在闲时还是比较好的，可一到高峰期便会绕道了；而且Cloudlet B是共享最大100Mbps上行带宽，理所应当慢。『*★★★★*』

7. [`莲花VPS · LotuServer`](http://www.lotuserver.com/)  http://www.lotuserver.com/  

   机房：香港沙田机房、美国洛杉矶CS机房和ENZU机房、凤凰城IOF机房  
   价格：HK **￥99+10**/Yr、**￥32**/month起  
   配置：HK 年费99为1CPU、128MB Memory、1GB SSD、 500GB Bandwidth、1Mbps；HK 32月费为1CPU、512MB Memory、5GB SSD、750GB Bandwidth 

   评价：年费方案的硬盘容量十分小，只有1GB，顶多用来开Shadowsocks（带宽不如`枫叶主机`专门的SS套餐），架网站就不用想了，只能选择月费方案；另外官方网站说支持D(DOS)防御；同时比较适合学生群体学习使用。『*★★★*』


### 最实惠

　　最实惠莫过于免费了，不过不是无限期无限量的免费，而是对新用户而言的，毕竟世界上没有免费的午餐，当然如果真心想吃也是可以在舔到的。例如[Amazon AWS](https://aws.amazon.com)的EC2，可**免费使用一年**，不过每月只有15GB流量；google的[GCE](https://cloud.google.com)和[DigitalOcean](https://www.digitalocean.com/?refcode=4daef23f81a9)都可免费使用两个月；类似DigitalOcean赠送 **$10**（可用两个月），[Vultr](https://www.vultr.com/?ref=6983219)注册新用户时会有不定额度的美金余额存储于你的账户，这两家为了防止恶意注册，封号很严，所以不要使用重复信息进行多次注册。

1.  [`Vultr`](https://www.vultr.com/?ref=6983219)  

    机房：新加坡、东京、美国、欧洲  
    价格：**$5**/month（**￥33**）起  
    配置：1CPU、768MB Memory、1000GB Bandwidth起  
    测试IP：108.61.201.151（Tokyo）、45.32.100.168（SG）、104.156.230.107（硅谷）、108.61.219.200（LA）  
    测试文件：http://hnd-jp-ping.vultr.com/vultr.com.100MB.bin （Tokyo）、http://sgp-ping.vultr.com/vultr.com.100MB.bin （SG）、 http://sjo-ca-us-ping.vultr.com/vultr.com.100MB.bin （硅谷）、	http://lax-ca-us-ping.vultr.com/vultr.com.100MB.bin （LA）

    评价：优惠狠多、技术狠强、机房狠多。优惠政策二选其一，新用户使用链接注册可获得一定的金额（当前**20美金**，验证&follow&发布Twitter又奖励**3美元**），新用户[充多少送多少](https://www.vultr.com/match/)（最多送 **$100**，且赠送的金额只能使用12个月），老用户充值八折优惠，而且最便宜的价格和DigitalOcean一样，不过Vultr有日本的机房，速度比DO洛杉矶机房快，且流量达1T；支持D(DOS)防御，从最普及的技术角度来谈，和DO一起作为最智能的VPS平台，也意味着管理员参与服务器架构的程度度很低；机房遍布亚欧美，是分布最广泛的服务商。另外，Tokyo和新加坡的速度虽不算最快，但肯定足够稳定，甚至超越了Linode。『*推荐给资金不足的朋友  只需充**5美元**即可用半年★★★★☆*』

2. [`搬瓦工 · BandwagonHost`](https://bandwagonhost.com/)

      机房：洛杉矶、凤凰城、佛罗里达、佛蒙特、荷兰  
      价格：搬瓦工本来是有很多极为便宜的VPS的（**3.99美元**/年），但是用的人多了，还怕抢不完ip么？现在最亲民的是 **$19.9**/年（约**￥132**）  
      配置：1CPU、256MB Memory、128MB vSWAP、500GB Bandwidth、10GB SSD、1GB Network、OpenVZ/KVM起步  
      测试IP：104.194.76.14（LA）、192.243.118.26（凤凰城）、184.105.138.67（佛蒙特）、23.252.104.22（佛罗里达）、45.62.122.106（荷兰）

      评价：全球最为人知的廉价VPS供应商，搬瓦工提供ss自动安装功能；狠便宜的老牌  建议洛杉矶机房  4.66%优惠码：` IAMSMART50BAR1`『*★★★★*』

3. [`Kvmla`](http://www.vpser.net/go/kvmla1)  年费**99元**人民币，机房在美国，和DO差不多的ping值，适合挂Shadowsocks + FinalSpeed加速番墙 ，由于连接慢，不适合挂大型网站；『***￥99***』

4. [`RamNode`](https://clientarea.ramnode.com)  OpenVZ最廉价的主机年费为 **$15**（约**￥100**），机房均在美国，推荐选购西雅图机房，网络速度同搬瓦工不相上下；『***￥100***』

5. [`HostUS`](http://www.hostus.cn/go/hostus-hk-256s)  HK Singapore Sydney http://www.hostus.cn/go/hostus-hk-256s  

   价格：OpenVZ架构 最便宜 **$25**/Yr（约 **166元**）三地可选，USA Atlanta **18.95美元**/Yr（约**￥126**）  
   配置：1vCPU，256MB Memory，10GB SSD，500GB Bandwidth 起  
   测试IP：45.124.64.3（HK）、210.16.120.5（Singapore）、27.100.36.5（Sydney）、162.245.216.243（Atlanta）  
   测试文件：http://hk-lg.hostus.us/100MB.test （HK）、http://sgp-lg.hostus.us/100MB.test （Singapore）、http://syd-lg.hostus.us/100MB.test （Sydney）、http://atl-lg.hostus.us/100MB.test （Atlanta）  

   评价：机房的连接速度不太稳定，时常会发生线路绕远的情况，但价格便宜足以吸引大量用户了，而且还支持D(DOS)防御；现在洛杉矶机房KVM VPS已开启CN2直连，而HK的CN2直连还会远么，那时HK的VPS肯定会被哄抢，那时再加颗*☆*。『*★★★★*』



6.  [`HostHatch`](https://hosthatch.com/)    

    机房：IBM旗下的Softlayer香港机房以及美国等地  
    价格：OpenVZ架构 **$30**/Yr起（约**200元**）或 **2.67美元**/month  起  
    配置：1CPU、256MB Memory、30GB SSD，1TB Bandwidth起  
    测试IP：119.81.130.170（HK）、107.181.166.4（LA）  
    测试文件：http://speedtest.hkg02.softlayer.com/downloads/test100.zip （HK）、http://mirror.lax.hosthatch.com/100mb.bin （LA）

    评价：支持D(DOS)防御，速度还是很不错的，相对HostUS，HostHatch还是更稳定、更快的。『*★★★★*』

7. [`VirMach`](https://virmach.com/)  **$7.5**/Yr起步（约**￥50**），便宜是便宜，不过即使是最合适的机房地址，在例举出来的VPS中依然是最慢的，很适合在校生学习Linux；『***￥50***』

8. `GigsGigsCloud`、`DigitalOcean`  均可进入『*最实惠*』之流，其中学生用户使用学校的Email可以在[Github Education](https://education.github.com/pack)上申请DigitalOcean的学生优惠金 **$100**（+注册赠送的**10美元**最多可以连续使用22个月），另外，HostUS和HostHatch连接速度还根据用户使用的网络供应商而有所区别，如电信联通用户连接较好，而移动用户就不那么流畅了。


> Vultr已成为Captain主力VPS，故也推荐大家使用，限时优惠链接：[https://www.vultr.com/?ref=6983219](https://www.vultr.com/?ref=6983219) ，赠送**20美元**，不过，注册时需要使用信用卡或者PayPal，如果使用Visa等信用卡需要支付 **$5**进行手续验证，1个月后会退还，推荐使用PayPal需要充值 **5美元**，存储在账号中，所以新用户最多可以有**28美金**存在于Vultr账号，由于Vultr支持月费的同时也支持按时计费，所以充值**30多元**足够使用半年的了。机房选择日本，再安装FinalSpeed，消耗两倍流量，但速度体验提升不少，可达到国内访问的速度效果。

### 最老牌

1.  [`Linode`](https://www.linode.com/?r=de15b88a486da4c4804c5f935eab2cd5b9fdb56f)  国际老牌VPS供应商，以VPS界高富帅闻名，不过，Linode最近也开通了廉价版本， **$5**/month，中国用户推荐东京机房，其性能优异，Gpbs级别的大水管，网速快，最近的Tokyo2机房代替了之前长期售罄的Tokyo1机房；
2.  [`棉花糖 · Sugarhosts`](http://www.sugarhosts.com/)  最低**5.95美元**/month（约39元人民币）  500GB流量  有香港机房硬盘有两种支持方式，SSD和机械；

3.  [`GoDaddy`](https://sg.godaddy.com/zh/hosting/web-hosting)  世界上拥有最多域名的公司，同时也有VPS业务，最便宜的价格是按年结算时**28人民币**/month，且年费用户获赠免费域名，机房推荐新加坡；

4.  [`Amazon AWS`](http:aws.amazon.com)  的CE2、[`Google Compute Engine`](https://cloud.google.com/compute/)  、[`Windows Azure`](https://azure.microsoft.com/zh-cn/)  , 由于EC2提供用户免费使用一年，所以在本文章之后，Captain会专门写一篇关于AWS的EC2的使用心得，与君分享；

5.  [`VPS.NET`](http://www.vps.net)  同样也是高富帅VPS服务商的代表，最近一年才开始有平民方案的，**$5**/month起步，当前只有欧美洲的机房供选择；

6.  [`Host1Plus`](http://www.host1plus.com/)  主打大西洋周边国家，**$2**/month起步，拥有美国、巴西、南非、德国的机房；

7.  [`中華電信 · hicloud`](http://hicloud.hinet.net/)  台湾著名的网络供应商，Mini款每日**4圆新台币**，即每日**0.84元**人民币，且每日1GB流量，台湾的带宽比香港的大，百兆带宽，优势明显，而且延迟低，ping值基本在50～70ms；『*对于搭建VPN销售给他人使用的情况，可以考虑入手hicloud高一级别的VPS*』

8.  [`OneasiaHost`](http://www.oneasiahost.com/)  新家坡的主机服务商，**$12**/quarter（约**￥80**）起步，每月200G流量；



## 优惠链接&优惠码

　　接下来，给大家列出各家VPS供应商的新用户注册优惠链接，直接通过官方链接的官网注册不会送金额：

1.  [`Vultr`](https://www.vultr.com/?ref=6983219)  https://www.vultr.com/?ref=6983219  **$20**金额，需要用户PayPal充值**5美金**或者信用卡暂存**5美金**；https://www.vultr.com/match/ 新用户充多少送多少，最多送**100美元**，且赠送的金额使用期限为12个月；

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
8.  8云科技 八折优惠码：`VPSMM8`
9.  枫叶VPS 9.5折优惠码：`10vps` 



##  支付方式

　　国内外的VPS服务商都提供了 **`信用卡`** 和 **`借记卡`** 支付方式，甚至有的要求在注册时提供信用卡卡号和卡背面后三位的CVV码，而也有些要求在注册时最少充值 **$5**，也有的是在购买VPS时才允许注册用户信息。国内的银联信用卡、借记卡不一定符合所有国外VPS厂商的要求，可能只限制使用VISA、MasterCard，例如Amazon Shop便是不允许使用银联信用卡，海淘用户一般是使用Visa信用卡。如果对此行为反感的鞋子们请绕道免费VPS，当然，免费VPS也有要求提供信用卡或借记卡信息，如AWS EC2、GCE均需要录入银联借记卡或者VISA、MasterCard的信息。

　　除信用卡、借记卡支付外，绝大多数都会提供 **`PayPal`** 支付，在PayPal官网注册信息并绑定信用卡或者借记卡便可以消费了，PayPal用途挺广泛的，绝对不会少于支付宝，所以在支付宝不能使用的情况下推荐优先使用PayPal，例如Vultr。

　　有些VPS厂商专门考虑中国用户的需求，提供了 **`支付宝`** 支付方式，例如搬瓦工、HostUS、Host1Plus、Sugarhosts、Kvmla、Godaddy。










