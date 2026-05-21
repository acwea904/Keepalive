# VPS8 每日签到

## JS用法

1. 登录 https://vps8.zz.cd
2. 浏览器 DevTools（F12）→ Console 运行 document.cookie，复制 Cookie 字符串
3. 在 GitHub 仓库 Settings → Secrets and variables → Actions → 新建 Secret：
   - **名称:** VPS8_COOKIES
   - **值:** 粘贴上面的 Cookie 字符串
4. Actions 选项卡 → VPS8 每日签到 → Run workflow 测试

## PY用法-环境变量

- AI_API_KEY
- AI_BASE_URL：`https://api.openai.com/v1`，需要带上 `/v1`
- AI_MODEL_NAME
- VPS8_EMAIL
- VPS8_PASSWORD
- TG_CHAT_ID
- TG_BOT_TOKEN

## 自动运行

默认每天 **北京时间 08:00**（UTC 00:00）自动签到。
