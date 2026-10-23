# nmr-agent-landing

NMR Agent 课题产品宣传页的源仓库。

- 线上：https://nmr.201014.xyz
- Pages 项目：`nmr-agent-landing`（Cloudflare Pages，**Git 集成** — push 即自动重建部署）
- 分支：`main`（生产分支）

## 内容

| 文件 | 说明 |
|---|---|
| `index.html` | 宣传页主体（单页，双语 `data-i18n`） |
| `GraphPulse宣传视频.mp4` | 宣传视频主文件（18MB） |
| `media/graphpulse-promo.mp4` | 压缩版宣传视频（3.5MB） |
| `media/graphpulse-poster.jpg` | 视频封面图 |

## 工作流

```bash
git pull
# 编辑 index.html / media/
git add -A && git commit -m "..." && git push
# → Cloudflare Pages 自动构建并部署到 nmr.201014.xyz
```

> 本机状态（`.claude/` `.codex/` `.repowise/` `.mcp.json` 等）已由 `.gitignore` 排除，不会进入仓库与部署产物。
