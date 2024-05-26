<p align="center">
  <a href="https://www.github.com/hoshinonyaruko/auto-withdraw-advideo">
    <img src="img/1.jpg" width="200" height="200" alt="auto-withdraw-advideo">
  </a>
</p>

<div align="center">
# QQ群二维码视频广告过滤器

_✨ 适用于Onebotv11的一键端 ✨_  
</div> 

---

## 介绍

最近实在是受够了,那些QQ群半夜混进的小号,发送的只有几秒钟的视频二维码广告。

把群环境弄得一团糟,而且基本都是出现在半夜3点左右,QQ的Q群管家也无法识别1-3秒的视频情色二维码广告.

本项目旨在提供一个简单而有效的解决方案，自动识别并撤回群内的短视频广告，确保群聊的清洁和用户的不被打扰。

目前采用判断视频长度的方案,可能会有误伤,

本工具能够识别并判断配置中指定秒数以内的视频（时间长度可自定义），让半夜的视频广告无处遁形，即便他们混进了群里也无济于事。

## 主要功能
- **自动撤回短视频广告**：自动检测并撤回指定秒数以内的视频。
- **配置极简**：用户只需要简单配置即可开始使用。
- **支持Onebot v11标凈**：适配使用Onebot v11标准的机器人。

## 用法
要使用本工具，你需要进行简单的配置：

- `port`: 例如 `"28800"` 表示监听 `ws://127.0.0.1:28800`。
- `video_second_limit`: 例如 `5` 代表自动撤回5秒以内的视频。

确保机器人连接上这个反向WebSocket地址，并设置机器人为群管理员，即可开始自动工作。

### 示例配置
```yaml
port: "28800"
video_second_limit: 5
```

## 使用方法
1. 确保机器人使用的是支持Onebot v11的实现。
2. 配置机器人连接到指定的WebSocket地址。
3. 将机器人设置为群管理员。
4. 调整`video_second_limit`配置以撤回指定长度的视频广告。

## TODO
- 拦截并撤回更多类型的广告。
- 实现进群验证码功能。
- 自定义撤回规则。
- 撤回卡片信息等。
- 找到视频广告更多特征,更精准的识别视频广告.

## 贡献
欢迎对本项目提出改进建议或直接贡献代码，一起打造更清洁的聊天环境。