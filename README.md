# legado 待读书单存档仓库

本仓库只用于**静态存档与浏览器在线查看**一批待读小说目录（书名 / 作者 / 简介）。

> **重要说明（2026-11-03 真机核对更正）**
> 这些 `.json` **不是**开源阅读（legado / 阅读 App）的书架备份格式，也**不能**在 App 里通过「网络导入 / 订阅书单 / 导入书单」粘贴使用。
> 官方 legado 的网络导入只接受**规则书源（bookSource）**；粘贴本仓库的清单链接会被当成书源解析，报"格式错误 / 解析失败 / 书源为空"。
> 想把清单里的书放进书架，只能在 App 里装好书源后，逐本搜索书名（必要时带作者）→ 点开结果 → 放入书架；本清单仅作对照查看用。

## 书单清单

| 文件 | 对应书单 | 条目 | 人工核对清单（纯文本） |
| --- | --- | --- | --- |
| `genre-98.json` | 题材书单（都市恋爱、日常、病娇与特殊题材等） | 98 | `genre-98.txt` |
| `ranking-nov2026-119.json` | 11月口碑增量榜（2026） | 119 | `ranking-nov2026-119.txt` |

## 在线查看链接（浏览器打开，非 App 订阅地址）

优先 fastly 镜像；不通时换 gcore。raw 主域在部分国内网络直连不稳，仅备用。

### 题材书单（98 本）

- fastly：`https://fastly.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/genre-98.json`
- gcore：`https://gcore.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/genre-98.json`
- raw：`https://raw.githubusercontent.com/liujiapei009/legado-bookshelf/main/genre-98.json`

### 11月口碑增量榜（119 本）

- fastly：`https://fastly.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/ranking-nov2026-119.json`
- gcore：`https://gcore.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/ranking-nov2026-119.json`
- raw：`https://raw.githubusercontent.com/liujiapei009/legado-bookshelf/main/ranking-nov2026-119.json`

## 更新方式

电脑端生成新书单 JSON 后，复制到本目录、提交并推送到 `main` 分支；上面的链接地址保持不变。仓库内仅书名 / 作者 / 简介，不含账号密码与小说正文。
