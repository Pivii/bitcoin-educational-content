---
term: UTXO SET

---
指在任何特定时刻所有现有 UTXO 的集合。换句话说，它是一个庞大的列表，列出了所有等待使用的比特币。如果把UTXO集合中所有UTXO的金额加起来，就得出了流通中比特币的总货币量。比特币网络中的每个节点都实时维护自己的UTXO集。当新的有效区块被确认时，它就会更新UTXO集，其中包含的交易会消耗UTXO集中的一些UTXO，并产生新的UTXO。

每个节点都会保存这组UTXO，以便快速验证交易中花费的UTXO是否合法。这样，它们就能发现并拒绝双重消费企图。UTXO集通常是人们对比特币去中心化担忧的核心，因为它的大小自然会迅速增加。由于UTXO集的一部分必须保存在RAM中，以便在合理的时间内验证交易，因此UTXO集会逐渐导致运行一个完整节点的成本过高。UTXO集对IBD（*初始块下载*）也有很大影响。可以放在 RAM 中的 UTXO 集越多，IBD 的速度就越快。在 Bitcoin Core 上，UTXO 集存储在名为"/chainstate "的文件夹中。

> ► *在英语中，"UTXO set "可译作 "UTXO set"。