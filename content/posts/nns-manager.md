---
title: "Dfinity神经元抵押教程"
date: 2021-05-19 T16:00:01+08:00
draft: false
summary: "Dfinity实现了一个自治化的区块链系统，使得传统应用在去中心化体系下的可能性。Dfinity实现自治化很重要的一个特色是全网维护一个开放式的网络神经元系统(NNS)，通过算法的方式实现了民主投票和民主决策。本文介绍了如何成为治理体系的一员：抵押神经元。"
---

Dfinity实现了一个自治化的区块链系统，使得传统应用在去中心化体系下的可能性。Dfinity实现自治化很重要的一个特色是全网维护一个开放式的网络神经元系统(NNS)，通过算法的方式实现了民主投票和民主决策。本文介绍了如何成为治理体系的一员：抵押神经元。

### 01
打开神经元管理界面 [](https://nns.ic0.app/)
>注：
>请使用带有指纹识别,或者人脸识别功能的设备以便进行身份注册;
>请使用Firfox或者Safari浏览器,Chrome暂不支持。
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"1.png")

### 02
点击登录，此时如果账号已存在，需要获取设备上存储的身份信息(指纹,面部信息,Yubikey硬件钱包)。如果没有注册身份认证，则跳转到[](https://identity.ic0.app/)进行身份注册。Dfinity不需要在各个应用都去注册新身份,有了这个唯一标识就可以全网畅游。
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"2.1.png")
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"2.2.png")
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"2.3.png")
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"2.4.png")

### 03
认证成功之后，你会获得一个全网唯一Number，请务必牢记！以后导出身份到新设备的时候需要用到。

### 04
请在多台设备上对你的身份进行备份，以免单台设备遗失，造成不必要的损失。在登录界面,，点击"Already registered but using a new device?"，输入你的唯一Number，导出界面连接在原来完成验证的设备上面打开，点击确认进行身份确认；或者也可以选择扫描二维码打开授权页面。
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"4.1.png")

### 05
注册好账号之后，重新访问 [](https://nns.ic0.app/) ，输入刚才的唯一标识number(例如:70162)，进行身份认证之后，就可以登录你的钱包和神经元管理页面了。
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"5.1.png")

这时候你会发现系统已经默认给你创建了一个主钱包账户，你也可以需要添加子账户。在下面的步骤中，你需要往改钱包转入至少1.2个ICP进行神经元创建。

### 06
拥有了一定的icp之后，点击NEURONS按钮，切换到神经元页面。在这里进行神经元创建，你可以输入你要质押进神经元的icp的个数(至少一个ICP)，拖动滑块来设置神经元溶解时延，点击锁定就创建好了你的第一个神经元。
>注：神经元是参与网络治理的单位，通过对网络中的提案进行投票来行使你的权利，不同的神经元投票的表决力是不一样的，基础来说，投票力与质押的icp占全网所有成正比，但是神经元的存续时长(神经元年龄)对投票权有一个最多25%的加成， 初始设置的神经元溶解时延对投票力有一个最多100%的加成，但是一旦设置了溶解时延就意味着需要质押的币无法流通，现在支持的设置溶解时延的范围是180天到8年。

### 07
神经元投票是基本操作，筛选出目前网络中处于open状态的提案，就可以进行投票了，但是投票的结果对于神经元的成熟的是有影响的，如果您的投票都和最终决议背道而驰，则对您的神经元的成熟没有任何益处;相反如果您顺应网络中多数人(至少51%)的决议，则会促进您的神经元的成熟，所以请用好您的投票权。如果您暂时没有想法，或者觉得一直需要操作太麻烦，系统提供了跟随机制，让您能够将您的决议绑定某个活跃的神经元，跟随它的决议，这样就能方便的参与网络治理了，注意您跟随的神经元是不会分得您的治理奖励的。

换句话说就是对于单个提案，越多的人参与投票，奖励越小;你赞成的提案通过率越高，收益越高。

![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"7.1.png")
上图展示了您的拥有的神经元、以及溶解时延、质押数量
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"7.2.png")
上图展示了神经元的成熟度，和投票历史记录
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"7.3.png")
上图展示了网络中开放投票的提案
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/"7.4.png")
上图展示了您设置跟随的神经元节点，值得注意的是不同的提案类型，您可以分开设置跟随的对象
也可以直接自己投票，打开vote页面，查看提案详情，选择是adopt还是reject。
![](https://storageapi.fleek.co/lyswifter-team-bucket/ice-foundation/Create NNS/7.5.png "7.5")

### 08
这样下来，就拥有了自己的治理神经元，随着网络中提案的增多，神经元会更快的成熟，一旦成熟度达到10%，您就可以基于这个神经元生成一个包含奖励ICP的神经元，(新神经元中ICP的个数 = 老神经元icp数量 * 成熟度)，并立即溶解这个神经元，这样就可以获得其中的ICP奖励;也可以将暂时不溶解此神经元，而是让其自动跟随旧神经元，相当于复投。

