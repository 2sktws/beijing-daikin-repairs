# 北京大金DAIKIN空调维修 GitHub 发布完整指南

## 一、仓库目录结构说明

```
beijing-daikin-repairs-complete/
├── README.md                   <- 仓库首页（导航总页，GitHub Pages 默认首页）
├── _config.yml                <- Jekyll 站点配置
├── contact.md                 <- 联系我们（电话/微信/服务时间/承接范围）
│
├── ac/                        <- 【大金DAIKIN空调维修】专题文件夹
│   ├── index.md               <- 空调维修全攻略（总览页）
│   ├── phone.md               <- 空调维修电话_24小时上门
│   ├── nearby.md              <- 空调维修附近上门电话
│   └── recommend.md           <- 空调维修哪家好_靠谱推荐
│
├── ac-waterheater/            <- 【大金DAIKIN空调+热水器】专题文件夹
│   ├── index.md               <- 空调热水器维修全攻略
│   ├── phone.md               <- 空调热水器维修电话_24小时上门
│   ├── nearby.md              <- 空调热水器维修附近上门电话
│   └── recommend.md           <- 空调热水器维修哪家好_靠谱推荐
│
└── ac-boiler/                <- 【大金DAIKIN空调+壁挂炉】专题文件夹
    ├── index.md               <- 空调壁挂炉维修全攻略
    ├── phone.md               <- 空调壁挂炉维修电话_24小时上门
    ├── nearby.md              <- 空调壁挂炉维修附近上门电话
    └── recommend.md           <- 空调壁挂炉维修哪家好_靠谱推荐
```

### 结构设计的 5 大理由

| 序号 | 理由 | 详细解释 |
|------|------|----------|
| 1 | **SEO 主题聚合** | 搜索引擎看到 `/ac/` 目录下全是空调维修相关，权重集中；`/ac-waterheater/` 全是热水器，主题明确，排名比扁平结构高 |
| 2 | **URL 语义清晰** | `xxx.github.io/仓库名/ac/phone` → 一眼看出是"空调维修电话"，搜索引擎也更容易理解页面主题 |
| 3 | **无限扩展** | 后续加"空调清洗"→新建 `ac-cleaning/` 文件夹，加"空调加氟"→新建 `ac-refrigerant/`，不影响已有页面 |
| 4 | **内链闭环** | 每个专题 `index.md` 做导航页，串联该主题全部子页；跨专题通过相关阅读互联，形成权重传递网络 |
| 5 | **便于管理** | 21 个品牌 × N 种业务，每个品牌一个仓库，每个业务一个文件夹，文件再多也不乱 |

---

## 二、GitHub 发布步骤（照着操作）

