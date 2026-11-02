# 同类方案调研与取舍

查阅日期：2026-10-28。以下是 GitHub 一手文档阅读结果，不是安装运行或性能评测；仓库 main 分支可能变化。本 Skill 独立编写，没有复制其脚本、模板或长段指令。不能将项目 README 的宣传视为验证结果。

| 来源 | 借鉴的方法 | 本 Skill 的取舍 |
|---|---|---|
| [Anthropic PPTX Skill](https://github.com/anthropics/skills/blob/main/skills/pptx/SKILL.md) | 模板先检查，原生对象编辑，制作后检查文件与实际渲染 | 使用本环境支持的引擎；不照搬其预装依赖、脚本路径及强制每页配图的审美要求 |
| [K-Dense scientific-slides](https://github.com/K-Dense-AI/scientific-agent-skills/blob/main/skills/scientific-slides/SKILL.md) | 学术场景、讲述节奏、保留原始科学图、视觉验证 | 不硬性凑文献数量；不默认外部图像 API；以可编辑 PPT 和证据忠实为先 |
| [HKUDS Paper2Slides](https://github.com/HKUDS/Paper2Slides) | 将资料解析、内容分析、规划和制作分离，保留来源关联，可从阶段继续 | 它是项目而非同格式 Skill；只吸收流程思想。README 展示图像/PDF 产物，不能据此保证原生可编辑 PPTX |

与本地 Presentations 技能配合：复用当前工具实现及渲染流程，这个 Skill 增加学术证据、评分要求、汇报叙事和个人工作模式，不重复维护一套制作引擎。

本次原创整合：把 rubric、证据 ID、逐页目的和讲述时间串起来；区分来源事实与解释；提供仅排版模式与中英讲解选项；为地图、访谈及观察性研究加入具体规则。偏好处理原则见 personalization.md。

后续改进应来自真实论文试用，例如听众是否理解关键图、讲稿是否超时、修改是否方便。不得仅凭功能数量或这份调研声称“全宇宙最完美”。
