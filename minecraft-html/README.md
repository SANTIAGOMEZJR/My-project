# Minecraft Java Survival

<p align="center">
  一个无需构建步骤的浏览器体素生存体验。
  <br>
  <a href="https://yxc1130.github.io/minecraft-java-survival/"><strong>在线游玩</strong></a>
  ·
  <a href="#操作">操作</a>
  ·
  <a href="#本地运行">本地运行</a>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Three.js-r160-111111?logo=threedotjs&logoColor=white" alt="Three.js r160">
  <img src="https://img.shields.io/badge/Runtime-Browser-2ea44f" alt="Browser runtime">
  <img src="https://img.shields.io/github/license/yxc1130/minecraft-java-survival" alt="MIT license">
</p>

![Minecraft Java Survival game screen](assets/preview.png)

## 概览

`Minecraft Java Survival` 是一个由单个 `index.html` 驱动的第一人称体素生存游戏。它以 Three.js 渲染程序化方块世界，并把世界变更、背包、生命、饥饿和玩家位置保存在浏览器本地存储中。

- 程序化生成有限世界，含平原、浅海、丘陵、积雪山地、树木、洞穴和矿石。
- 鼠标指向方块，支持持续挖掘、拾取、背包堆叠和放置。
- 第一人称移动、碰撞、跳跃、疾跑、游泳、跌落伤害与重生。
- 日夜循环、云层、星空、水面、像素材质和挖掘粒子效果。
- 本地自动存档；可从菜单生成新世界或清除存档。
- 无打包、无服务端、无构建产物。现代浏览器打开即可运行。

## 操作

| 输入 | 行为 |
| --- | --- |
| `W` `A` `S` `D` | 移动 |
| 鼠标 | 环顾四周 |
| `Space` | 跳跃 / 水中上浮 |
| `Shift` | 疾跑 |
| 鼠标左键 | 按住挖掘方块 |
| 鼠标右键 | 放置当前方块 |
| `1` - `9` / 滚轮 | 选择物品栏 |
| `Esc` | 释放鼠标并打开暂停菜单 |

## 本地运行

项目直接依赖浏览器原生 ES Modules 和 jsDelivr 上的 Three.js。为了避免浏览器对本地模块资源的限制，使用任意静态文件服务器启动：

```bash
npx serve .
```

然后在浏览器打开命令输出的本地地址。需要支持 WebGL 和 Pointer Lock API 的现代桌面浏览器。

## 项目结构

```text
.
├── index.html                  # 游戏界面、渲染、输入、存档与世界逻辑
├── assets/preview.png          # GitHub 仓库预览图
├── .github/workflows/
│   └── deploy-pages.yml        # GitHub Pages 自动部署
└── test/repository.test.mjs    # 发布资料完整性检查
```

## 部署

推送到 `main` 分支会触发 GitHub Actions，并发布根目录中的静态站点到 GitHub Pages：

<https://yxc1130.github.io/minecraft-java-survival/>

## 技术说明

- [Three.js](https://threejs.org/) r160 负责 WebGL 渲染。
- 方块纹理由运行时 Canvas 生成，不依赖外部贴图文件。
- 地形、树木、矿石和洞穴以种子驱动的噪声与哈希函数生成。
- 存档仅写入当前浏览器的 `localStorage`，不会上传到网络。

## 许可与声明

本项目以 [MIT License](LICENSE) 发布。

Minecraft 是 Mojang Studios 的商标。本项目是独立的浏览器实验作品，与 Mojang Studios 或 Microsoft 没有隶属、认可或合作关系。
