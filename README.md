---
layout: default
title: Home
---

# 北京一卡通AppJS交互方法汇总1

## 一、NFC相关
### 1.1  getNfcCardParams
获取NFC卡片充值参数，仅支持iOS端调用，客户端支持版本为6.0.0.0~最新

| 传参 | 注释 | 回参 | 注释 |
|------|------|------|------|
|   无   |      |  params   |成功返回对象
|      |      |    result  | 失败返回0

### 1.2 nfcExecuteApdu
NFC执行指令，仅支持iOS端调用，客户端支持版本为6.0.0.0~最新
| 传参 | 注释 | 回参 | 注释 |
|------|------|------|------|
|   execute   |  指令    |  execute   |执行结果|

### 1.3 startNFCScan

NFC开始贴卡扫描，仅支持iOS端调用，客户端支持版本为6.0.0.0~最新

| 传参    | 注释     | 回参      | 注释            |
| ------- | -------- | --------- | --------------- |
| message | 显示文案 | isSuccess | 结果 1成功0失败 |

### 1.4 endNFCScan

NFC结束贴卡扫描，仅支持iOS端调用，客户端支持版本为6.0.0.0~最新

| 传参    | 注释     | 回参      | 注释            |
| ------- | -------- | --------- | --------------- |
| message | 显示文案 | isSuccess | 结果 1成功0失败 |

