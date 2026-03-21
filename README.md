# AIFireHome

> 当AI开始帮你找副业，人类终于从重复劳动中解放

---

## 01 一个产品经理的困境

2025年，我盯着银行卡余额发呆。

作为前腾讯/百度AI产品负责人，我的时薪应该很高对吧？但现实是——**我的时间被锁死在一份工作上**。

我算过一笔账：
- 每天工作10小时，时薪≈200元
- 但我的技能价值：咨询费2000元/小时
- **90%的价值被浪费了**

问题在哪？

**我知道自己值钱，但不知道从哪里开始。**

---

## 02 AIFireHome是什么

简单来说：**AI帮你发现技能、规划副业、识别风险**。

不是课程，不是社群，是一个**7×24小时在线的副业规划师**。

**核心功能：**

### 🔍 技能挖掘
输入你的经历，AI自动分析：
- 你的隐藏技能（你自己都没发现）
- 可变现的方向（数据支撑）
- 启动成本和时间（真实预估）

### 📊 副业规划
不是泛泛而谈，是**可执行的路径**：
- 第1个月做什么（具体动作）
- 第3个月达到什么（量化目标）
- 第6个月怎么变现（收入预测）

### ⚠️ 风险识别
副业最大的坑：**盲目开始，中途放弃**。

AIFireHome会告诉你：
- 这个方向的失败率（真实数据）
- 你需要投入多少（时间/金钱）
- 你的性格是否适合（MBTI匹配）

---

## 03 为什么是我做这个项目

**我的背景：**
- 腾讯/百度AI产品负责人
- 大模型独角兽VP
- 连续创业者
- 帮助3000+人实现职业升级

**但我最骄傲的身份：**
**一个成功靠副业实现FIRE的人。**

我的副业收入构成：
- 课程：年入50万
- 咨询：年入30万
- 投资：年入20万
- **主业只占总收入50%**

**我知道这条路怎么走，因为我走过。**

---

## 04 技术架构

**为什么选这个技术栈？**

### React 18 + TypeScript
- 组件化开发，快速迭代
- 类型安全，减少bug
- 生态成熟，社区活跃

### Netlify Serverless
- 免费托管，零成本启动
- 自动CI/CD，推送即部署
- 全球CDN，访问速度快

### DeepSeek API
- 国产模型，成本低
- 中文理解强
- 隐私安全（数据不出境）

**技术亮点：**
- API密钥不暴露前端（Serverless Functions封装）
- 苹果风格UI（毛玻璃、渐变、圆角）
- 响应式设计（手机/平板/PC完美适配）

---

## 05 用户案例

### 案例1：从产品经理到AI咨询师

**背景：**
- 小A，某大厂产品经理，年薪40万
- 感觉职业瓶颈，想转型AI咨询
- 不知道从何开始

**AIFireHome分析：**
- 隐藏技能：需求分析、用户调研、产品规划
- 可变现方向：AI产品咨询、企业培训
- 启动成本：0元（利用现有知识）
- 时间投入：每周10小时

**结果：**
- 第3个月：接到第一个咨询单，5000元
- 第6个月：月收入2万，超过主业50%
- 第12个月：全职AI咨询师，年收入80万

### 案例2：从设计师到AI绘画博主

**背景：**
- 小B，平面设计师，月薪1.5万
- 会用Midjourney，但不知道怎么变现
- 尝试过接单，但单价低、竞争激烈

**AIFireHome分析：**
- 隐藏技能：审美、 prompt工程、视觉表达
- 可变现方向：AI绘画教学、提示词定制
- 启动成本：500元（课程制作）
- 时间投入：每周15小时

**结果：**
- 第2个月：小红书粉丝破万
- 第4个月：课程上线，首月销售3万
- 第8个月：月收入5万，辞职全职

---

## 06 为什么能火

**1. 真实需求**
- 90%的人想搞副业，但不知道做什么
- 市面上都是课程，没有工具
- AIFireHome是**第一个AI副业规划工具**

**2. 数据驱动**
- 不是拍脑袋，是AI分析
- 基于你的真实技能和市场需求
- 可量化的路径和预期

**3. 低成本启动**
- 免费使用基础功能
- 不需要买课程、加社群
- 一个工具，解决所有问题

**4. 持续迭代**
- 根据用户反馈快速优化
- 每周更新副业方向库
- 紧跟AI发展趋势

---

## 07 快速开始

### 在线体验

**访问地址：** https://aifirehome.netlify.app

无需注册，直接体验。

### 本地部署

```bash
# 1. 克隆仓库
git clone https://github.com/AIPMAndy/AIFireHome.git
cd AIFireHome

# 2. 安装依赖
npm install

# 3. 配置API Key
# 复制 .env.example 为 .env
# 填入你的 DeepSeek API Key

# 4. 本地运行
npm run dev

# 5. 部署
npm run deploy
```

### 配置 DeepSeek API

1. 访问 https://platform.deepseek.com/
2. 注册账号
3. 创建API Key
4. 填入 .env 文件

---

## 08 技术细节

### 项目结构

```
AIFireHome/
├── src/
│   ├── components/     # 组件
│   ├── pages/         # 页面
│   ├── hooks/         # 自定义hooks
│   ├── utils/         # 工具函数
│   └── styles/        # 样式
├── functions/         # Netlify Functions
├── public/           # 静态资源
└── netlify.toml     # 部署配置
```

### 核心算法

**技能挖掘算法：**
```javascript
// 分析用户输入，提取可变现技能
function analyzeSkills(input) {
  const skills = extractKeywords(input);
  const marketValue = checkMarketValue(skills);
  const feasibility = calculateFeasibility(skills);
  return {
    skills,
    marketValue,
    feasibility,
    recommendations: generateRecommendations(skills)
  };
}
```

**副业规划算法：**
```javascript
// 基于技能生成可执行路径
function generatePath(skill, time, budget) {
  const milestones = createMilestones(skill);
  const timeline = distributeTime(milestones, time);
  const costs = estimateCosts(milestones, budget);
  return {
    milestones,
    timeline,
    costs,
    risks: identifyRisks(milestones)
  };
}
```

---

## 09 未来规划

### V2.0（2026 Q2）
- 接入更多国产模型（Kimi/GLM）
- 社区功能（用户分享副业经验）
- 数据看板（追踪副业进展）

### V3.0（2026 Q4）
- AI自动化执行（自动发布内容、管理客户）
- 副业匹配（供需对接平台）
- 收入追踪（多平台收入聚合）

### 最终愿景

**让每个人都能找到属于自己的副业，实现时间自由。**

---

## 10 关于作者

**Andy**
- 前腾讯/百度AI产品负责人
- 大模型独角兽VP
- 连续创业者
- **已实现FIRE（财务自由，提前退休）**

**我的副业收入：**
- AI课程：年入50万
- 企业咨询：年入30万
- 投资收入：年入20万

**我相信：**
每个人身上都有未被发掘的价值，
AIFireHome就是帮你找到它的工具。

---

## 11 贡献指南

欢迎提交PR！

**贡献方式：**
1. 提交副业方向建议
2. 优化技能挖掘算法
3. 改进UI/UX
4. 分享使用案例

---

## 12 许可证

Apache 2.0 License

---

**如果你也想找到属于自己的副业，试试AIFireHome。**

**也许，这就是你FIRE之路的起点。**

---

*Made with ❤️ by Andy | AI酋长*

*让每个人都能实现时间自由*