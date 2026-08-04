# 健身 App 首页(Home Tab)设计竞品调研 · Strava / Fitbod / Nike Training Club

> **信息时效说明**:以下信息主要来自 2023–2026 年间的评测、官方公告与社区讨论(检索于 2026-08)。三款 App 均高频迭代 UI,模块顺序为"最近版本的典型状态",逐像素细节请以 Mobbin / 真机截图为准;凡属推断或来源不足处已标注"未确认"。另注:本次调研环境中多个信息源(Mobbin、ScreensDesign、Pratt 设计评论、部分评测站)无法直接抓取全文,相关结论基于搜索摘要交叉验证,置信度略低于全文核实。

---

## 1. Strava —— Feed-first(社交动态流)代表

### 1.1 首页自上而下模块顺序

2025 年 7 月 Strava 完成大改版:底部导航从「Feed / Explore / Record / Profile / Training」改为「**Home / Maps / Record / Groups / You**」,Home 被明确定位为"看好友动态"的社交流,你自己的数据全部迁到 You tab(来源:Cycling Weekly、road.cc、the5krunner,2025)。

Home tab 典型结构:

1. **顶栏**:Logo/页面标题 + 搜索、通知、私信(Messages,2024 年上线)入口
2. **Feed 顶部卡片区**(横向/堆叠的"cards",近年不断加码,构成事实上的"状态区"):
   - **Your Weekly Snapshot(周快照)**:本周活动数/时长/距离,并与上周同期对比,全量用户可见(2024 年起)
   - **Streak(连续训练)指标**:2025-07 社区帖证实新加在 feed 顶部
   - 不定期插入:挑战/俱乐部推荐、好友推荐、订阅推广等运营卡片(具体组合按用户状态动态变化,顺序未确认)
3. **活动动态流(主体)**:好友活动卡片,每张含头像/姓名、活动标题、关键数据(距离/配速/爬升)、路线小地图、照片、Kudos(点赞)/评论按钮;穿插好友加入挑战、俱乐部动态、赞助商挑战(Sponsored Challenges,官方广告形态)
4. **排序可选**:「Latest Activities(纯时间序)」或「Personalized(算法序)」,收藏(favorite)的运动员会被置顶加权

### 1.2 首屏第一优先级与主 CTA

- 第一优先级 = **"你和你朋友这周练了什么"**:周快照(自我状态)+ 好友动态(社交)。
- "记录一次运动"**不在**首页,而是底部导航正中的独立 **Record tab**——Strava 的答案是:高频核心动作给专属 tab,首页留给消费与互动。
- 首页主 CTA 事实上是 **Kudos/评论**(互动),而非开始运动。

### 1.3 个性化 / 状态驱动

- 周快照按你本周数据实时变化,是最主要的"状态驱动"模块;训练结束后新活动即时进入 feed 顶部,收获 kudos 形成反馈闭环。
- Personalized 排序基于互动偏好。新用户冷启动依赖好友推荐/俱乐部推荐卡片(具体新手态首页,未确认)。
- 恢复度/生理状态类信息不在首页(订阅版 Fitness/Relative Effort 在 You/训练模块)。

### 1.4 社交位置与形态 + Feed-first 优缺点

社交**就是首页本身**。用户/研究怎么说:

- **优点**:学术研究(如《Kudos make you run!》, Social Networks 2022;"Strava made me do it" 预印本 2025)证实 kudos 能显著提高跑量与频次,好友互赞形成行为传染;社区归属感、留存强。
- **缺点**:
  - 社会比较与压力:研究与 road.cc 报道指出,对易做"向上比较"、低自我关怀人群(尤其女性、伤病期用户)有自尊/心理负面影响;有用户称周快照"first thing you see, makes me feel bad",且**不可关闭**,被批"更像社交媒体的坏部分"。
  - 2017 年改算法流曾引发 #BringBackChronological 大规模抗议,2020 年被迫恢复时间序——feed-first 产品动排序即触雷。
  - 2025 社区帖:官方不断往 feed 顶部堆新卡片(streak 等),"app 迅速失去简洁性",用户要求可自定义/重排卡片而不得。

### 1.5 商业化门控在首页的呈现

