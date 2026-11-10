# 短视频创作者 AI 工具榜（creator-ai-tools）

面向短视频创作者的 AI 工具导航 + 对比榜单站，纯静态站，托管在 GitHub Pages，零成本运营。

- 线上地址：https://xwdeshenghuo.github.io/creator-ai-tools/
- 本地目录：`~/workspace/money-system/creator-ai-site/`

## 定位

- 按用途分四类：**数字人、配音、剪辑、文案与字幕**，每类一张对比表（工具名 / 核心功能 / 起步价 / 佣金计划 / 适合人群）
- 每个工具一个详情页：简介、核心功能、价格一览、适合人群、官网入口
- 内容原则：**如实**。价格与功能只写官网公开页面可查的信息，不编造、不写虚假实测；每页底部标注更新日期与「价格以官网为准」
- 变现：靠工具官方联盟佣金。当前运营者联盟账号尚未注册，所有外链先指向工具官网，详情页中留有 `<!-- TODO: 联盟账号注册后… -->` 注释标记，注册完成后按标记逐页替换为联盟链接。剪映/CapCut 无联盟计划，作免费工具条目如实标注，不产生佣金

## 首批工具（v1，2026-11-08）

| 工具 | 分类 | 联盟计划（已核实官方条款） |
|---|---|---|
| HeyGen | 数字人 | 20%，持续 12 个月 |
| Synthesia | 数字人 | 25% |
| ElevenLabs | 配音 | 22%，持续 12 个月 |
| Murf | 配音 | 20%，持续 24 个月 |
| OpusClip | 剪辑 | 25%（第一年） |
| Descript | 剪辑 / 文案与字幕 | $25 / 新订阅 |
| 剪映 / CapCut | 剪辑 / 文案与字幕 | 无（如实标注） |

## 更新方式

1. **价格巡检**：每月至少核对一次各工具官网 pricing 页，价格有变就改对应详情页与首页表格，并更新页面底部日期
2. **口径**：只写官网可查数据；第三方评测的价格只作线索，必须回官网确认后才写入

## 后续加工具的流程

1. 先核三件事：官网现行价格、核心功能、是否有官方联盟计划（佣金比例/周期查官方条款页）
2. 复制任一现有详情页（如 `tools/heygen.html`）改内容，存为 `tools/<slug>.html`
3. 在 `index.html` 对应分类表格加一行；如工具跨类（如 Descript），在两个分类各加一行
4. 更新本 README 的工具表，提交推送，Pages 自动重新发布

## v2 精修（2026-11-08）

- **视觉/体验**：样式表统一升级（页眉渐变、表格斑马纹、表格外层 `.tw` 小屏横向滚动、移动端断点）；首页新增「按需求快速选」卡片区；每个详情页新增「优点 / 注意点」双栏区块（内容全部由各页原有事实提炼，未引入新数据）
- **SEO**：首页与 7 个详情页补齐 canonical、Open Graph、Twitter Card；首页加 JSON-LD 工具清单；新增 `robots.txt` 与 `sitemap.xml`（含全部 8 个页面）
- **互链**：全部页面页脚加「姊妹站」区——权益货源价榜、白嫖限免清单、TG 频道 @AIShengzhang、Muse 邀请码教程仓（四条链接上线前均实测返回 200）
- **占位标注**：详情页官网按钮下方加可见说明——联盟账号尚在申请中、现为官网直达链接（占位、非联盟链接）；剪映页标注无联盟计划、本站不从该条目获佣金。HTML 内的 TODO 注释保留，注册后按注释替换并同步改掉这段说明

## 待办

- [ ] 运营者注册各工具联盟账号后，按详情页中的 TODO 注释替换联盟链接
- [ ] 上线 30 天验收：看搜索引擎收录页数与导航站收录家数（不看佣金）

## 站外发布（2026-11-10 公域扫盘新增）

- 选购指南页：https://xwdeshenghuo.github.io/creator-ai-tools/guides/how-to-choose.html
- RSS：https://xwdeshenghuo.github.io/creator-ai-tools/feed.xml
- IndexNow：密钥文件已上线，2026-11-10 已向 api.indexnow.org / Bing / Yandex 提交全部 9 个 URL（返回 200/200/202）
- Telegraph 英文介绍页：https://telegra.ph/Best-AI-Tools-for-Video-Creators-in-2026--Avatar-Voice-and-Editing-Compared-11-10
- GitHub Gist 英文版：https://gist.github.com/xwdeshenghuo/edd61fa3c23be406d010b8d0388050e3
- Awesome 清单 PR：https://github.com/0voice/awesome-ai-tools/pull/242（待审）
