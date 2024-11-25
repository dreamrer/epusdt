## Epusdt

## 安装须知

- 本项目修改自 https://github.com/fmnx/epusdt
- 安装过程大致与原版 epusdt 相同，但是需要替换 `static` `.env` `epusdt`。
- 数据库结构有修改，[请用这个文件](./sql/v0.0.1.sql)
- 兼容原版的 epusdt 插件（默认收 `polygon` 链，使用 `channel` 参数可同时收 `trc20`）

### Polygon Scan API

Polygon 链收款需要在 .env 中填写 `polygon_api` ，否则可能会被 polygonscan 限制查询区块链查询。详情请看 `.env.example` 文件

## 教程：

- 开发者接入`epusdt`文档👉🏻[开发者接入epusdt](wiki/API.md)

注意：项目中的其他教程和插件来自原版epusdt，不一定正确。

### URL 基本格式：
https://域名/api/v1/order/create-transaction
https://域名/api/v1/order/create-transaction?channel=polygon&exchange_rate=7.2
