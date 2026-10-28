# 🐍 贪吃蛇 · Snake

纯前端实现的小游戏：**单个 HTML 文件、零依赖、无需构建**，双击即玩，也可部署到 GitHub Pages。

## 玩法

| 操作 | 按键 |
|---|---|
| 移动 | 方向键 / `W` `A` `S` `D` |
| 暂停 / 继续 | `空格` |
| 重新开始 | `R` |
| 手机 | 下方方向键，或在棋盘上滑动 |

吃到食物 **+10 分**，速度逐渐加快；撞墙或撞到自己结束。最高分保存在浏览器本地。

## 运行

直接用 Chrome / Edge 打开 `index.html`。

或本地起个静态服务器：

```bash
python -m http.server 8000
# 访问 http://localhost:8000/
```

## 部署到 GitHub Pages

1. 仓库 **Settings → Pages**
2. Source 选 `Deploy from a branch`，分支 `main`，目录选 `/(root)`
3. 访问 `https://<用户名>.github.io/<仓库名>/`

## 目录

```
snake/
└── index.html    # 全部代码（HTML + CSS + JS）
```

## 可调参数

`index.html` 脚本开头：

| 变量 | 作用 | 默认 |
|---|---|---|
| `COLS` / `ROWS` | 棋盘列数 / 行数 | 20 × 20 |
| `CELL` | 每格像素 | 24 |
| `tickMs` | 初始速度（毫秒/步） | 150 |

## 许可

[MIT](../LICENSE)
