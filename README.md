屏蔽了中国大陆 IP 访问的区块链产品域名列表

---

一些加密货币服务和 app 出于规避风险考虑，主动对中国大陆用户停用了部分或全部功能。对于非中心化服务来说想要精准屏蔽指定地区用户是难以实现的，它们绝大多数只是通过检查客户端 IP 来执行屏蔽策略。

越过那道墙对区块链玩家是基本技能，途径繁多大家各显神通，出于体验考虑，我们通常会让代理常开并通过配置文件来自动化地判断网络请求应该走代理还是直接访问。对于没有显式配置的域名，常见的兜底策略是本地代理工具检查目标服务 IP，非大陆的一律走代理，但某些产品本身服务就部署在大陆或者拥有大陆节点，这样的兜底策略并非全部有效，还是需要手动添加此类域名。

这个文档汇总了屏蔽大陆 IP 或者被墙刻意阻断的域名，方便大家快速把它们添加到配置文件中，顺带提供一份我自己正在使用的 Surge 规则配置样例。这里不精准列举服务使用的所有子域名，没有必要且需要持续维护，而是建议对这些域名按尾缀全量匹配，例如 binance.com 意味着 binance.com 和 *.binance.com（通配符匹配）都应该被纳入代理规则。

欢迎大家 PR 添加更多域名和其他代理工具的规则样例。

## 产品和域名列表

| 产品          | 域名                                                         |
| ------------- | :----------------------------------------------------------- |
| Binance       | binance.com<br />binance.cloud                                                 |
| OKEX          | okex.com<br />okx.com                                  |
| Bybit          | bybit.com                                                     |
| Huobi          | huobi.com                                                     |
| DeBank        | debank.com                                                   |
| ZKSwap        | zks.org<br />zks.app<br />zkswap.info                        |
| Loopring      | loopring.org<br />loopring.io<br />loopring.network<br />api.loopring.network<br />ipdata.co |
| CoinGecko     | coingecko.com                                                |
| CoinMarketCap | coinmarketcap.com                                            |
| imToken       | token.im<br />tongke.top<br />tongke.co<br />tokenlon.im                    |
| OneKey        | onekey-asset.com<br />onekey.so                              |
| 区块链123     | qkl123.com                                                   |
| TradingView  | tradingview.com                                                  |
| 非小号        | feixiaohao.co<br />feixiaoquan.com<br />fxhapp.com                                                   |
## 致谢
[中国涉加密货币机构与项目陆续宣布关停与限制 —— 吴说](https://www.wu-talk.com/html/supervise/2021_2042.html)