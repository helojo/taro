---
title: Taro.startLocationUpdateBackground(option)
sidebar_label: startLocationUpdateBackground
id: version-2.0.3-startLocationUpdateBackground
original_id: startLocationUpdateBackground
---

开启小程序进入前后台时均接收位置消息，需引导用户开启[授权]((open-ability/authorize#后台定位))。授权以后，小程序在运行中或进入后台均可接受位置消息变化。

**注意**
- 安卓微信7.0.6版本，iOS 7.0.5版本起支持该接口
- 需在app.json中配置requiredBackgroundModes: ['location']后使用
- 获取位置信息需配置[地理位置用途说明](https://developers.weixin.qq.com/miniprogram/dev/reference/configuration/app.html#permission)。

> [参考文档](https://developers.weixin.qq.com/miniprogram/dev/api/location/wx.startLocationUpdateBackground.html)

## 类型

```tsx
(option?: Option) => void
```

## 参数

### Option

| 参数 | 类型 | 必填 | 说明 |
| --- | --- | :---: | --- |
| complete | `(res: CallbackResult) => void` | 否 | 接口调用结束的回调函数（调用成功、失败都会执行） |
| fail | `(res: CallbackResult) => void` | 否 | 接口调用失败的回调函数 |
| success | `(res: CallbackResult) => void` | 否 | 接口调用成功的回调函数 |

## API 支持度

| API | 微信小程序 | H5 | React Native |
| :---: | :---: | :---: | :---: |
| Taro.startLocationUpdateBackground | ✔️ |  |  |
