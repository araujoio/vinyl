# 配置指南

如何为 Vinyl 配置环境变量与外部服务集成。

### 环境配置

在项目根目录下创建 `.env` 文件并添加以下变量：

```env
YOUTUBE_API_KEY=your_youtube_api_key_here
```

#### 获取 YouTube API 密钥

1. 访问 [Google Cloud Console](https://console.cloud.google.com/) 并前往 **API 和服务**。

   ![Google Cloud Console - APIs & Services](../../../assets/configuration-step-01.png)

2. 在左侧菜单栏中点击 **库**。

   ![Google Cloud Console - Library](../../../assets/configuration-step-02.png)

3. 搜索 **YouTube Data API v3**，在目录中选中并点击 **启用**。

   ![Google Cloud Console - Enable YouTube Data API v3](../../../assets/configuration-step-03.png)

4. API 启用后，前往左侧的 **凭据**，点击 **+ 创建凭据** 并选择 **API 密钥**。

   ![Google Cloud Console - Credentials](../../../assets/configuration-step-04.png)

5. 在 **创建 API 密钥** 面板中完成设置并点击 **创建**：
   - **名称：** 输入便于识别的名称（如 `vinyl-key`）。
   - **可访问的 API：** 在 API 限制中勾选 **YouTube Data API v3**。
   - **应用限制：** 保持为 **无**。

   ![Google Cloud Console - Create API Key](../../../assets/configuration-step-05.png)

6. 复制生成的 API 密钥并将其配置到 `.env` 文件的 `YOUTUBE_API_KEY`：

   ```env
   YOUTUBE_API_KEY=your_actual_api_key_here
   ```

> [!TIP]
> Google Cloud 为 YouTube Data API 提供了充裕的每日免费配额，足以满足本地开发与个人日常使用需求。

<div align="left">
  <a href="../01-installation/README.md"><strong>← 上一步：安装</strong></a>
</div>

---

*免责声明：本文档由内部人工智能自动化流程翻译，可能包含错误或不准确之处。英文原始文档为官方权威参考来源。*
