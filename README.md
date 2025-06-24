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

5. **配置环境变量**
   - 复制 `.env.example` 为 `.env`
   - 填写你的 API Key 等配置信息

## Moonshot API 对接说明

