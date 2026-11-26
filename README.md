# KOBE AIRWAYS · 坠机航班

一个可以直接在浏览器里玩的 3D 叙事小游戏，单文件构建，无外部依赖。

## 在线游玩

https://cubernie.github.io/groupwork-1/

打开即玩，无需安装。首次进入会加载 3.6 MB 左右的内嵌资源。

## 操作

| 操作 | 按键 |
| --- | --- |
| 移动 | `W` `A` `S` `D` |
| 环视 | 移动鼠标（点击画面锁定指针） |
| 交互 / 跳跃 | `Space`、`E`、`F` |
| 奔跑 | `Shift` |
| 释放鼠标 | `Esc` |

游戏内的解谜键位（例如 `X` 慢放时间、`K` 连线、`Q` 等）会在对应剧情里以键帽提示显示，跟着屏幕提示走即可。

## 兼容性

- ✅ 桌面浏览器（Chrome / Edge / Firefox / Safari）
- ⚠️ 手机浏览器可以打开，但**没有触屏操作**，需要键盘和鼠标

## 技术说明

- `index.html`：完整游戏，three.js r160 与全部模块以字符串内嵌，通过 Blob URL + import map 加载
- `kobe-airways.html`：旧链接的跳转页
- `.nojekyll`：关闭 GitHub Pages 的 Jekyll 处理，避免大文件被改写

## 本地运行

直接双击 `index.html` 即可；若浏览器限制本地模块加载，可在目录下起一个静态服务器：

```bash
python -m http.server 8000
```

然后访问 http://localhost:8000/ 。

## 许可

游戏代码与美术资源版权归原作者所有，仅用于课程小组作业展示。
