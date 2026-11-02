# legado 书单订阅仓库

手机阅读（legado / 开源阅读）书架书单的公开静态托管。仓库内每个 `.json` 是一份可在阅读 App「网络导入 / 订阅书单」中粘贴直链导入的书架清单，格式为 `author / intro / name` 精简书单（不含章节链接、封面与阅读进度）。

## 书单清单

| 文件 | 对应书单 | 条目 | 核对清单（仅供人工核对，不用于导入） |
| --- | --- | --- | --- |
| `genre-98.json` | 题材书单（都市恋爱、日常、病娇与特殊题材等） | 98 | `genre-98.txt` |
| `ranking-nov2026-119.json` | 11月口碑增量榜（2026） | 119 | `ranking-nov2026-119.txt` |

## 订阅链接（在阅读 App「网络导入 / 订阅书单 / 导入书单」粘贴）

优先使用 fastly 镜像；不通时换 gcore 备用镜像。raw 主域在部分国内网络直连不稳，仅作备用。

### 题材书单（98 本）

- 主（fastly）：`https://fastly.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/genre-98.json`
- 备（gcore）：`https://gcore.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/genre-98.json`
- raw 备用：`https://raw.githubusercontent.com/liujiapei009/legado-bookshelf/main/genre-98.json`

### 11月口碑增量榜（119 本）

- 主（fastly）：`https://fastly.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/ranking-nov2026-119.json`
- 备（gcore）：`https://gcore.jsdelivr.net/gh/liujiapei009/legado-bookshelf@main/ranking-nov2026-119.json`
- raw 备用：`https://raw.githubusercontent.com/liujiapei009/legado-bookshelf/main/ranking-nov2026-119.json`

> 若 App 对 `.json` 后缀识别不稳，可改用同目录同名 `.txt` 镜像链接，或在 App 内改后缀重试；导入以 `.json` 为准。

## 更新方式

电脑端生成新书单 JSON 后，复制到本目录、提交并推送到 `main` 分支；上面的链接地址保持不变，手机端重新订阅或刷新即可拉到最新内容。
