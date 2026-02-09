# 🌉 桥梁守卫者 | Bridge Defender

[![GitHub Pages](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue?logo=github)](https://chenhaubin.github.io/bridge-defender/bridge-defender-game.html)
[![HTML5](https://img.shields.io/badge/HTML5-Canvas-orange?logo=html5)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-yellow?logo=javascript)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

> 一款基于 HTML5 Canvas 的桥梁塔防射击游戏

![Game Preview](https://img.shields.io/badge/Preview-Available-brightgreen)

## 🎮 游戏简介

在遥远的未来，一座连接两个世界的桥梁正遭到敌人入侵。你扮演一名精英守卫者，控制高科技战斗单位在桥梁上巡逻，自动射击摧毁来犯的敌军。

**核心特色：**
- 🌉 **透视桥梁视角** - 独特的双车道纵深视觉效果
- 🎮 **流畅操作** - 左右切换车道，自动瞄准射击
- 💥 **炫酷特效** - 粒子爆炸、伤害飘字、发光UI
- 🔊 **动态音效** - Web Audio API 实时生成音效
- 📱 **多端适配** - 支持键盘和触屏操作

## 🎯 游戏玩法

### 操作说明

| 操作 | 键盘 | 触屏 |
|------|------|------|
| 向左移动 | `←` 或 `A` | 向左滑动 |
| 向右移动 | `→` 或 `D` | 向右滑动 |
| 切换车道 | `空格键` | 快速滑动 |

### 游戏元素

#### 敌人
| 类型 | 颜色 | 生命值 | 速度 | 分数 |
|------|------|--------|------|------|
| 无人机 | 🔴 红色 | 30 | 快 | 10 |
| 坦克 | 🟠 橙色 | 80 | 慢 | 25 |
| 高速单位 | 🟣 紫色 | 15 | 极快 | 15 |

#### 道具
| 道具 | 效果 | 持续时间 |
|------|------|----------|
| 💚 生命包 | 恢复 20 HP | 即时 |
| 💙 能量核心 | 快速射击 | 5秒 |
| 💜 多重火力 | 三连发射击 | 即时 |

#### 障碍物
- 🟡 **路障** - 阻挡去路，需要多次射击摧毁（50 HP）

### 计分规则
- 摧毁敌人获得对应分数
- 波次越高，挑战越大
- 敌人到达底部扣除 10 点生命

## 🚀 快速开始

### 在线游玩
👉 **[点击开始游戏](https://chenhaubin.github.io/bridge-defender/bridge-defender-game.html)**

### 本地运行

```bash
# 克隆仓库
git clone https://github.com/chenhaubin/bridge-defender.git

# 进入目录
cd bridge-defender

# 用浏览器打开
open bridge-defender-game.html

# 或启动本地服务器
python3 -m http.server 8080
# 访问 http://localhost:8080/bridge-defender-game.html
```

## 🛠️ 技术栈

- **HTML5 Canvas** - 游戏渲染
- **Vanilla JavaScript** - 游戏逻辑（无依赖）
- **Web Audio API** - 动态音效生成
- **CSS3** - UI 样式与动画

## 📁 项目结构

```
bridge-defender/
├── bridge-defender-game.html    # 主游戏文件（单文件架构）
├── README.md                     # 项目说明
└── LICENSE                       # MIT 许可证
```

> 采用单文件架构，所有代码（HTML + CSS + JS）集成在一个文件中，便于部署和分享。

## 🎨 游戏截图

*游戏启动界面 - 科技感UI设计*

*战斗场景 - 透视桥梁视角*

*道具收集 - 多彩特效*

## 🔧 开发计划

- [ ] 添加更多敌人类型
- [ ] 实现武器升级系统
- [ ] 添加背景音乐
- [ ] 本地排行榜
- [ ] 移动端手势优化
- [ ] PWA 离线支持

## 🤝 贡献指南

欢迎提交 Issue 和 Pull Request！

1. Fork 本仓库
2. 创建你的分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送分支 (`git push origin feature/AmazingFeature`)
5. 创建 Pull Request

## 📄 许可证

本项目基于 [MIT](LICENSE) 许可证开源。

## 🙏 致谢

- 游戏灵感来源于经典塔防和射击游戏
- 感谢 HTML5 Game Development 社区的教程和资源

---

<p align="center">Made with ❤️ by <a href="https://github.com/chenhaubin">@chenhaubin</a></p>