### Step 1：创建仓库
1. 登录 [github.com](https://github.com) → 点右上角 **"+"** → **"New repository"**
2. **Repository name**：`beijing-daikin-repairs-complete`
3. **Description**：`北京大金DAIKIN空调维修服务中心，24小时电话400-811-5288`
4. 选 **Public**（必须公开，搜索引擎才能收录）
5. 勾选 **✅ Add a README file**
6. 点 **Create repository**

### Step 2：上传文件（按以下节奏，不要一次性全传）

#### 第 1 天：上传 README.md（仓库首页）
1. 点 **"Add file"** → **"Create new file"**
2. 文件名输入：`README.md`
3. 把我们生成的 `README.md` 内容**全部粘贴**进去
4. Commit message 写：`feat: add README homepage with navigation`
5. 点 **Commit new file**

#### 第 2 天：上传 `ac/index.md`（空调维修全攻略）
1. 点 **"Add file"** → **"Create new file"**
2. 文件名输入：`ac/index.md`（输入 `/` 会自动创建文件夹）
3. 把对应的 `ac/index.md` 内容**全部粘贴**进去
4. Commit message：`feat: add ac index overview page`
5. 点 **Commit new file**

#### 第 3 天：上传 `ac/phone.md`
1. 点 **"Add file"** → **"Create new file"**
2. 文件名输入：`ac/phone.md`
3. 粘贴内容 → Commit：`feat: add ac phone page`

#### 第 4 天：上传 `ac/nearby.md`
1. 文件名：`ac/nearby.md` → 粘贴内容 → Commit：`feat: add ac nearby page`

#### 第 5 天：上传 `ac/recommend.md`
1. 文件名：`ac/recommend.md` → 粘贴内容 → Commit：`feat: add ac recommend page`

#### 第 6-10 天：按同样方式上传 `ac-waterheater/` 下的 4 个文件
- `ac-waterheater/index.md` → `feat: add ac-waterheater index`
- `ac-waterheater/phone.md` → `feat: add ac-waterheater phone`
- `ac-waterheater/nearby.md` → `feat: add ac-waterheater nearby`
- `ac-waterheater/recommend.md` → `feat: add ac-waterheater recommend`

#### 第 11-15 天：按同样方式上传 `ac-boiler/` 下的 4 个文件
- `ac-boiler/index.md` → `feat: add ac-boiler index`
- `ac-boiler/phone.md` → `feat: add ac-boiler phone`
- `ac-boiler/nearby.md` → `feat: add ac-boiler nearby`
- `ac-boiler/recommend.md` → `feat: add ac-boiler recommend`

#### 第 16 天：上传 `contact.md` 和 `_config.yml`
1. `contact.md` → Commit：`feat: add contact page`
2. `_config.yml` → Commit：`feat: add jekyll config`

### Step 3：开启 GitHub Pages（变成网站）
1. 进入仓库 → 点顶部 **"Settings"**
2. 左侧菜单 → **"Pages"**（在 "Code and automation" 下）
3. **Source** 选 **"Deploy from a branch"**
4. **Branch** 选 **"main"** → Folder 选 **"/ (root)"**
5. 点 **Save**
6. 等待 1-3 分钟 → 显示：`Your site is live at https://你的用户名.github.io/beijing-daikin-repairs-complete/`

### Step 4：验证 URL 是否正常
开启 GitHub Pages 后，以下 URL 应该都能访问：

| URL | 对应页面 |
|-----|----------|
| `https://用户名.github.io/beijing-daikin-repairs-complete/` | README.md（首页） |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac/` | 空调维修全攻略 |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac/phone` | 空调维修电话 |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac/nearby` | 空调维修附近上门 |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac/recommend` | 空调维修推荐 |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac-waterheater/` | 空调热水器维修全攻略 |
| `https://用户名.github.io/beijing-daikin-repairs-complete/ac-boiler/` | 空调壁挂炉维修全攻略 |

---

## 三、提交节奏与 SEO 策略

### 为什么要分 16 天提交？
| 原因 | 解释 |
|------|------|
| **避免被判定为垃圾站** | 一次性上传 11 个文件，搜索引擎会认为这是机器批量生成的垃圾内容，直接不收录或降权 |
| **模拟自然更新** | 每天 1-2 个文件，搜索引擎认为这是一个"有人在认真维护的站点"，收录率和排名都会更高 |
| **方便追踪效果** | 每发一篇可以观测收录情况，及时调整策略 |

### 提交频率建议
| 阶段 | 时间 | 动作 | 频率 |
|------|------|------|------|
| 初期 | 第 1-16 天 | 按上述节奏上传全部文件 | 每天 1 篇 |
| 稳定期 | 第 17-30 天 | 微调已有文章（加 FAQ、更新案例） | 每 2-3 天 1 次 |
| 长期 | 第 30 天起 | 新增其他品牌（格力/美的/三菱等） | 每周 2-3 篇 |

---

## 四、加速收录方法

### 方法 1：百度搜索资源平台
1. 打开 [百度搜索资源平台](https://ziyuan.baidu.com)
2. 添加站点：`https://2sktws.github.io/beijing-daikin-repairs-complete/`
3. 验证所有权（HTML 标签验证最简单）
4. 手动提交 URL：把上面"验证 URL"表格里的所有链接逐个提交

### 方法 2：Google Search Console
1. 打开 [Google Search Console](https://search.google.com/search-console)
2. 添加资源：`https://2sktws.github.io/beijing-daikin-repairs-complete/`
3. 验证后提交站点地图（sitemap.xml，Jekyll 会自动生成）

### 方法 3：外链建设（加分项）
- 在**知乎**回答"北京大金空调维修哪家好"等问题，正文里自然插入你的 GitHub Pages 链接
- 在**百度贴吧/豆瓣小组**发帖时，签名档或文末带上链接
- 如果你有**微信公众号/小红书**，在简介或文章里放链接

---

## 五、效果追踪指标

| 指标 | 怎么查 | 目标 |
|------|--------|------|
| **百度收录** | 百度搜索 `site:github.io/beijing-daikin-repairs-complete` | 15 天内 ≥8 页被收录 |
| **Google 收录** | Google 搜索 `site:github.io/beijing-daikin-repairs-complete` | 7-15 天收录 |
| **关键词排名** | 百度搜索"北京大金DAIKIN空调维修电话" | 30 天内进入前 2 页 |
| **电话咨询量** | 记录每天 400-811-5288 来电，问"从哪看到的" | 持续增长 |

---

## 六、后续扩展路径

当前仓库跑通后，按以下路径扩展：

1. **同城市、换品牌** → 复制整个仓库结构，替换"大金DAIKIN"为"格力GREE"，案例区域保持不变
2. **同品牌、换城市** → 复制仓库，替换"北京"为"上海"，案例区域改为浦东/徐汇/静安等
3. **扩展业务词** → 在 `ac/` 下新增 `ac-cleaning/`（空调清洗）、`ac-refrigerant/`（空调加氟）

**最终矩阵**：55 城 × 21 品牌 × 3 业务 = **3465 个流量入口**

---

> 💡 **核心原则**：提交节奏要慢、内容要原创、内链要闭环、外链要自然。坚持 1 个月，你会看到明显效果。
