# estimate-before-build 先估后建

"It'll take a few minutes" is where scope creep pays rent. Estimate first — not to predict the future, but to make the scope decision explicit.

"几分钟就好"是范围蔓延的房租来源。先估——不是为了预言未来，而是为了让范围决策显式化。

## Why / 为什么

The expensive failure is not the wrong estimate — it is the **unmade decision**: the agent starts building, the request turns out to be three times the size anyone imagined, and stopping now looks like failure. An estimate before the first edit turns that silent slide into a choice: this scope for this budget, or a smaller scope.

昂贵的失败不是估错——而是**没做决定**：agent 开始动手，请求实际是任何人想象的三倍，此刻停下显得像失败。动手前的估算把无声滑坡变成选择：这个范围配这个预算，或者缩小范围。

## Size bands, not hours / 用档位，不用小时

| Band | Meaning | Example |
|---|---|---|
| S | one sitting, no unknowns | add a field to a form |
| M | a few sittings or one unknown | new page with data fetching |
| L | multiple unknowns or cross-system | payment integration |
| XL | needs its own plan first | migration, rewrite |

Hours invite false precision and calendar promises; bands communicate shape. **Name the uncertainty driver** for M and above ("depends on the API's real pagination behavior") — the driver is where the risk lives and where a spike belongs.

小时数制造假精度和日历承诺；档位传达形状。M 档以上必须**点名不确定性来源**（"取决于 API 真实的分页行为"）——风险住在那里，spike 也该打在那里。

## The decision that must surface / 必须摆上桌面的决定

Present, don't pick: full scope in the estimate, a reduced scope that fits the budget, or a timeboxed spike for the unknowns first. Then record the estimate — because the **finish-line comparison** (estimate vs actual, per task) is the only mechanism that makes the next estimate better.

摆出来，别替选：全范围、能塞进预算的缩减范围、或先 timebox 探明未知。然后把估算记录下来——因为**终点对账**（逐任务：估的 vs 实际）是让下次估算变准的唯一机制。

## Install / 安装

```bash
npx skills add ChenneyZhuang/estimate-before-build
```

Per-agent paths: [COMPATIBILITY.md](COMPATIBILITY.md). MIT. v0.1.0.

各 agent 安装路径见 COMPATIBILITY.md。MIT 许可，v0.1.0。
