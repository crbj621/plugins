# 积分与 Token 余量 · Credit Balance & Tokens

<img src="https://raw.githubusercontent.com/crbj621/plugins/page-credit-balance-v1.1.0/packages/page-credit-balance/page/icon.png" width="96" alt="积分与 Token 余量插件图标">

一个 Magpie 页面插件。把不同供应商的余额折算成你熟悉的积分，看看指定模型在高峰和低峰分别还能用多少 Token，并查清近几天的积分花在哪里。

[下载最新版](https://github.com/crbj621/plugins/releases/latest) · [中文详细说明](https://github.com/crbj621/plugins/blob/add-page-credit-balance/packages/page-credit-balance/README.zh-CN.md) · [English guide](https://github.com/crbj621/plugins/blob/add-page-credit-balance/packages/page-credit-balance/README.md) · [社区收录进度](https://github.com/magpie-community/plugins/pull/1288)

## 能做什么

| 功能 | 用法 |
| --- | --- |
| 折合积分 | 选 WorkBuddy 等供应商和一个型号当基准。按各家同一时段的费率，把余额折成基准供应商的积分。高峰和低峰各有一个合计。 |
| 按型号看 Token | 手动勾选各家的对应型号，可以选多个别名。同一个账户的余额只计一次。可查看单家余量，也可勾选多家合计。 |
| 查积分消耗 | 查看滚动 24 小时、北京时间最近 7 日或 30 日的消耗。展开供应商可按型号查看，并区分实际扣分、估算和暂时无法归到型号的部分。 |

例如，某家有 200 积分，假设高峰每百万 Token 扣 4 积分、低峰扣 2 积分，分别约能用 5,000 万和 1 亿 Token。再按基准供应商对应时段的费率换算，就得到高峰和低峰的折合积分。详细说明里有完整算例与费率来源。

## 安装

需要 **Magpie 0.1.4402 或更新版本**。在[发布页](https://github.com/crbj621/plugins/releases/latest)下载 `.tgz` 安装包，解压后，在包含 `package` 子目录的位置执行：

```sh
magpie plugin add ./package
```

打开 Magpie 侧栏的 **积分与 Token 余量**。第一次使用时，先选基准供应商或目标型号，再展开各家勾选相同模型。插件在本机读取 Magpie 的额度和用量记录。

## 维护与标星

觉得好用，登录 GitHub 后可点本仓库右上角的 **Star**。反馈消耗差异时，提供供应商、模型、统计时间和页面显示的数据来源，便于对照。

[插件源码](https://github.com/crbj621/plugins/tree/add-page-credit-balance/packages/page-credit-balance) · [上游 Magpie 社区插件目录](https://github.com/magpie-community/plugins)
