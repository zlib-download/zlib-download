# zlib.download Project

zlib.download 是一个代理访问 zlibrary API 的工具。能够提供与原 zlibrary 网站基本一致的下载体验。

**zlib.download 服务器本身不存储任何数据。所有内容均从 zlibrary 服务器实时获取并转发。**

## 项目介绍

zlib.download 最初由 zhelper 小组开发，作为 zhelper V4 的下载组件提供服务。zhelper V4 于 2022.11.23 上线，截止 2022.11.19 为止，提供了 110M/s 峰值下载速度的下载服务，以及共计 40T 的数据传输。

但由于直接提供下载服务风险过大且不可控制。zhelper 小组于 2022.11.20 暂停了 zhelper V4 的下载。并于同日启动 zlib.download 网址，希望能够将原 zhelper V4 核心代码可靠地分布式部署，分散风险，提高可用性。

## 使用说明

1. 从搜索网页获取所需要下载书籍的信息
```
从 TOR 官网获取：搜索完成后，在详情界面，复制链接如 http://bookszlibb74ugqojhzhg2a63w5i2atv5bqarulgczawnbmsb6s6qead.onion/book/11651373/1132ee
从 zhelper 获取：搜索完成后，在下载界面，复制链接如 https://download.v4.zhelper.net/download/3511909/db1f53
从 clibrary 获取：搜索完成后，在详情界面，复制链接如 https://clibrary.top/book/3511911/f37da4
```
2. 注意其中共同的特点：最后以 数字/字符串 的形式结尾。如 3511909/db1f53 或者 3511911/f37da4
3. 然后，请访问 [替换成可用的服务器域名]/download/[替换成上一步的数字]/[替换成上一步的字符串] 即可
4. 如果需要使用自己的额度，请使用 [替换成可用的服务器域名]/download/[替换成上一步的数字]/[替换成上一步的字符串]/[替换成remix_userid]/[替换成remix_userkey]

## 部署说明

一方面考虑到 zlibrary 接口存在被恶意利用的可能性，另一方面考虑到 zlibrary 服务器本身的负担，我们决定暂时不对代码核心部分进行开源。但是，您仍然可以通过提交 issue 或者 discussion 的方式向我们申请部署。我们将会考察您的 Github 基本信息，以确保您不会将本项目用于某些恶意用途。

申请通过后，我们将给出详细的部署教程。

```
是否熟悉 Docker：（是/否）
可以提供的下载服务器：（一一列出，如 4C/16G/1G@不限 独立服务器，TOR 不算！！！，需要你有一台能够部署 Docker 的服务器）
是否自带域名：（是/否）
是否需要接入公共账号：（是/否）
是否参加图书馆备份项目：（是/否）
我承诺不将本项目源码用于盈利：（必须回答是）
我已知晓潜在的风险：（必须回答是）
我承诺不传播本项目源码：（必须回答是）
```

## 公共接口与致谢

test1.zlib.download 测试接口，感谢 zhelper 小组提供测试接口。
zlibdown.ga 感谢 Royce rii 提供此接口。

