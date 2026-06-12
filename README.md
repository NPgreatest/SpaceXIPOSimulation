# SpaceX IPO Simulation (SPCX)

本地 IPO 首日短线交易沙盘 · Local day-1 trading sandbox. **No install, no server, no API.**

## 打开 / Open

```bash
open index.html
```

或直接双击 `index.html` · Or double-click `index.html`

## 功能 / Features

- 固定：**SPCX**，IPO 成本 **$135**
- 4 种情景：止损 · TP1 · TP2 · 放飞 Trailing
- 滑块：成交价 E、止损价、最高价 H、乐观度（期望收益）
- 中英文切换（右上角）
- 情景内 P/L **累计**计算；情景之间**不累加**

## 计算说明 / Calculation

| 情景 | 路径 |
|------|------|
| Stop loss | E → stop |
| TP1 | TP1 sell → remainder @ E |
| TP2 | TP1 + TP2 → remainder @ E |
| Moon | TP1 + TP2 → trailing exit |

Expected P/L = weighted sum of scenario totals.

## 文件 / Files

| File | Description |
|------|-------------|
| `index.html` | 全部代码（HTML + CSS + JS） |

## Disclaimer

Sandbox only. Not investment advice. No auto-trading.
