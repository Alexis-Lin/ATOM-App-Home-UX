# ATOM App Home · 目标偏好体系呼应点参考

> 版本：v1.0　|　日期：2026-08-04　|　受众：产品 / 设计 / 研发
> 性质：**参考基线**。将 [`ATOM-UserGoalPreference-and-OnBoarding`](https://github.com/Alexis-Lin/ATOM-UserGoalPreference-and-OnBoarding) 仓库中与 App 首页直接相关的逻辑提炼为条目（P#）。只摘录不改写,源头以该仓 `schema/` SSOT 为准。

---

## P1 · 数据闭环:首页的引擎

数据流:`GOAL + STATUS + PREFERENCE →生成→ PLAN →执行→ LOG →回流→ STATUS → PLAN 重算`。
**对首页的含义**:首页不必发明自己的逻辑——它是**这条闭环的每日渲染面**。「今天练什么」来自 PLAN,「练得怎么样」来自 LOG/STATUS,「为什么练」来自 GOAL。首页做的是呈现与触发,不是决策。
源:`schema/PRD.md` §3、README「数据模型一句话」。

## P2 · Intent 两层目标模型:用户的原话可以上首页

`Goal.Intent`(用户怎么说:`user_intent_raw` 原文永远保留、`goals[]` 多目标带 priority/milestone/timeframe) ──映射──▶ `Goal.TrainingTarget`(系统怎么理解:D1 能力/D2 部位/D3 身体构成/D4 进阶锚点,仅 mapper 可写)。
**对首页的含义**:① 首页文案可以直接引用用户自己的话和里程碑(「距离十月婚礼还有 9 周」),这是「与我相关」的最短路径;② 「为什么今天练这个」可由 Target(focus_map/regions)派生解释,PLAN 可解释性有数据基础。
源:`schema/PRD.md` §4/§6、`intent-catalog.md`。

## P3 · mindset{motivation[], barrier[]}:激励文案的专用素材

动机(激励文案用)与阻力(留存干预用),明确**不参与算计划**。
**对首页的含义**:人格层问候/碎碎念(总纲 D2,呼应 Companion R4 Natter)的正当素材源——按 motivation 定口味、按 barrier 做干预(如「没时间」型用户推 10 分钟课)。
源:`schema/PRD.md` §4。

## P4 · 展示映射:进度模块的现成组件

每维天然一种可视化,已在该仓定义:D1→六维雷达+派生文案;D2→人体图高亮;D3→数字卡+进度条;D4→进阶阶梯(第 N 阶/共 M 阶)+成就解锁;goals[]→目标卡片列表。
**对首页的含义**:首页「我的进度」模块不需要新发明图形语言,从这套映射里**按主目标选 1 个**上首屏即可(全量展示归档案/历史页)。
源:`schema/PRD.md` §8。

## P5 · STATUS vs Target = 里程表 vs 目的地

STATUS 记「现在是多少」,Target 记「要到多少」,同指标同口径,**进度 = Target − STATUS 直接可算**。
**对首页的含义**:首页进度条/数字卡的数据口径已被定义,不存在首页自造口径的空间(呼应总纲 D10 口径对齐)。
源:`schema/PRD.md` §6。

## P6 · PREFERENCE 三分:推荐与快速开练的过滤依据

想不想(喜好:favorite/disliked 动作、指导风格)· 有没有(器械/场地/时间资源约束,PLAN 按硬约束消费)· 能不能(伤病安全,SSOT=STATUS.health)。偏好是用户主权字段。
**对首页的含义**:① 首页内容货架(精选/推荐)应按 PREFERENCE 过滤(不推没器械的课、避开 disliked 动作),从「人找内容」变「内容适配人」;② 「快速开练」兜底动线按资源约束(时间/器械)即时选课。
源:`schema/PRD.md` §7。

## P7 · Onboarding 衔接:与首页新手任务同源

该仓正在按 Intent 目录 V1.2 重写 Onboarding 问卷(`ui/onboarding/questionnaire-spec.md` 现为历史稿)。
**对首页的含义**:v1 首页新手任务清单②(个人资料)③(训练偏好)与该问卷是同一采集动线(总纲 D7「放注册流程还是首页清单」),两仓必须一起定,避免重复问。
源:该仓 README、`ui/onboarding/`。

## P8 · 依赖与未决(首页设计需跟踪)

- **`aggregate` 合成/呈现口径未定**(该仓开放问题 #1)——首页 A/B 区的「目标概览一句话」直接依赖它;
- **STATUS 模块细化中**(ATOM 如何实测 PFI 六维/体态角度/当前进阶位)——影响首页进度模块的数据可得性;
- 问卷 V1.2 重写未完成——影响 D7 拍板时机。
源:`schema/PRD.md` §10、README 当前状态。
