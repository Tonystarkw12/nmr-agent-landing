# nmr-agent-landing

NMR Agent 课题产品宣传页的源仓库。

- 线上：https://nmr.201014.xyz
- Pages 项目：`nmr-agent-landing`（Cloudflare Pages，**Git 集成** — push 即自动重建部署）
- 分支：`main`（生产分支）
- GraphPulse 桌面客户端（Windows/macOS/Linux）：发布在 [GitHub Releases](https://github.com/Tonystarkw12/nmr-agent-landing/releases)，页面下载卡直链 `releases/latest/download/<文件名>`。注意 Linux AppImage 76MB 超出 Cloudflare Pages 单文件 25MiB 上限，安装包一律走 Releases，不进仓库。

## 内容

| 文件 | 说明 |
|---|---|
| `index.html` | 宣传页主体（单页，双语 `data-i18n`） |
| `GraphPulse宣传视频.mp4` | 宣传视频主文件（18MB） |
| `media/graphpulse-promo.mp4` | 压缩版宣传视频（3.5MB） |
| `media/graphpulse-poster.jpg` | 视频封面图 |
| `NMRagent宣传视频.mp4` | NMRagent 宣传视频主文件（6MB） |
| `nmrsim-py宣传视频.mp4` | nmrsimpy 宣传视频主文件（7MB） |
| `media/nmragent-promo.mp4` / `media/nmragent-poster.jpg` | NMRagent 部署版视频与封面 |
| `media/nmrsim-py-promo.mp4` / `media/nmrsim-py-poster.jpg` | nmrsimpy 部署版视频与封面 |

## 工作流

```bash
git pull
# 编辑 index.html / media/
git add -A && git commit -m "..." && git push
# → Cloudflare Pages 自动构建并部署到 nmr.201014.xyz
```

> 本机状态（`.claude/` `.codex/` `.repowise/` `.mcp.json` 等）已由 `.gitignore` 排除，不会进入仓库与部署产物。
