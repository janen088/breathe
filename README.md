# 呼吸引导

> 打工人的每日呼吸处方 — 5种呼吸节奏，离线可用

一个极简的 PWA 呼吸引导工具，无外部依赖，支持离线使用，适配移动端和微信内置浏览器。

## 功能

- 🧘 5 种呼吸节奏：安神入睡、冷静聚焦、午后提神、下班解压、工位偷闲
- 📱 PWA 支持：可添加到桌面，全屏使用
- 🔌 离线可用：Service Worker 缓存所有资源
- 🎨 极简设计：羊皮纸色 + 深海蓝，低饱和度
- 📲 微信兼容：无外部依赖，触摸友好

## 部署

### Vercel（推荐）

```bash
# 安装 Vercel CLI
npm i -g vercel

# 部署
vercel --prod
```

或者直接在 [vercel.com](https://vercel.com) 导入 Git 仓库，零配置部署。

### 其他静态托管

项目为纯静态文件，可直接部署到任何静态托管服务：

- 将所有文件上传到服务器根目录
- 确保 `sw.js` 响应头包含 `Service-Worker-Allowed: /`

## 技术栈

- 纯 HTML + CSS + JavaScript（零依赖）
- Canvas 动画
- PWA（manifest.json + Service Worker）
- SVG 图标

## 文件结构

```
breathe/
├── index.html      # 主页面（含所有样式和逻辑）
├── manifest.json   # PWA 清单
├── sw.js           # Service Worker
├── icon.svg        # SVG 图标
├── icon-192.png    # 192x192 PNG 图标
├── icon-512.png    # 512x512 PNG 图标
├── vercel.json     # Vercel 部署配置
├── .gitignore
└── README.md
```

## License

MIT
