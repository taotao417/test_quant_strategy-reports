# v11.1-small-no-star 量化策略报告

**策略版本：** v11.1-small-no-star
**回测周期：** 2021-01-01 ~ 至今
**持仓风格：** Top10 核心 + Top20 缓冲

## 报告归档

### 盘后日报（每日 17:00 推送）
- [2026-07-03 盘后报告](daily_report/daily_report_2026-07-03_v11_1_small_no_star.md)
- [2026-07-02 盘后报告](daily_report/daily_report_2026-07-02_v11_1_small_no_star.md)
- [全部历史盘后报告 →](daily_report/)

### 盘中交易报告（9:35 / 14:00 推送）
- [2026-07-03 盘中报告](intraday_report/)
- [全部历史盘中报告 →](intraday_report/)

### 决策检查点
- [latest_decision.md](daily_report/latest_decision_v11_1_small_no_star.md)

## 策略摘要

- **候选池**：沪深300 + 中证500 成分股，约 120 只
- **因子**：动量 (25%) + 风险 (15%) + 流动性 (10%) + 财务占位 (50%)
- **建仓规则**：Top10 全部买入，每只等权 1 手（T+1 开盘成交）
- **调仓规则**：每日信号，T+1 开盘执行
- **卖出规则**：① 跌出 Top20 立即卖 ② Top20 内 + 高点回撤≥8% 且 浮盈≥3% → 止盈
- **仓位管理**：基于中证500 收盘 vs MA20/MA60 动态 60-100%

## 数据源

- 个股行情：AKShare `stock_zh_a_daily` (前复权 qfq)
- 中证500：AKShare `stock_zh_index_daily` (增量刷新)

## 推送通道

- Server 酱 (Turbo)：微信推送每日 9:35 / 14:00 / 17:00 报告
- GitHub Pages：本页面，所有报告永久归档

## 免责声明

⚠️ 以上内容由 AI 基于公开信息整理生成，仅供参考，不构成任何投资建议或个股推荐。投资有风险，决策需谨慎。
