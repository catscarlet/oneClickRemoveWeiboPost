# oneClickRemoveWeiboPost 一键删除微博

基本功能就是，在新浪微博(weibo.com)我的主页页面列表页，为每条微博增加了一个 **[删除]** 按钮，点一下这个按钮，就立即删除这条微博，没有提示框，没有确认，秒杀，一刀切，不含糊。免除 **新浪人为设置的多次瞄准和点击才能删除粉丝的麻烦**。

## 安装

Chrome用户需要安装 **<暴力猴 扩展程序>**：[谷歌商店链接](https://chrome.google.com/webstore/detail/violentmonkey/jinjaccalgkegednnccohejagnlnfdag?hl=zh-CN)，[GitHub链接](https://github.com/violentmonkey/violentmonkey/releases/latest)。

脚本安装地址：<https://greasyfork.org/zh-CN/scripts/32313-oneclickremoveweibopost>，点击页面上的 **安装此脚本** 即可。

其他浏览器未经过测试，请尝试 Tampermonkey  Greasemonkey、或同类扩展。

## 反馈

关于使用的反馈，可以发送到 greasyfork对应项目页、GitHub项目页 或 我的博客。有时间的话我会看的，有时间的话。

欢迎对项目进行 Pull Request。

## 兼容性

### 扩展

与暴力猴 v2.8.0 兼容。

其他扩展程序未实际测试。

### 其他脚本

与 Yet Another Weibo Filter 完全兼容。

## 已知问题

1. 因为列表是延迟载入的，而且微博页面地址也无法固定，不知道怎么解决，所以使用了轮询。如果对性能有要求，建议在不使用的时候暂停脚本。
2. 不仅是自己的个人页面，在其他人的个人页面也会显示 **[删除]** 按钮，这个，当然你是删不掉的。新浪会提示 "系统繁忙，请稍候再试吧。"，当然，明显不是这个理由。
3. 买了微博会员并使用了卡片背景的用户，页面上可能不会正确显示 **[删除]** 按钮。反正我没有会员，我也不想冲会员，会员用户如果想使用的话……你是花了钱的用户，有事找微博官方吧，我又没有钱……

## 安全性

### 信息收集

脚本不会以任何方式收集您的任何个人信息。但您使用脚本过程中产生的网络访问可能会被您的网络提供商以及对应网站所记录。

### 本地存储

脚本不会存储您的任何操作记录。如果您删掉了某条微博，那就删掉了，不会记录是谁被删掉了，什么时候被删掉了，也没有恢复的办法

打开浏览器控制台，可以看到被删掉的DOM信息，可用于调试和检查。

## 代码

GitHub：<https://github.com/catscarlet/oneClickRemoveWeiboPost>
