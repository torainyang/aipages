一、文件清单（你后面在本地或 Gemini / ChatGPT 里自己创建）

你需要 3 个核心文件，就这 3 个，足够把这个 GPT 搭起来：

McK-Slide-en.md

作用：视觉 + 逻辑 Blueprint（“A 文件”）

放在：GPT 的 Knowledge / 自己本地知识库

内容：

Canvas（1280×720，白底，外层 #EEF2FA）

字体规则（中文强制楷体，数字/Highlight 用 Georgia）

色板、Grid、Diagram 映射（2×2、From–To、Strategy House、Waterfall、Flywheel 等）

Executive Summary 的叙事规则

密度控制（每页 3 组内容 / 大表格独占一页）

Appendix & Research 的用法

Cross-slide consistency check

McK-Slide-AgentSystem-FINAL.md

作用：GPT 的 System Instruction（“B 文件”）

放在：GPT 的 System prompt 或 Knowledge + 明确引用

内容：

统一 persona 定义（EM + Partner Narrative + Visual Architect）

Workflow：Input → Storyline Compiler → Diagram Selection Engine → Extractor→Renderer → Research → HTML 生成 → Consistency Check → 安全阀（>12 页时收敛/拆 Deck）

输出策略：

首次先给文字版总结

再由你决定：只要 Exec / Exec+Detail / 要不要 Appendix

确认真后，直接生成 HTML 文件（在目标环境用 code 工具写文件）

mck_ui_library_v1.html

作用：UI 组件库（真正的前端骨架）

放在：GPT 的知识库、或你的前端项目里当模板

内容：

1280×720 slide canvas + page-shell 居中

全局 CSS 变量 / 字体栈 / grid utilities（.grid-2, .grid-3, .col-1-2, .stack-3 等）

Diagram skeleton：

.diag-strategy-house（roof + pillars + foundation）

.diag-from-to（左灰、箭头、中蓝）

.diag-2x2（十字轴 + 4 cell）

.diag-waterfall（bars + label）

.diag-driver-tree

.diag-flywheel

.diag-timeline-snake

.diag-funnel

.diag-cap-stack

.diag-swimlane

Demo slide（只是示例，方便你在浏览器打开看效果）
