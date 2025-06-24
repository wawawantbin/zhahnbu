# zhahnbu
## 快速开始

1. **克隆项目**
   ```bash
   git clone <your-repo-url>
   ```

2. **打开微信开发者工具**
   - 选择 `miniprogram` 目录作为项目根目录导入
   - 使用你自己的小程序 AppID

3. **配置 Moonshot API**
   - 在 `components/chat-bot/chat-bot.js` 中填写你的 Moonshot API Key
   - 确保微信小程序后台已将 `https://api.moonshot.cn` 配置为 request 合法域名

4. **编译并运行**
   - 点击“编译”按钮，预览小程序

## Moonshot API 对接说明

- API 地址：`https://api.moonshot.cn/v1/chat/completions`
- 请求方式：POST
- 请求头需包含：
  - `Content-Type: application/json`
  - `Authorization: Bearer <你的API密钥>`
- 每个页面可通过 `systemPrompt` 属性设置不同的机器人性格

## 个性化机器人示例

```xml
<!-- 塔罗牌占卜 -->
<chat-bot
  title="塔罗牌占卜"
  icon="🔮"
  placeholder="请输入你想占卜的问题..."
  welcome="欢迎来到塔罗牌占卜世界！"
  systemPrompt="你是一个神秘、温柔、善于安慰用户的塔罗牌占卜师，请用诗意和鼓励的语气回答用户。"
/>
```

## 注意事项

- **API Key 请勿泄露**，如需上线建议用云函数中转
- **本地开发如遇“域名不在白名单”问题，请在微信公众平台后台配置合法域名**
- **如需自定义风格，可修改 chat-bot 组件的样式文件**

## License

MIT
