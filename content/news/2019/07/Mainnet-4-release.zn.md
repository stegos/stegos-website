---
author: "Vladimir Lebedev"
date: 2019-08-07
linktitle: 主网预览 4 20190807
title: "主网预览 4"
description: "这是即将推出的Stegos主网的第四个预览版本。"
metaTitle: "主网预览 4"
metaDescription: "这是即将推出的Stegos主网的第四个预览版本。"
categories: [ "开发" ]
tags: ["stegos", "周报", "技术"]
weight: 7
draft: false
---
​
Stegos打造前沿科技，从而保护您的隐私安全，避免被其他人窥视，因此你会感到非常给力以及安全。
​
这是一个修复错误的版本, 自[主网预览 3](https://github.com/stegos/stegos/releases/tag/v0.10)以来多出了100多个错误修复程序。
​
### Stegos v0.11中的新增内容:
​
- 提高了Snowball混币协议的整体稳定性和性能，现在Snowball即使在3G/4G这样的慢速移动数据连接环境下也能可靠运行。
- 调整核心区块链常数和限制，以达到通胀目标，现在每隔6-8秒产生一个新区块。
- 将HashCash替换为VDF用于网络授权协议，使网络授权延迟更具可预测性。
- 节点添加自动re-staking，以允许节点在没有电子冷钱包密钥的情况下工作。
- 重新设计了交易跟踪和付款历史记录，修复了内部质量保证期间发现的几个问题。
- 重新安排数据目录布局并更改默认路径以满足Linux和Mac准则。
- 为Node和CLI添加了新的命令行和配置选项。
- 在命令行客户端中过滤掉扰人的通知。
- 改进了WebSocket API的可用性。
​
请参考[Sprint 20](https://github.com/stegos/stegos/milestone/21?closed=1) and [Sprint 21](https://github.com/stegos/stegos/milestone/22?closed=1) GitHub上的里程碑获取已修复错误的完整列表。
​
### 入门教程
​
#### 运行节点
​
如果您安装了Mainnet Preview 3，请停止运行节点并清理数据目录：
​
```
rm -rf ~/.local/stegos ~/.config/stegos
```
​
下载并运行Stegos节点:
​
**Linux 64-bit:**
​
```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.11/stegosd-linux-x64 -o stegosd
chmod a+x stegosd
./stegosd
```
​
**macOS 64-bit:**
​
```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.11/stegosd-macos-x64 -o stegosd
chmod a+x stegosd
./stegosd
```
​
在第一次运行时，节点将在以下路径中创建一个数据目录 `$HOME/.local/share/stegos` on Linux or `$HOME/Library/Application Support/stegos` 在Mac上，该目录的结构如下:
​
​
```
    ├── accounts/  <!-- Accounts
    │   ├── 1
    │   │   ├── account.pkey <!-- Account #1 public key (address)
    │   │   ├── account.skey <!-- Account #2 secret key (address)
    │   │   └── history/     <!-- Payment History (RocksDB)
    │   └── 2
    │       ├── account.pkey <!-- Account #1 public key (address)
    │       ├── account.skey <!-- Account #2 secret key (address)
    │       └── history/     <!-- Payment History (RocksDB)
    ├── api.token            <!-- Generated API Token
    ├── chain/               <!-- Blockchain (RocksDB)
    ├── network.pkey         <!-- Ephemeral network (consensus) public key.
    ├── network.skey         <!-- Ephemeral network (consensus) secret key.
```
​
节点将开始与网络同步，并打印大量INFO消息，其中包含有关同步状态的调试信息。
​
新节点没有默认帐户。如要创建新帐户，请使用命令行客户端连接到节点。
​
#### 连接到节点
​
下载并运行命令行客户端。
​
Linux 64-bit:
​
```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.11/stegos-linux-x64 -o stegos
chmod a+x stegos
./stegos
```
​
macOS 64-bit:
​
```bash
curl -L https://github.com/stegos/stegos/releases/download/v0.11/stegos-macos-x64 -o stegos
chmod a+x stegos
./stegos
```
​
命令行客户端将尝试连接到本地节点并进行打印 `stegos>` 提示。想要获得帮助，请在提示符下输入 `help` 命令。默认情况下, 客户端从当前目录中的 `api_token.txt` 文件中读取API代币，并尝试连接到默认 (`127.0.0.1:3145`) 节点地址。请查阅 `stegos --help` 来覆写这些选项。
​
#### 账户使用
​
输入 `create account` 创建新账户。系统会要求您输入密码，此密码在本地用于加密磁盘上的数据，请记住它。
​
输入 `show recovery` 获取24个字的恢复短语。此恢复短语是您的密钥的编码表示，请记下来并保存在安全的地方，没有其他密码恢复机制。
​
输入 `recover account` 从已保存的24个字的恢复短语中还原帐户。
​
输入 `show accounts` 列出可用账户。
​
输入 `use ACCOUNT_ID` 在CLI中切换活动帐户。
​
输入 `show balance` 获取余额。
​
输入 `pay RECIPIENT AMOUNT` 发送资金。
​
输入 `show history 15m` 查看已创建交易和付款历史的状态。
​
### 反馈
​
请加入我们的[电报群](https://stg.to/tgcch)来获取测试网代币。
订阅官方[电报公告频道](https://stg.to/tgnch)来获取最新的消息。
