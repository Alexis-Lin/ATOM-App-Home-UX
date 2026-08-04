# ATOM · App Home UX（手机 App 首页 Home Tab 优化设计）

> BodyPark ATOM **手机 App** 首页 Home Tab 的优化设计工作仓库。
> 本仓库存放该项目的**讨论定义、产品/交互规格、工程设计文件**。

---

## 这是什么

BodyPark ATOM 产品家族目前有两条「首页」线：

| 线 | 载体 | 仓库 |
|---|---|---|
| **Companion Home** | ATOM 圆屏桌面设备的拟人化管家首页（表情卡） | [`ATOM-Companion-Home`](https://github.com/Alexis-Lin/ATOM-Companion-Home) |
| **App Home（本仓库）** | 手机 App 的首页 Home Tab | 本仓库 |

本仓库聚焦**手机 App 首页 Home Tab 的优化设计**。设计上可能参考或呼应设备端 Companion Home 的既有逻辑（拟人化人格、S1/S2/S3 分层、碎碎念 Natter、能量签 Energy Draw、连胜 Streak 等）——已提炼为 [`ATOM-APP-REF-Companion呼应点.md`](ATOM-APP-REF-Companion呼应点.md)，讨论时直接引用即可，不必重读设备端全套文档。

---

## 文档导航

| 文档 | 内容 | 状态 |
|---|---|---|
| [ATOM-APP-00-总纲.md](ATOM-APP-00-总纲.md) | 总览：目标 / 范围 / 基线方案 / 待讨论决策清单 D1–D18 | 🚧 v0.4，随讨论迭代 |
| [ATOM-APP-01-首页立意-三区模型.md](ATOM-APP-01-首页立意-三区模型.md) | 立意：首页=PLAN 闭环每日渲染面;三区模型 / CTA 状态矩阵 / 社区承接 | 🚧 v0.1 讨论稿 |
| [ATOM-APP-02-信息架构与状态框架.md](ATOM-APP-02-信息架构与状态框架.md) | 模块落位 / 五维状态体系与分区状态机 / A 区决策树 / 快照 HS-1~8 | 🚧 v0.1 讨论稿 |
| [ATOM-APP-03-计划Tab提案.md](ATOM-APP-03-计划Tab提案.md) | 「训练」Tab：计划主页 + 动作库全屏二级页 + 与首页分界规则 | 🚧 v0.2 讨论稿 |
| [ATOM-APP-04-Tab架构与模块聚类.md](ATOM-APP-04-Tab架构与模块聚类.md) | 五 Tab × 九模块聚类：首页/训练/ATOM(中央)/社区/我的 + 分期与护栏 | 🚧 v0.1 讨论稿 |
| [ATOM-APP-REF-竞品首页扫描.md](ATOM-APP-REF-竞品首页扫描.md) | 9 产品竞品首页扫描（Peloton/Ladder/Fitness+/Keep/训记/咕咚/Strava/Fitbod/NTC）,原始报告在 [research/](research/) | ✅ 参考基线 |
| [wireframe/home-wireframe-v0.html](wireframe/home-wireframe-v0.html) | 低保真线框：三区模型 × 状态快照 HS-1~7 可切换（浏览器打开） | 🚧 v0 |
| [wireframe/app-prototype-v1.html](wireframe/app-prototype-v1.html) | 全 App 框架交互原型：iPhone17(402×874pt) · 四 Tab 可点 · 动作库全屏二级页 · ◎ATOM 面板 · 跨页深链 | 🚧 v1 |
| [ATOM-APP-REF-Companion呼应点.md](ATOM-APP-REF-Companion呼应点.md) | 设备端 Companion Home 逻辑提炼：可呼应的概念、机制与参数（R1–R10） | ✅ 参考基线 |
| [ATOM-APP-REF-目标偏好呼应点.md](ATOM-APP-REF-目标偏好呼应点.md) | [ATOM-UserGoalPreference-and-OnBoarding](https://github.com/Alexis-Lin/ATOM-UserGoalPreference-and-OnBoarding) 逻辑提炼：首页的个性化引擎（P1–P8） | ✅ 参考基线 |
| [v1-基线方案/](v1-基线方案/) | 历史阶段方案 v1（2026-06-08）：改版方案说明 + 可交互原型 HTML（浏览器打开,可切新/老用户与设备异常态） | ✅ 只读存档 |

> 后续按需增补（沿用设备端仓库的编号习惯）：
> `ATOM-APP-01-信息架构.md` · `ATOM-APP-02-<模块>-PRD.md` · `ATOM-APP-技术设计.md` · `ATOM-APP-设计素材清单.md` · 原型 Demo 等。

---

## 文档规范

- **命名**：`ATOM-APP-<编号|类别>-<主题>.md`，与设备端仓库的 `ATOM-<编号>-<主题>.md` 保持家族一致、前缀区分。
- **文头**：每份文档标注 `版本 | 日期 | 受众`。
- **讨论沉淀**：讨论中的定义、拍板结论进对应文档;未拍板事项集中挂在总纲「待讨论决策清单」，避免散落。
- **跨仓引用**：呼应设备端逻辑时,引用 `ATOM-APP-REF-Companion呼应点.md` 的条目号,并注明设备端源文档章节（如 `Companion ATOM-01 §4`）。
