# @forgetmelody/koishi-plugin-waifu

[![npm](https://img.shields.io/npm/v/@forgetmelody/koishi-plugin-waifu?style=flat-square)](https://www.npmjs.com/package/@forgetmelody/koishi-plugin-waifu)

娶群友！来寻找你今日的群友老婆吧！

## 安装

```sh
npm install @forgetmelody/koishi-plugin-waifu
```

## 可选的

### 特性

* 避免用户抽中他人的老婆
* 只让用户抽中活跃的群友
* 适配 QQ 官方机器人 Markdown 消息与按钮，输出使用 @ 用户替代引用回复

### 指令

* 强娶
* 求婚
* 离婚
* 换老婆

## QQ 官方机器人

插件会自动识别 `qq` 平台的群聊消息，改用 Markdown 消息发送，并用 `<qqbot-at-user>` 原生标签 @ 用户（替代引用回复）。

按钮有两种显示方式：

| 配置 | 效果 |
| --- | --- |
| `qqKeyboardTemplate` 留空 | 使用自定义按钮，按钮会以独立气泡显示在卡片下方 |
| 填写按钮模板 ID | 使用按钮模板，按钮嵌在 Markdown 卡片内 |

使用按钮模板前需要在 [QQ 开放平台](https://q.qq.com/) 创建按钮模板，按钮动作类型选择「指令」，`data` 分别填写 `娶群友` 和 `离婚`，然后把模板 ID 填入插件配置。

> 模板按钮的文字是固定的，无法由代码动态生成；如果未启用 `divorce`，模板中请不要包含「离婚」按钮。

私聊场景不会发送按钮，也不会 @ 用户。

## 致谢

本项目基于 [idranme/koishi-plugin-waifu](https://github.com/idranme/koishi-plugin-waifu) 二次开发，遵循 MIT License。

