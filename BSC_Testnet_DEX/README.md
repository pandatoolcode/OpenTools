# BSC Testnet DEX Tool

这是由一键发币平台[PandaTool](https://pandatool.org)开发的，基于 **BSC 测试网** 和 **PancakeSwap V2** 协议构建的 DEX 前端工具，用于演示 EVM 生态下的链上交互流程。

---

## 🔗 在线演示

https://pandatoolcode.github.io/OpenTools/BSC_Testnet_DEX/

---

## 🧰 适用网络与钱包

- **网络**：BSC Testnet（Chain ID: 97）
- **钱包**：MetaMask
- **浏览器**：https://testnet.bscscan.com
- **RPC**：https://data-seed-prebsc-1-s1.binance.org:8545

---

## 💧 水龙头

- **官方水龙头**：https://testnet.binance.org/faucet-smart
- **备用渠道**：BNB Chain Discord 的 `#testnet-faucet` 频道
- **跨链闪兑**：https://bridge.pandatool.org/
- **第三方购买**：https://www.bisell.site/buy/3

---

## 📄 核心合约地址

| 合约 | 地址 |
|------|------|
| V2 Router | 0xD99D1c33F9fC3444f8101754aBC46c52416550D1 |
| V2 Factory | 0x6725F303b657a9451d8BA641348b6761A6CC7a17 |
| WBNB | 0xae13d989daC2f0dEbFf460aC112a837C89BAa7cd |
| 测试 USDT | 0x66E972502A34A625828C544a1914E8D8cc2A9dE5 |

---

## ✨ 功能特性

### 兑换（Swap）
支持：

- BNB ↔ BEP-20
- BEP-20 ↔ BEP-20
- 有税代币（Fee-on-Transfer Token）交易

其中有税代币场景使用专门方法处理，适合验证 PancakeSwap V2 的实际兼容性。

### 添加流动性
支持：

- BNB + BEP-20
- BEP-20 + BEP-20

可用于测试池子创建、配对和 LP 初始化。

### 移除流动性
支持：

- LP 仓位扫描
- 按比例移除
- 从 LP 列表直接发起操作

### 池子信息查询
可查询任意交易对的：

- 储备量
- 占比
- 我的 LP
- 基础池状态

### 交易日志
实时记录：

- 交易状态
- 交易哈希
- 可跳转浏览器查看结果

### LP 一键扫描
自动扫描 Factory 中的所有池子，列出用户持有的 LP 仓位，便于集中管理。

### 有税代币支持
额外支持以下专用方法：

- `swapExactTokensForTokensSupportingFeeOnTransferTokens`
- `removeLiquidityETHSupportingFeeOnTransferTokens`

用于确保带手续费代币的交易与撤池流程正常运行。

---

## 🧪 使用提示

- 请先将钱包网络切换到 **BSC Testnet**
- 测试前建议先从水龙头领取少量 **tBNB**
- 所有测试网资产均无实际价值，仅用于开发和验证

---

## ⚠️ 免责声明

本项目仅用于开发、测试与学习，不构成任何投资建议、收益承诺或交易保证。链上操作存在风险，请自行评估并谨慎使用。

---

## 📄 License

MIT
