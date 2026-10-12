# clash-hot-countries

每日自动扫描并更新的**热门国家免费代理** Clash / Mihomo 订阅，方便做链式代理（`dialer-proxy` / 前置代理）。

> 免费节点随时会挂，仅供临时使用；不要用它们登录重要账号。普通 HTTP/SOCKS 代理不加密。

## 订阅链接（推荐 jsDelivr）

中文节点名：

```
https://cdn.jsdelivr.net/gh/yuluo688/clash-hot-countries@master/clash-hot-countries-zh.yaml
```

英文节点名：

```
https://cdn.jsdelivr.net/gh/yuluo688/clash-hot-countries@master/clash-hot-countries-en.yaml
```

默认文件（与中文版相同）：

```
https://cdn.jsdelivr.net/gh/yuluo688/clash-hot-countries@master/clash-hot-countries.yaml
```

若 `@master` 被 CDN 缓存成旧内容，把链接里的 `@master` 换成最新 commit 短哈希即可。

GitHub raw（国内常被重置，不推荐）：

```
https://raw.githubusercontent.com/yuluo688/clash-hot-countries/master/clash-hot-countries-zh.yaml
https://raw.githubusercontent.com/yuluo688/clash-hot-countries/master/clash-hot-countries-en.yaml
```

## 仓库文件

| 文件 | 说明 |
|------|------|
| `clash-hot-countries-zh.yaml` | 节点名为中文国名，如 `美国-HTTP-…` |
| `clash-hot-countries-en.yaml` | 节点名为英文代号，如 `US-HTTP-…` |
| `clash-hot-countries.yaml` | 默认中文版（同上） |

两份里的节点内容相同，只是显示名语言不同。

## 覆盖国家

美国、日本、新加坡、香港、韩国、德国、英国、法国、土耳其、印度、印尼、台湾、马来西亚、泰国、荷兰、加拿大、澳大利亚、巴西。

## 更新频率

每天北京时间约 **05:02**、**15:02** 自动扫描并 push。某国可能扫不到可用节点，列表会为空或变少。

## 筛选标准（概要）

- 出口 IP 地理与标称国家一致  
- HTTPS 可连通  
- 约 30–40 秒内多次探测多数通过  
- 优先 VLESS / SS / VMess / Trojan；没有再用无密码 HTTP / SOCKS  

## 使用提示

1. 在 Clash / Mihomo 客户端添加上述订阅 URL，定时更新。  
2. 链式代理时，可将这些节点作为出站或 `dialer-proxy`。  
3. 节点大量失效时，等下一轮自动更新，或手动再扫。  

## License

内容来自公开免费代理列表，仅作学习与测试。使用风险自负。
