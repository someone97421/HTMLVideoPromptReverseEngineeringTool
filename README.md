# 🎬 视频/图片反推器 | Video/Image Reverse Prompt Generator

一款纯前端的多模态 AI 提示词反推工具，支持图片和视频的 AI 分析与提示词生成。

A pure frontend multimodal AI prompt reverse engineering tool that supports image and video analysis with prompt generation.

---

## ✨ 功能特性 | Features

- 📷 **图片上传** - 支持多张图片拖拽、粘贴上传（JPG, PNG, GIF, WebP）
- 🎬 **视频上传** - 支持视频文件上传，自动获取服务器 URL（单文件 ≤20MB）
- 🔗 **视频 URL** - 支持直接输入视频链接进行反推
- 🤖 **系统预设** - 内置视频/图片反推提示词模板，支持自定义预设
- ⚙️ **灵活配置** - 支持配置 OpenAI 兼容 API 的 Base URL、API Key、模型参数
- 📝 **流式输出** - 支持流式响应，实时查看生成结果
- 📚 **历史记录** - 本地保存历史记录，支持一键恢复和复制
- 🌙 **深色主题** - 优雅的深色 UI 设计

---

- 📷 **Image Upload** - Drag & drop or paste multiple images (JPG, PNG, GIF, WebP)
- 🎬 **Video Upload** - Upload video files and auto-get server URL (single file ≤20MB)
- 🔗 **Video URL** - Directly input video links for reverse prompting
- 🤖 **System Presets** - Built-in video/image reverse prompt templates with custom preset support
- ⚙️ **Flexible Config** - Configure OpenAI-compatible API Base URL, API Key, model parameters
- 📝 **Streaming Output** - Stream responses for real-time result viewing
- 📚 **History** - Local history storage with one-click restore and copy
- 🌙 **Dark Theme** - Elegant dark UI design

---

## 🚀 使用方法 | Usage

1. 打开 `index.html` 文件或部署到任意静态服务器
2. 在「设置」面板中配置你的 API 信息（Base URL 和 API Key）
3. 选择「系统提示词」预设（可选）
4. 上传图片或视频，或直接输入视频 URL
5. 点击「提交」按钮，等待 AI 返回结果

---

1. Open `index.html` or deploy to any static server
2. Configure your API info in the "Settings" panel (Base URL and API Key)
3. Select a "System Prompt" preset (optional)
4. Upload images or videos, or directly input video URLs
5. Click "Submit" and wait for the AI response

---

## ⚙️ 配置说明 | Configuration

| 配置项 | 说明 | Default |
|--------|------|---------|
| Base URL | API 基础地址 | `https://ai.t8star.cn/v1` |
| API Key | 你的 API 密钥 | - |
| 模型名称 | AI 模型 ID | `gemini-3-flash-preview` |
| Max Tokens | 最大生成 Token 数 | 4000 |
| Temperature | 生成随机性 (0-2) | 0.7 |
| Top P | 核采样概率 (0-1) | 1 |
| 历史记录条数 | 本地保存的历史数量 | 20 |
| Stream 输出 | 是否启用流式响应 | 启用 |

---

| Setting | Description | Default |
|---------|-------------|---------|
| Base URL | API base address | `https://ai.t8star.cn/v1` |
| API Key | Your API key | - |
| Model | AI model ID | `gemini-3-flash-preview` |
| Max Tokens | Max tokens to generate | 4000 |
| Temperature | Randomness (0-2) | 0.7 |
| Top P | Nucleus sampling (0-1) | 1 |
| History Limit | Local history count | 20 |
| Stream | Enable streaming response | Enabled |

---

## 📂 项目结构 | Project Structure

```
.
├── index.html      # 主页面 / Main page
├── favicon.png     # 网站图标 / Favicon
└── README.md       # 项目说明 / Project README
```

---

## 🔧 技术栈 | Tech Stack

- **纯前端** - 无需后端服务器，数据存储在浏览器本地
- **OpenAI 兼容 API** - 支持任意兼容 OpenAI 格式的 API 服务
- **浏览器 API** - FileReader、Fetch API、localStorage

---

- **Pure Frontend** - No backend required, data stored in browser locally
- **OpenAI Compatible API** - Supports any OpenAI-compatible API service
- **Browser APIs** - FileReader, Fetch API, localStorage

---

## 💡 系统提示词预设 | System Prompt Presets

### 📹 视频反推预设
用于分析视频内容，生成适合视频生成模型的提示词（中英文双语）。

Analyze video content and generate prompts suitable for video generation models (bilingual Chinese/English).

### 📷 图片反推预设
用于分析图片内容，生成适合图像生成模型的提示词（中英文双语）。

Analyze image content and generate prompts suitable for image generation models (bilingual Chinese/English).

### 自定义预设
支持创建、保存、重命名和删除自定义系统提示词预设。

Support creating, saving, renaming, and deleting custom system prompt presets.

---

## 🌐 浏览器兼容性 | Browser Compatibility

- Chrome / Edge / Firefox / Safari 最新版本
- 支持拖拽和粘贴功能的现代浏览器

---

- Chrome / Edge / Firefox / Safari latest versions
- Modern browsers supporting drag & drop and paste functionality

---

## 📄 许可证 | License

MIT License
