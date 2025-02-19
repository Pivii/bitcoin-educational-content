---
term: 术语： TIMESTAMP

---
时间戳（英文为 "timestamping"）是一种将精确的时间标记与事件、数据或信息关联起来的机制。在计算机系统的一般情况下，时间戳用于确定操作的时间顺序和验证数据随时间变化的完整性。

就比特币而言，时间戳用于确定交易和区块的时间顺序。区块链中的每个区块都包含一个时间戳，表明其创建的大致时间。中本聪甚至在他的白皮书中提到了 "时间戳服务器"，用来描述我们今天所说的 "区块链"。在比特币中，时间戳的作用是确定交易的时间顺序，以便在没有中央机构干预的情况下，确定哪笔交易在先。这种机制允许每个用户验证过去是否存在交易，从而防止恶意用户进行双重消费。中本聪在他的《白皮书》中用一句名言证明了这一机制的合理性："*确认不存在交易的唯一方法就是了解所有交易*"。这一标准是以 Unix 时间为基础制定的，Unix 时间表示自 1970 年 1 月 1 日以来经过的总秒数。

> ► *比特币的区块时间戳相对灵活，时间戳只需大于前 11 个区块时间的中位数（MTP），小于节点返回时间的中位数（网络调整时间）加 2 小时即可视为有效。