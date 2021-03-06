---
title: "ICP基金会：Dfinity宣布将与以太坊集成"
date: 2021-06-04T19:38:34+08:00
draft: false
summary: 近日，Dfinity创始人Dominic发布信息称Dfinity将与以太坊网络整合，而这将产生巨大的价值。但应如何做到这一点呢？可以分为以下两个阶段。互联网计算机网络是使用所谓的"链键"密码学创建的。这在很大程度上取决于阈值加密，其中组织成子网区块链的节点机器组协同管理单个"链键"，通常只有 48 字节。从本质上讲，这是链条的公钥，用户与这些链的交互上的相应签名会提示出 （a） 交互有效，（b） 链条正确。
---

### 阶段一:使互联网计算机智能合约能够调用以太坊智能合约

互联网计算机网络是使用所谓的"链键"密码学创建的。这在很大程度上取决于阈值加密，其中组织成子网区块链的节点机器组协同管理单个"链键"，通常只有 48 字节。从本质上讲，这是链条的公钥，用户与这些链的交互上的相应签名会提示出 （a） 交互有效，（b） 链条正确。
复杂的协议组件管理这些链键，即使构成链的节点来来去去，这些链键保持不变。不存在相应的"私钥"。相反，组成链条的节点保留"私钥共享"，这些共享可以用在等于"阈值"的某个数字中生成与公共链键相对应的签名。互联网计算机复杂的协议架构旨在管理这些密钥拜占庭故障容忍，并确保即使在托管区块链的节点发生变化时链键保持不变。
现在，Dfinity团队将在互联网计算机区块链上将此功能显示为智能合约。虽然互联网计算机严重依赖BLS阈值密码学，也正是密码学方案确保了比特币和以太坊余额以及智能合约，但Dfinity团队将引入对ECDSA阈值变种的支持，从本质上讲，这将使互联网计算机上的智能合约能够创建与这些链条上的公共密钥相关的比特币和以太坊交易，而无需持有相应的私钥。
为了使开发人员使用变得简单，Dfinity团队将在互联网计算机上创建一个特殊的"代理"智能合约，这将使创建比特币和以太坊交易变得像调用功能一样简单！这意味着互联网计算机上的智能合约将能够调用以太坊智能合约的功能。
在这个阶段，Dfinity团队应该注意到，ECDSA阈值根本不有效，并且完全不适合互联网计算机区块链协议中的一般使用。然而，互联网计算机区块链运行效率高，与这些网络必须支付的交易费用相比，创建比特币和以太坊交易所消耗的周期成本仍然相对较小。因此，即使构建以太坊交易的签名在计算上将非常昂贵，成本也不应成为问题。
现在，Dfinity团队必须考虑如何返回从互联网计算机到以太坊的结果，以及以太坊的智能合约将如何在互联网计算机上转化为智能合约。
以太坊智能合约能够调用到互联网计算机智能合约中，使以太坊能够返回结果
鉴于对以太坊网络当前的哈希速度的了解，只需通过"工作证明"检查哪些块的嵌入程度即可看到哪些块有效。即，如果社区中继将新的以太坊块复制到互联网计算机上的代理合约中，该合约将能够通过查看链中嵌入多少工作来检测块何时已最终确定。一旦合约能够看到一个块已经完成，它可以扫描块从以太坊智能合约到互联网计算机智能合约的calls，以及以前在其他方向调用的结果。然后，代理将调用互联网计算机上的智能合约，并将价值返回到以前称为以太坊的智能合约。当然，以太坊的智能合约也会通过以太坊的另一份代理合约，在互联网计算机上签订智能合约。
这种相对简单的架构，由链键启用，已经非常强大。最终用户与互联网计算机上的智能合约提供的 Web 体验交互，可以触发呼叫以太坊，结果可以返回给他们。此外，以太坊的智能合约可以呼叫互联网计算机上的智能合约，这些合约可能为他们执行计算复杂的任务，并代表他们维护和处理大量数据。无需区块链集线器、预言机或其他中介机构即可实现此目标。
然而，有一个领域需要改进。互联网计算机上的智能合约只能向最终用户显示以太坊的数据，即以太坊智能合约通过代理调用的函数呼叫推送给他们的数据。虽然这是可行的，但以太坊的任何功能通话都非常昂贵——需要几十美元，而在互联网上打电话的成本只有不到一分钱。这未能给予以太坊智能合约在所有情况下因互联网计算机的效率而提供的全部好处。为了解决最后一块问题，Dfinity团队必须进入第二阶段。

### 阶段二：降低调用以太坊的成本

要使以太坊智能合约的数据和功能以接近零的成本提供给互联网计算机智能合约，Dfinity团队必须在代理合约中保留以太坊当前状态的副本。即代理合约不仅必须扫描最终确定的以太坊区块以太坊块以获得交易数据，还必须使用收到的方块来维护和更新以太坊的完整状态的副本。一旦完成，互联网计算机智能合约将能够呼叫以太坊智能合约，这些合约不会修改其状态，成本接近于零。从本质上讲，它将在合约内部运行以太坊节点，就像在 AWS 上运行的 Infura 节点维护以太坊当前状态的副本。
第二阶段是一项更为复杂的工作，需要更长的时间，尤其是因为互联网计算机智能合约目前最多只能容纳4GB的内存页面，因此以太坊状态必须分片通过多个合约。但尽管如此，所提供的优势将是巨大的，因此，如果可能的话，当然应该这样做——一些以太坊开发人员已经在考虑实施这一点，并在代码方面取得了一些进展。
最后需要注意的是，一个凌乱的快捷方式是可能的，这将涉及使互联网计算机节点与以太坊节点交谈，以便他们可以提供一个低成本的桥梁查询以太坊状态。这里的挑战是，这将涉及信任谁运行以太坊节点，网络相互操作，这提供了远远低于只有智能合约参与的安全性。但是，如果有人想出一种改进安全性的方法，这可能会提供阶段 1.5 解决方案。

### 总结

区块链是新的互联网，一个伟大的第一步将是确保互联网计算机和以太坊可以像单一网络一样运作，提供它们在这两个网络中的相对优势的好处——这种整合可能证明是变革性的。



