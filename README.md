# ⚡ 赛博修仙 · Cyber Cultivation

> 电子工程 × 修仙 — 用电阻、电容、芯片、PCB 主板合成装备，在赛博废墟里打怪升级的网页小游戏。

[![Play Online](https://img.shields.io/badge/Play%20Online-GitHub%20Pages-blue?style=for-the-badge)](https://pmhawaii666.github.io/cyber-xiuxian/)

---

## 🎮 一句话玩法

废墟打怪 → 拆解电阻/电容/芯片 → 合成武器护甲 → 闭关修炼 → 突破境界 → 飞升

## ✨ 核心特性

- **10 大境界 × 40 小阶** — 从炼气到飞升，每个境界形象和特效都会变化
- **电子元器件机制** — 10 种真实电子元件，每个都按物理特性设计游戏效果：
  - 电阻 🟫 = 减伤（限流）
  - 电容 🔵 = 储能/瞬发法术
  - 二极管 🟨 = 单向护盾/信号干扰
  - 晶体管 🟪 = 伤害放大
  - CPU 🧠 = 超频一击（伤害×4 但需要冷却）
- **回合制战斗** — 普攻/法术/道具/逃跑，带暴击系统、伤害飘字、火花粒子、屏幕震动
- **合成组装系统** — PCB 板当基底，拼电阻电容做护盾、武器、突破丹
- **战斗快捷栏** — 最多 4 个法术常驻快捷栏，法术面板 ⭐ 一键配置
- **任务系统** — 主线 + 每日 + 成就，自动计数 + 徽章提醒
- **闭关离线恢复** — 关闭页面也能积累修为（上限 24 小时）
- **Web Audio 合成音效** — 零文件依赖，纯代码生成 12 种电子音效
- **自动存档** — localStorage 本地自动保存
- **个人中心** — 头像、属性、音量、特效开关、战绩统计

## 📂 项目结构

```
cyber-xiuxian/
├── index.html          ← 游戏本体（单文件，约 250KB）
├── README.md
└── GAME_DESIGN.md      ← 完整设计文档
```

## 🚀 本地运行

```bash
# 方式 1：直接双击 index.html
# 方式 2：起个本地服务器（推荐，避免 localStorage 问题）
cd xiuxian
python -m http.server 8080
# 然后浏览器打开 http://localhost:8080
```

## 🌐 部署到 GitHub Pages

```bash
cd xiuxian
git init && git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/cyber-xiuxian.git
git add .
git commit -m "v2.0 赛博修仙完整版"
git push -u origin main
```

然后 GitHub 仓库 → Settings → Pages → Source 选 `main / root` → Save

## 🛠️ 技术栈

- **纯前端单 HTML 文件** — HTML + CSS + 原生 JavaScript
- **零外部依赖** — 无 CDN、无构建工具、无框架
- **Web Audio API** — 纯代码合成音效
- **localStorage** — 自动存档

## 📋 更新日志

**v2.0** (2026-11-20)
- 🏷️ 任务系统（主线/每日/成就 12 个任务）
- ⚔️ 战斗快捷栏默认展开，支持法术面板 ⭐ 配置
- 📉 头部精简（节省 70% 高度）
- 🔧 闭关 bug 修复（不满也加经验 + 停止按钮 + 离线恢复）
- 🎨 法术面板新增快捷栏配置区

**v1.x**
- 境界进化系统（10 大境界 × 专属形象 + 特效）
- 电子元器件系统（10 种零件 + 物理特性→游戏机制）
- 合成组装（5 类 17 配方）
- 回合制战斗 + 动态特效（飘字/火花/震动/摇晃）
- Web Audio 合成音效（12 种）
- 个人中心（属性/设置/战绩）
- 示波器血条 + 嘉立创科技蓝主题

## 📄 License

MIT — 随便玩，随便改。
