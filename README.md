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
| [ATOM-APP-00-总纲.md](ATOM-APP-00-总纲.md) | 总览：目标 / 范围 / 现状问题 / 待讨论决策清单 | 🚧 v0.1 骨架，随讨论迭代 |
| [ATOM-APP-REF-Companion呼应点.md](ATOM-APP-REF-Companion呼应点.md) | 设备端 Companion Home 逻辑提炼：可呼应的概念、机制与参数 | ✅ 参考基线 |

> 后续按需增补（沿用设备端仓库的编号习惯）：
> `ATOM-APP-01-信息架构.md` · `ATOM-APP-02-<模块>-PRD.md` · `ATOM-APP-技术设计.md` · `ATOM-APP-设计素材清单.md` · 原型 Demo 等。

---

## 文档规范

- **命名**：`ATOM-APP-<编号|类别>-<主题>.md`，与设备端仓库的 `ATOM-<编号>-<主题>.md` 保持家族一致、前缀区分。
- **文头**：每份文档标注 `版本 | 日期 | 受众`。
- **讨论沉淀**：讨论中的定义、拍板结论进对应文档;未拍板事项集中挂在总纲「待讨论决策清单」，避免散落。
- **跨仓引用**：呼应设备端逻辑时,引用 `ATOM-APP-REF-Companion呼应点.md` 的条目号,并注明设备端源文档章节（如 `Companion ATOM-01 §4`）。