- 免费版可完整记录与看 feed;路线推荐、训练计划、Live Segments、国家排行等锁在订阅($79.99/年),feed 内以试用推广卡、功能点上的锁标呈现(锁标具体样式未确认)。
- **Sponsored Challenges** 是原生广告,直接混入 feed/Groups;官方称约 1/3 用户视其为正面体验。
- 评测(BarBend 2026 等)对免费版价值评价分化,"最好的功能都在墙后"是常见抱怨。

### 1.6 一个最值得借鉴 + 一个公认槽点

- **借鉴**:「Record」独立成底部中央 tab,把"消费社交流"与"发起运动"彻底解耦——首页可以纯粹做留存与互动,不牺牲核心动作触达。
- **槽点**:首页顶部运营卡片不断膨胀且不可关闭/不可重排(周快照、streak),把状态展示做成了焦虑制造机,社区反弹持续 2024–2025。

---

## 2. Fitbod —— "今日该练这一节"(AI 力量训练)代表

### 2.1 首页(Workout tab)自上而下模块顺序

Fitbod 打开即落在 **Workout(训练)tab**,整个首页就是"为你生成好的今天这节课":

1. **顶部中央:Gym Profile 选择器**(官方帮助中心确认位置)——切换"家里/健身房/出差"等器械档案,切换后当日训练即时重算
2. 周目标/连续性指示(streak、每周第几练;确切样式未确认)
3. **今日训练卡**:目标肌群标签(如 Chest & Triceps)、预计时长、难度;下方为**完整练习清单**——每个动作显示缩略图 + 建议组数×次数×重量(AI 按你的历史与恢复度推荐),可单个替换(swap)、增删、标"多练/少练/排除"
4. 恢复度入口:**肌肉热力图/身体图**显示各肌群疲劳-恢复百分比(评测普遍确认此"recovery heatmap"存在;当前版本它在首页内嵌还是在 Recovery/Body 分页,未确认——多数评测描述为独立 tab 页,首页以"练恢复好的肌群"结果体现)
5. **大按钮「Start Workout」**:进入逐动作引导+计时+记录流程
6. 底部导航另有 Body(Results/Strength Score、体测)、Log(历史)等 tab;2025 年 Results 页改版,加入实时 **Strength Score**、肌群强度分、Records(PR/里程碑庆祝)

### 2.2 首屏第一优先级与主 CTA

- 第一优先级 = **"今天该练的那一节"**,零选择压力:打开即见已生成的完整训练。
- 主 CTA 明确单一:**Start Workout**。浏览/自选是次要路径(可自建 workout,但产品不引导)。

### 2.3 个性化 / 状态驱动(Fitbod 特色)

- **肌群恢复模型**是核心卖点:算法追踪每个肌群的训练量与休息时间,今日训练围绕"已恢复的肌群"生成,热力图向用户解释"为什么今天练这个"——把黑盒推荐做成了可视化理由。
- **训练后状态变化**:完成训练→该肌群变"疲劳"色→下次打开时今日推荐已重算;并弹 PR/Records 庆祝、Strength Score 增长(2025 版强化)。
- 反馈闭环:对整节课/单个动作标"太容易/太难",影响后续生成。
- **新用户**:onboarding 问目标、经验、器械→立即生成第一节;**免费额度为 3 次生成的训练(总共 3 次,非每周)**,之后强制订阅。

### 2.4 社区/社交

- 首页**没有社交模块**,产品整体几乎无社区(仅分享导出、Apple Health 等集成)。这是刻意取舍:单人闭环工具。无"好友动态"意味着无比较压力,但也少了 Strava 式留存钩子。

### 2.5 商业化门控在首页的呈现

- **硬门控**:3 次免费训练用完后,首页的核心内容(生成的今日训练)本身就在付费墙后——试用即产品,paywall 出现在你已建立习惯的位置。订阅约 $12.99–15.99/月 或 ~$80–96/年(各评测口径略异)。
- 无广告、无内购杂音;评测普遍认为"免费版基本不可用,但试用转化设计诚实"。

### 2.6 一个最值得借鉴 + 一个公认槽点

