---
term: BIP49

---
BIP49 是一个信息性 BIP，介绍了用于在高清钱包中生成嵌套 SegWit 地址的派生方法。建议的派生路径遵循 BIP43 和 BIP44 的标准，并在目标深度处添加索引 `49'`（加固派生）。例如，P2SH-P2WPKH 账户的第一个地址将由以下路径推导得出：`m/49'/0'/0'/0/0`.嵌套 SegWit 脚本是在 SegWit 推出时发明的，目的是为了方便采用。这些脚本允许使用这一新标准，甚至在尚未与 SegWit 原生兼容的钱包上使用。