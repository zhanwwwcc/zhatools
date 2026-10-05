# zhatools · 离线小工具集

一组小巧的浏览器工具，打开即用。**所有代码都跑在你自己的浏览器里** —— 不联网、不上传任何内容，断网也能正常工作。

> 在线访问：**https://zhanwwwcc.github.io/zhatools/**

## 🧰 工具列表

| 工具 | 在线地址 | 说明 |
| --- | --- | --- |
| 二维码生成器 | [/qr/](https://zhanwwwcc.github.io/zhatools/qr/) | 文字、网址一键变二维码，支持中文/Emoji，可下载 PNG 或复制到剪贴板 |
| 字幕格式转换器 | [/subtitle/](https://zhanwwwcc.github.io/zhatools/subtitle/) | VTT / SRT / LRC / ASS / SSA / SUB 七种格式任意互转，核心支持 VTT → LRC |

## ✨ 共同特点

- 🔒 **100% 离线**：算法与依赖全部内嵌，无任何 CDN、在线 API 或网络请求
- 📦 **单文件即产品**：每个工具都是一个独立的 HTML 文件，无构建步骤，拷走就能用
- 🖥️ **无需安装**：双击打开即可，不需要服务器、不需要环境
- 🔤 **中文友好**：完整支持中文、Emoji，并对老编码（GBK/GB18030/UTF-16）做自动兜底
- 🧩 **互不干扰**：每个工具各自独立，某个工具出问题不影响其他工具

## 📁 目录结构

```
zhatools/
├── index.html          # 导航首页（工具卡片）
├── qr/
│   └── index.html      # 二维码生成器
├── subtitle/
│   └── index.html      # 字幕格式转换器
├── README.md
└── LICENSE
```

## 🚀 本地使用

任选一种：

1. **单个工具离线用**：直接下载 `qr/index.html` 或 `subtitle/index.html`，双击打开即可，不需要网络
2. **整套工具本地跑**：在项目根目录执行 `python3 -m http.server 8000`，然后访问 http://localhost:8000/

## ➕ 如何新增一个工具

1. 新建目录 `新工具名/index.html`，把完整的单文件工具放进去（入口文件名必须是 `index.html`）
2. 在根目录 `index.html` 的卡片区加一张 `<a class="card" href="新工具名/index.html">` 卡片
3. 在本 README 的「工具列表」表格里补一行
4. 提交推送，GitHub Pages 会自动更新

## 📄 License

[MIT](LICENSE) © 2026 zhanwwwcc
