# Bifrost Subgraph 开发者使用说明

欢迎使用 Bifrost Subgraph!本文档将指导您如何创建、部署和查询这个 subgraph。

## 先决条件

在开始之前,请确保您已经:

- 注册了一个 Bifrost 账户并获得了 API 密钥。
  - 请访问以下链接之一并填写表格以申请 API 密钥:
    - [https://forms.gle/tijPPdW37hFX6QFG9](https://forms.gle/tijPPdW37hFX6QFG9)
- 安装了 Graph CLI。
- 安装了 Yarn 包管理器。

## 创建 Subgraph

1. 选择一个 subgraph 名称,格式为 `<用户名>/<subgraph名称>`,例如 "alice/mysubgraph"。
   - `<用户名>`:这是您在 Bifrost 上的用户名。
   - `<subgraph名称>`:这是您为 subgraph 选择的具体名称,通常反映 subgraph 的功能或其索引的智能合约。

2. 在终端中运行以下命令,将 `{apikey}` 替换为您从上述链接申请获得的 Bifrost API 密钥,将 `<用户名/subgraph名称>` 替换为您选择的 subgraph 名称:

```bash
graph create --node https://bifrost.bfno.de/{apikey} <用户名/subgraph名称>
