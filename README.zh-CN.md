# Clash Verge 国内网站直连增强规则

作者 / 水印：**blackielovelife**

这是一份给 Clash Verge / Mihomo 使用的国内常用网站直连增强模板。它的目标很简单：让小红书、B站、微博、新片场、百度、知乎、抖音等国内网站尽量走 `DIRECT`，减少“第一次打不开、刷新一下又好了”“登录信息获取失败”“点个人主页卡住”这类问题。

## 适合谁用

- 使用 Clash Verge 或 Clash Verge Rev 的用户
- 国内网站偶尔首开失败、刷新后恢复的用户
- 想让国内常用网站尽量直连、国外网站继续按原代理规则走的用户
- 想分享一份不含个人节点信息的公开规则模板给朋友的人

## 覆盖的网站

- 小红书 / Rednote
- Bilibili / B站
- 微博
- 新片场
- 百度 / 贴吧 / 百度网盘相关域名
- 知乎
- 抖音
- 微信 / 公众号 / 开放平台 / 微信支付 / 图片头像 CDN
- QQ、微信、淘宝、天猫、阿里 CDN、支付宝、京东等常见国内服务
- Loyalsoldier 的国内直连、局域网、中国 IP 等公开规则集

## 隐私说明

这个仓库不会包含你的个人 Clash 配置。

不会上传：

- 代理节点
- 机场订阅链接
- UUID
- 密码
- token
- 代理组名称
- Clash Verge 生成后的完整运行配置

仓库里只有公开规则源和域名规则，可以放心分享。

## 最简单用法

1. 打开 Clash Verge。
2. 进入 `Profiles`。
3. 找到当前配置的 `Merge` / `Profile Enhancement` / `配置增强`。
4. 复制 `clash-verge-merge-template.yaml` 里的内容。
5. 粘贴进去并保存。
6. 重新加载配置，或者重启 Clash Verge。

## 如果你已经有自己的 Merge 配置

如果你不想替换整份模板，可以只复制：

`rules/cn-stable-direct-patch.yaml`

把里面的规则放到你现有配置的 `prepend-rules:` 下面，位置尽量靠前。

## 文件说明

- `clash-verge-merge-template.yaml`：完整 Clash Verge 配置增强模板。
- `rules/cn-stable-direct-patch.yaml`：只包含国内常用网站增强直连规则，适合合并到已有配置。
- `COLLABORATION_RULES.zh-CN.md`：通用协作习惯和更新规则。
- `README.md`：英文说明。
- `README.zh-CN.md`：中文说明。

## 小提示

如果应用规则后，某个网站还是第一次打开失败、刷新后成功，可以尝试：

1. 重启 Clash Verge。
2. 关闭并重新打开浏览器。
3. 清理浏览器 DNS / socket 缓存。
4. 确认 Clash Verge 当前模式是 `Rule`，不是 `Global` 或 `Direct`。

这套规则是偏保守的：只把明确属于国内常用服务的域名强制直连，不会改变你的国外网站代理策略。
