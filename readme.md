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

消息中的按钮使用 QQ 官方机器人的自定义键盘（`keyboard.content.rows`），与 Markdown 正文、图片同属一条 `msg_type: 2` 消息，因此头像、文字与按钮会显示在同一张卡片内；无需在 [QQ 开放平台](https://q.qq.com/) 申请按钮模板 ID，按钮文字与指令也可根据配置动态生成。

头像使用 Markdown 图片语法并显式声明宽高（统一为 100px），避免手机端因缺少宽高而把图片显示为 `[avatar]` 占位。

私聊场景不会发送按钮，也不会 @ 用户。

## 致谢

本项目基于 [idranme/koishi-plugin-waifu](https://github.com/idranme/koishi-plugin-waifu) 二次开发，遵循 MIT License。

