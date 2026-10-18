<p align="center">
  <img src="https://img.shields.io/badge/陈鑫杰-FoamValue-blue?style=for-the-badge" alt="name" />
</p>

<h1 align="center">Hi, I'm 陈鑫杰 / FoamValue 👋</h1>

<p align="center">
  <b>资深全栈工程师 · Java 开发专家 · 15 年研发经验</b>
</p>

<p align="center">
  <a href="mailto:FoamValue@live.cn"><img src="https://img.shields.io/badge/Email-FoamValue@live.cn-EA4335?style=flat-square&logo=gmail&logoColor=white" alt="Email" /></a>
  <a href="https://chenxinjie.cn"><img src="https://img.shields.io/badge/Blog-chenxinjie.cn-4285F4?style=flat-square&logo=googlechrome&logoColor=white" alt="Blog" /></a>
  <a href="https://github.com/FoamValue"><img src="https://img.shields.io/badge/GitHub-FoamValue-181717?style=flat-square&logo=github&logoColor=white" alt="GitHub" /></a>
  <a href="https://gitee.com/FoamValue"><img src="https://img.shields.io/badge/Gitee-FoamValue-C71D23?style=flat-square&logo=gitee&logoColor=white" alt="Gitee" /></a>
  <img src="https://img.shields.io/badge/公众号-Alan手记%EF%BC%88FoamValue%EF%BC%89-07C160?style=flat-square&logo=wechat&logoColor=white" alt="WeChat" />
</p>

---

## 👨‍💻 关于我

- **15 年研发经验**，具备扎实的 B/S 架构设计与落地能力。
- 精通 **Java 后端生态体系**，同时熟练掌握 **React / Vue** 等主流前端框架，能够独立完成从系统设计到交付的全链路开发。
- **6 年以上技术团队管理经验**，善于制定技术方案、把控项目节奏，在团队建设与人才梯次培养方面积累了丰富实践。
- 热衷探索前沿技术，积极将 **AI 工具（Trae、OpenCode 配合 DeepSeek 大模型）** 深度融入日常研发流程，构建「需求即代码」工作流，从原型设计到功能实现再到容器化部署全链路提效。
- 坚持阅读与技术分享，热爱跑步与体能训练，注重持续精进与长期主义。

---

## 🛠 技术栈

| 分类 | 技术 |
| :--- | :--- |
| **后端核心** | Java · Spring Boot · Spring Cloud · Spring · MyBatis · Hibernate · JVM 调优 · 并发编程 |
| **数据库** | MySQL · PostgreSQL · Oracle · Redis · SQL 优化 · 索引策略 · 分库分表 |
| **前端技术** | JavaScript · CSS · Vue · React · Vant · Bootstrap |
| **中间件** | RabbitMQ · ActiveMQ · Nginx · Activiti · Quartz · 帆软报表 |
| **运维部署** | Linux · Docker · Nexus 私服 · MySQL 主从同步 · HSF · TXC |
| **AI 辅助** | Trae · OpenCode · DeepSeek 大模型 |

---

## 🚀 开源项目

### 📦 upload-file — 大文件传输 Java Maven 工具包
> 面向大文件**分片上传 / 断点续传 / Range 断点下载**的通用 Maven 依赖包，纯 Java 编写、兼容 JDK 8 及以上，已发布坐标 `cn.chenxinjie:upload-file:1.0.0`。

- 聚合多模块设计：核心 API、Servlet 接入、Spring Boot Starter（零配置开箱即用）与演示工程分层解耦
- 覆盖分片上传、断点续传、分片 MD5 校验、按序合并与自动清理、基于 HTTP Range 的断点下载
- 任务元数据落盘持久化，服务重启不丢进度；存储层 SPI 可扩展
- 全流程使用 Trae + DeepSeek 完成架构设计、编码实现与配套文档

**技术栈**：Java 8+ · Maven 多模块 · Gson · Servlet 3.0+ · Spring Boot Starter
🔗 [upload-file](https://github.com/FoamValue/upload-file)

### 🗂 PathFinder — Java 开源文件管理系统
> 面向单组织私有部署的文件管理系统，围绕「文件放哪、谁能看、如何找」三大问题提供统一、安全、可审计的内容文件管理能力，以 **MIT 协议**开源。

- **安全体系**：图片验证码 + 前端 RSA 加密传输 + BCrypt 存储密码，连续失败锁定、单会话登录、会话超时登出、首次登录强制改密
- **大文件传输**：复用自研 upload-file 组件，实现分片上传、断点续传、秒传、异步合并与 Range 断点下载
- **数据权限**：个人 / 部门 / 公共三级空间归属，部门树可见性继承，权限过滤服务端强制生效
- **工程能力**：真分页检索、软删除回收站、全量操作审计留痕、磁盘使用率告警、导入目录定时同步
- **容器化交付**：nginx + 后端 + Redis + MySQL 多容器编排，配套 PRD / TSDD / PLAN / TESTCASES / REVIEW 全套工程文档

**技术栈**：React 18 · TypeScript · Ant Design 5 · Vite / JDK 26 · Spring Boot 4.1 · Spring Security · Redis 9 · MySQL 8 / Docker Compose · nginx
🔗 [path-finder](https://github.com/FoamValue/path-finder)

### 🦕 认知小图鉴（studyHall）— Java 开源认知类系统
> 面向 **3-6 岁幼儿**的自然认知图鉴网页应用，打开即看、无需登录、平板优先、零后台运维，覆盖植物 / 动物 / 昆虫 / 恐龙四大板块。

- 沉浸式低龄交互：大字号大热区触控、三步到达、首尾循环切换、植物多部位切换与返回精确定位
- 预生成语音朗读：中英文各一，升级为 AAC 音频，累计产出 380 个音频文件
- **AI 接管的内容扩容通道**：不开发管理后台，内容由 AI 按约定 schema 生产、经幂等脚本灌入，扩容零代码改动
- 内容与代码规模：190 个条目、296 张图片、380 段音频
- 质量门禁：JUnit + Testcontainers 21 用例、Vitest 67 用例、Playwright E2E 47 用例，全绿方可提交；Docker Compose 五容器一键部署

**技术栈**：React 18 · Ant Design 5 · Vite / JDK 26 · Spring Boot 4.1 / MongoDB · Redis · MySQL / Node.js 内容通道 / Docker Compose
🔗 [studyHall](https://github.com/FoamValue/studyHall)

---

<p align="center"><i>保持好奇，持续精进，长期主义。</i></p>
