# Telegram API 注册教程

[视频教程链接](https://www.youtube.com/watch?v=TWreKchDMWc&t=3s)

### 访问 Telegram 开发者平台

1. 打开浏览器，访问 [Telegram 开发者平台](https://my.telegram.org)。
2. 使用你的 Telegram 帐户登录。如果尚未登录，会提示你输入手机号码并进行身份验证。

### 创建应用

1. 登录成功后，你将进入 Telegram 开发者平台的主页面。
2. 点击页面右上角的 **“API development tools”** 链接。
3. 你将被引导到 **“Your applications”** 页面。在这里，点击 **“Create new application”** 按钮以创建一个新的应用。

### 填写应用信息

1. 在 **“Create new application”** 页面，填写以下信息：
   - **Application title（应用标题）：** 你的应用名称。
   - **Short name（简短名称）：** 应用的简短标识符。
   - **Platform（平台）：** 选择你的应用所在的平台（例如：Web, Desktop, Mobile）。
   - **Description（描述）：** 应用的简短描述（可选）。
   - **Website（网站）：** 你的应用或开发者的官方网站（可选）。
2. 完成填写后，点击 **“Create application”** 按钮。

### 获取 API_ID 和 API_HASH

1. 创建成功后，你将被重定向到 **“Your applications”** 页面。
2. 在你创建的应用下，你可以看到 **“API ID”** 和 **“API Hash”**。这两个值是你在使用 Telegram API 时必需的。

### 记录你的 API_ID 和 API_HASH

1. **API ID：** 这是一个数字 ID，用于唯一标识你的应用。
2. **API Hash：** 这是一个密钥字符串，用于验证你的应用的请求。

请妥善保管这两个信息，不要将其泄露给他人。