- **借鉴**:**用恢复度热力图给推荐"讲理由"**——"今天练背,因为胸还没恢复"一句可视化解释,同时解决了信任、教育与差异化;加上 Gym Profile 一键切换场景、训练即时重算,是"状态驱动首页"的教科书。
- **槽点**:算法选动作有时**随机感/怪异**(Reddit 与多篇评测反复提到:accessory 动作偏多、顺序不合常规编排、长期渐进超负荷逻辑弱于固定计划),重度训练者需要频繁手动 swap 才像样;此外 3 次免费额度过于苛刻也是差评常客(App Store 评论区,2024–2026)。

---

## 3. Nike Training Club(NTC)—— 内容库/货架型参照

### 3.1 首页(Home tab)自上而下模块顺序

底部导航(iOS 近年版本):**Home / Workouts(Browse) / Activity / Profile**(具体命名随版本变化,未确认最新)。Home tab 是编辑运营的内容货架:

1. 顶部问候/品牌区(未确认具体样式)
2. **最新/主推内容大卡**:评测称"打开先看到最新上架内容"(What's New 性质)
3. **Today's Picks / For You**:按偏好、历史与时段推荐的横向 workout 轮播
4. **Featured Programs**:多周训练计划(4–8 周 program)入口
5. **Collections**:主题合集货架(部位/器械/时长/瑜伽/孕产等)
6. 健康生活内容:营养、恢复、心态类文章与短视频(Well-being 内容)
7. (穿插)教练/名人课程、与 Nike 生态的联动位(未确认当前是否有商品导流)

Workouts/Browse tab 才是全量库:按肌群、器械、时长、强度筛选 200+ 视频课。Activity tab 显示历史与"奖杯"。

### 3.2 首屏第一优先级与主 CTA

- 第一优先级 = **内容货架**("看看有什么新课/推荐课"),主 CTA 是**从轮播里挑一节课开始**——是"逛-挑-练"模式,而非 Fitbod 的"已替你决定"或 Strava 的"看朋友"。
- 若已加入 Program,当日课程会前置(在 Home 顶部展示进行中的 program 进度;确切位置未确认)。

### 3.3 个性化 / 状态驱动

- 仅有轻量推荐(Today's Picks 按历史/时段),**无自适应**:不按表现调难度、不做恢复度概念、不学习你的负重——被几乎所有评测点名为最大短板(dr-muscle、madmuscles-review、Garage Gym Reviews 等,2023–2026)。
- 训练后:Activity 里加一条记录 + 奖杯;首页内容基本不因你的完成情况发生结构性变化(除 program 进度推进)。
- 新老用户差异主要体现在推荐轮播内容,货架结构不变。

### 3.4 社区/社交

- 首页**无社交流**。无好友、无点赞;社交仅限分享到外部平台(与同门 Nike Run Club 的排行榜/挑战相比更弱)。定位为"免费内容健身房",社区不是其留存抓手,品牌与内容质量才是。

### 3.5 商业化门控在首页的呈现

- **2020 年起 Premium 完全免费**,首页无付费墙、无广告轰炸——评测普遍惊叹"免费版就是完整版"(Tom's Guide、Reviewed)。
- 隐性商业化:NTC 是 Nike 品牌/会员生态的获客与留存工具(注册即 Nike Member,与电商打通);首页是否有直接卖货位,未确认(历史上偏克制)。

### 3.6 一个最值得借鉴 + 一个公认槽点

- **借鉴**:**零门控 + 高制作水准内容货架**建立的信任与品牌好感:免费策略消除首页一切转化噪音,使首页可以 100% 服务于"让你今天想练一节"——对内容型首页,货架分层(新品→为你推荐→计划→合集→轻内容)的信息架构本身也是标准范式。
- **槽点**:**无个性化、无进阶追踪**:不记重量明细、看不到力量进步曲线、课程一刀切不随你成长(one-size-fits-all),进阶用户很快"毕业"流失;Pratt 设计评论(2023)与多篇评测还提到内容量大导致的**发现/导航负担**(货架太深,找到"适合我的下一节"成本高)。

---

## 4. 横向速览

| 维度 | Strava | Fitbod | NTC |
|---|---|---|---|
| 首页范式 | 好友动态流 + 顶部状态卡 | 今日 AI 训练(单一 CTA) | 编辑内容货架 |
| 主 CTA | Kudos/互动(记录另设中央 tab) | Start Workout | 挑一节课开始 |
| 状态驱动 | 周快照/Streak(被诟病制造焦虑) | 肌群恢复热力图驱动生成(标杆) | 几乎无 |
| 社交 | 即首页本体 | 无 | 无 |
| 商业化 | 功能锁+试用卡+原生赞助挑战 | 3 次免费后核心即付费墙 | 完全免费 |
| 核心教训 | 状态卡不可关闭/不断堆卡 → 反弹 | 推荐要"讲理由"才被信任 | 无个性化 → 进阶用户流失 |

**综合启示**:三者验证了三条互斥主线各自的天花板——若做"今日推荐训练"首页(Fitbod 线),关键是给推荐可视化理由(恢复度)并保持 CTA 唯一;社交若引入首页,需给用户对比较类模块的开关权(Strava 教训);运营卡片区要有数量纪律与用户可控性。

## Sources

- [Cycling Weekly – Strava 新导航改版](https://www.cyclingweekly.com/news/product-news/a-new-look-for-strava-app-with-updates-to-the-navigation-bar-498270) · [the5krunner – Strava App Redesign (2025-07)](https://the5krunner.com/2025/07/16/strava-app-redesign/) · [road.cc – Weekly Snapshot "makes me feel bad"](https://road.cc/content/tech-news/stravas-weekly-snapshot-makes-me-feel-bad-307315)
- [Strava 社区 – Home tab 顶部新 UI 抱怨 (2025-07)](https://communityhub.strava.com/strava-features-chat-5/new-strava-ui-layout-on-to-of-the-feed-in-the-home-tab-10870) · [Strava Support – Feed Ordering](https://support.strava.com/hc/en-us/articles/115001183630-Feed-Ordering) · [TidBITS – 恢复时间序 feed (2020)](https://tidbits.com/2020/03/06/strava-finally-listens-to-its-users-brings-back-chronological-feed/)
- [Kudos make you run!(Social Networks, 2022)](https://www.sciencedirect.com/science/article/pii/S0378873322000909) · ["Strava made me do it" 预印本](https://sciety.org/articles/activity/10.31234/osf.io/4gajv_v1) · [BarBend – Strava Review 2026](https://barbend.com/strava-app-review/) · [Strava Business – Sponsored Challenges](https://business.strava.com/challenges)
- [Fitbod 官方 – Gym Profile](https://fitbod.me/blog/your-gym-profile/) · [Fitbod – Strength Score / Results 改版](https://fitbod.me/blog/how-fitbod-tracks-your-strength-progress-with-real-time-metrics-and-scores/) · [Fitness Drum – Fitbod Review](https://fitnessdrum.com/fitbod-review/) · [Fittest Travel – Fitbod Review](https://www.fittesttravel.com/blog/2019/10/3/fitbod-app-review) · [Indie Hackers – Fitbod 2026 实测(免费 3 次训练)](https://www.indiehackers.com/post/fitbod-app-review-2026-honest-take-after-real-testing-45d5f07a1b) · [TechRadar – Fitbod Review](https://www.techradar.com/health-fitness/fitbod-app-review) · [HotelGyms – Fitbod 使用指南](https://www.hotelgyms.com/blog/how-to-use-the-fitbod-app)
- [MakeUseOf – NTC 使用指南](https://www.makeuseof.com/how-use-nike-training-club-app-next-level-fitness/) · [Reviewed – NTC Review](https://www.reviewed.com/health/content/nike-training-club-review-workout-app) · [Garage Gym Reviews – NTC Review 2026](https://www.garagegymreviews.com/nike-training-club-review) · [Pratt IXD – NTC 设计评论 (2023)](https://ixd.prattsi.org/2023/09/design-critique-nike-training-club-iphone-app/) · [dr-muscle – NTC Review](https://dr-muscle.com/nike-training-club-app-review/) · [Tom's Guide – NTC Review](https://tomsguide.com/reviews/nike-training-club-app)
