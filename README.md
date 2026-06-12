# SpaceX IPO Simulation (SPCX)

本地 IPO 首日短线交易沙盘 · Local day-1 trading sandbox. **No install, no server, no API.**

## 在线体验 / Live demo

**[打开模拟器 →](https://npgreatest.github.io/SpaceXIPOSimulation/)**

> GitHub README **不能**内嵌可交互 HTML（会过滤 script，且 blob 链接只显示源码）。  
> 用 **GitHub Pages** 托管 `index.html`，用户点链接即可浏览器里直接用，无需下载。

首次启用：Repo → **Settings → Pages** → Source 选 **master** 分支、**/ (root)** → Save。

## 本地打开 / Open locally

```bash
git clone git@github.com:NPgreatest/SpaceXIPOSimulation.git
cd SpaceXIPOSimulation
open index.html
```

或双击 `index.html` · Or double-click `index.html`

## 功能 / Features

- 固定：**SPCX**，IPO 成本 **$135**
- 4 种情景：止损 · TP1 · TP2 · 放飞 Trailing
- 滑块：成交价 E、止损价、最高价 H、乐观度（期望收益）
- 中英文切换（右上角）
- 情景内 P/L **累计**；情景之间**不累加**

## 计算 / Calculation

| 情景 | 路径 |
|------|------|
| Stop loss | E → stop |
| TP1 | TP1 sell → remainder @ E |
| TP2 | TP1 + TP2 → remainder @ E |
| Moon | TP1 + TP2 → trailing exit |

## Disclaimer

Sandbox only. Not investment advice. No auto-trading.
