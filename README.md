# 跨境电商图片提示词库

一个静态网页工具，用于快速生成美国、英国市场常用电商图片提示词。当前重点服务 TikTok Shop，同时保留 Amazon / eBay / Shopify / 通用电商模板。

## 在线地址

GitHub Pages:

```text
https://coderdnf.github.io/img-prompt/
```

GitHub 仓库:

```text
https://github.com/coderdnf/img-prompt
```

## 日常使用

1. 打开线上地址。
2. 在左侧填写产品名称、平台、画面比例、目标买家、核心卖点、用户痛点、材质细节和必须避免项。
3. 平台选择 `TikTok Shop` 时，右侧显示 TikTok Shop 专用模板。
4. 平台选择 `Amazon`、`eBay`、`Shopify` 或 `通用电商` 时，右侧显示通用电商模板。
5. 点击 `复制提示词`，粘贴到 GPT 或图片生成工具里使用。
6. 点击 `查看 6 个 Prompt 心法` 可以查看常用提问方法图片。

## 当前模板

TikTok Shop 专用模板:

- 高点击商品封面图
- 真人使用种草图
- 痛点瞬间图
- 使用前后对比图
- 直播间挂车图
- 移动端卖点信息图
- 开箱套装展示图
- TikTok Shop 8 张图整套生成

Amazon / 通用电商模板:

- 白底主图
- 生活场景图
- 核心卖点信息图
- 问题解决型图片
- 同类普通款对比图
- 尺寸规格图
- 材质细节特写
- 7 张图整套生成模板
- 通用负面提示词

## 文件结构

```text
.
├── AGENTS.md
├── README.md
├── index.html
├── server.mjs
├── .gitignore
└── assets/
    └── prompt-mindset.png
```

说明:

- `index.html`: 线上页面主体，包含样式、模板数据和复制功能。
- `assets/prompt-mindset.png`: 6 个 Prompt 心法图片。
- `server.mjs`: 可选本地静态服务，不是 GitHub Pages 必需文件。
- `.gitignore`: 忽略本地服务日志。

## 本地预览

直接打开 `index.html` 即可。

如果需要本地服务预览:

```powershell
cd D:\Codex-item\img-prompt
node server.mjs
```

然后访问:

```text
http://127.0.0.1:5173/
```

## 更新线上页面

修改文件后执行:

```powershell
cd D:\Codex-item\img-prompt
git status
git add README.md AGENTS.md index.html assets
git commit -m "Update prompt library"
git push
```

如果 Git 提示 `dubious ownership`:

```powershell
git config --global --add safe.directory D:/Codex-item/img-prompt
```

推送后等待 1-3 分钟，再刷新 GitHub Pages 页面。

## 注意

- GitHub Pages 是公开页面，不要放账号、密钥、供应链信息、真实爆款产品库或未公开产品数据。
- 不要直接复制竞品品牌名、Logo、包装图或受保护设计到提示词里。
- TikTok Shop 模板更偏短视频货架、移动端点击和场景种草；Amazon / 通用模板更偏清晰展示、信息图和合规表达。
