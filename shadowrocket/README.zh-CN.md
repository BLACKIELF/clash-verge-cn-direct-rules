# Shadowrocket 小火箭规则

作者 / 水印：**blackielovelife**

这里提供一个 `.list` 版本：

- `国内联网规则-内部使用版.list`：适合自己用，除了公版规则外，额外加入 `.cn`、局域网和中国 IP 直连兜底。

## 使用方式

在 Shadowrocket 里添加远程规则 / 规则集时，使用 GitHub Raw 地址。

内部使用版：

`https://raw.githubusercontent.com/BLACKIELF/clash-verge-cn-direct-rules/main/shadowrocket/%E5%9B%BD%E5%86%85%E8%81%94%E7%BD%91%E8%A7%84%E5%88%99-%E5%86%85%E9%83%A8%E4%BD%BF%E7%94%A8%E7%89%88.list`

## 手动添加时怎么选

如果扫码后进入的是 Shadowrocket 的“规则”编辑页，请这样设置：

- 类型：`RULE-SET`
- 策略：`DIRECT`
- URL / 域名 / 规则集地址：填写上面的 Raw 地址

然后点保存。

注意：不要选择 `DOMAIN-SUFFIX`。`DOMAIN-SUFFIX` 是用来添加单个域名后缀的，如果把整条 Raw 链接填进去，小火箭会把链接当成一个域名规则，规则不会按预期生效。

如果二维码无法直接导入，请复制 Raw 地址到 Shadowrocket 的远程规则 URL 输入框。
