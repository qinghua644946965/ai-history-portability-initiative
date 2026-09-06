# 项目定位 / Project positioning

**User Initiative / Open Discussion Draft**
**现实对照核查日期 / Comparison reviewed: 2026-09-06**

## 中文

本项目不是首创、优先权或独占概念声明。名称、公开日期和文档归档用于识别与引用，不证明率先提出或填补行业空白。本项目保留问题洞察与验证价值，不以“尚无人实现”为成立前提。它不是行业标准、完整市场调查或已验证的产品优势声明。

### 真正关注的问题

用户如何通过正式授权、只读分页和稳定增量定位，持续取得自己有权访问的 AI 会话与任务记录？倡议聚焦持续数据访问，不把数据可携带、导出或增量同步当作新概念，也不要求用户建设知识库。

### 现实对照的解释范围

下表列出已核查官方文档中的相邻能力，不是完整竞品清单。文档记载的能力、配置后可用的机制、本仓库原型与端到端实测应分别标注；本次未对外部产品做部署测试。未核查的能力记为未知，不能记为不存在。基础能力已有工程实现，不表示每一种 Agent 产品或组合都已成熟。

## English

This project makes no claim of invention priority or exclusive ownership of a concept. Its name, publication date, and archive support identification and citation, not a claim to be first or to fill an industry void. Its value rests on problem analysis and validation rather than an assertion that nobody has implemented the idea. It is not an industry standard, exhaustive market survey, or demonstrated product advantage.

### The actual question

How can users continuously obtain AI conversation and task records they may access through formal authorization, read-only pagination, and stable incremental positioning? The initiative focuses on ongoing data access; portability, export, and incremental synchronization are existing concepts, and a knowledge base is not required.

### How to read the comparison

The table records adjacent capabilities described in official documentation, not an exhaustive competitor list. Distinguish documented capability, configured functionality, this repository’s prototype, and end-to-end measurements. No external product deployment tests were performed for this review. Unchecked means unknown, not absent. Established foundations do not imply that every agent product or combination is mature.

## 已有基础与边界 / Existing foundations and boundaries

| 方向 / Area | 官方来源 / Official source | 已有能力 / Existing capability | 对照边界 / Comparison boundary |
| --- | --- | --- | --- |
| Data portability | [Data Transfer Project](https://github.com/dtinit/data-transfer-project) | 跨服务数据迁移框架 / Cross-service data transfer framework | 不证明覆盖所有 AI 记录或持续增量读取 / Does not establish all AI record coverage or ongoing incremental reads |
| User-controlled data | [Solid](https://solidproject.org/about) | 数据自主控制的相邻方向 / Adjacent work on user-controlled data | 不等于某厂商已开放所请求的接口 / Does not establish a requested provider interface |

## 验证与持续修订 / Validation and revision

按具体产品和入口记录可取得的数据范围、授权、分页、增量、编辑删除语义、附件与限流。比较全量导出与增量访问的完整性和人工投入。现有案例仍是待核验用户报告，不能由检索失败推断删除或全行业缺口。

Record accessible data, authorization, pagination, incremental access, edit/deletion semantics, attachments, and limits for each product and interface. Compare completeness and manual effort for full exports and incremental access. Existing cases remain user reports pending verification; retrieval failure does not prove deletion or an industry-wide gap.

每次重要修订补充具体产品、版本/日期、访问入口、数据与权限范围、官方来源、复现步骤、结果及限制。先判断能否复用已有工具，再说明本项目增加了什么以及代价。发现已有方案覆盖需求时，更新对照、缩小范围或转为参考实现/用户倡议；不为了维护原创性而人为扩大缺口。保留现有免责声明、失败记录和证据等级。

For each substantive revision, record the product, version/date, interface, data and permission scope, official sources, reproduction steps, outcomes, and limits. Evaluate reuse before adding a layer, and explain its cost. When an existing solution covers the need, update the comparison, narrow scope, or focus on a reference implementation or user initiative. Do not manufacture gaps to defend originality. Preserve existing caveats, failures, and evidence levels.
