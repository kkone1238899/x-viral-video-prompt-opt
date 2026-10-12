# 提示词优化

> prompt 写不好，出片靠运气？这个库收集视频 prompt 优化 skills，每条都写清楚能帮你解决什么、怎么用它搞钱。
>
> A curated collection of prompt optimization prompts & skills for viral short videos, gathered from practitioners sharing on X.
> 
> Each entry answers two questions: what problem it solves (and who it's for), and how to make money with it.
> 
> Star counts verified via GitHub API on 2026-10-12. Continuously updated.

## 条目

### Prompt Optimizer

**核心提炼**
- 解决什么问题：手写的 prompt 又糙又玄，AI 输出质量不稳定——缺一个把想法打磨成好 prompt 的工具。
- 核心用法（5 步）：1) 打开在线版 prompt.always200.com，或装桌面版 / Chrome 插件 / Docker 自部署；2) 粘贴自己写的 prompt，选模型（OpenAI / Gemini / DeepSeek / Grok 等）；3) 一键优化，多轮迭代打磨；4) 用分析 / 对比评测看是不是真的变好了；5) 存成可复用的 prompt 资产。还有图像生成模式（文生图 / 图生图，支持 Seedream / Gemini），做视频前可先出关键帧。
- 什么时候用 / 常见坑：任何模型出片翻车，先拿它"审一遍 prompt"；纯客户端直连 AI 服务商、数据不经过中间服务器，API key 需要自己配。

**适用场景**：所有写 prompt 的人、做 prompt 咨询或教学的人。

**怎么用它搞钱**：提示词优化服务 / 教学 / 卖 prompt 资产包。

**来源**：[linshenkx/prompt-optimizer](https://github.com/linshenkx/prompt-optimizer) · ⭐37657 · 更新于 2026-10-09

### PromptEnhancer

**核心提炼**
- 解决什么问题：英文 prompt 写得太糙，生图模型"听不懂"、出图偏离意图——需要一个改写器把 prompt 重构成模型好理解的结构。
- 核心用法（4 步）：1) `pip install -r requirements.txt` 装好环境；2) 从 Hugging Face 下载 PromptEnhancer-7B（13GB，质量和效率最均衡）；3) 输入原始 prompt，模型做思维链改写——保留原意，输出结构化增强版；4) 拿增强后的 prompt 去生图或做图生图编辑。
- 什么时候用 / 常见坑：做视频分镜图 / 关键帧之前先过一遍增强器；官方是腾讯混元团队的 CVPR 2026 项目，偏研究向，跑 7B / 32B 模型需要 GPU。

**适用场景**：做 AI 视频分镜 / 关键帧的创作者、技术向 prompt 玩家。

**怎么用它搞钱**：分镜 / 关键帧代做服务 / 技术教学。

**来源**：[Hunyuan-PromptEnhancer/PromptEnhancer](https://github.com/Hunyuan-PromptEnhancer/PromptEnhancer) · ⭐3787 · 更新于 2026-08-18

### seedance2-skill

**核心提炼**
- 解决什么问题：不会写 Seedance 2.0 视频提示词——不清楚输入约束、@ 引用语法、运镜语言，盲试烧积分。
- 核心用法（3 步）：1) `npx skills add dexhunter/seedance2-skill`，或复制 SKILL.md 到 `~/.claude/skills`；2) 把创意需求告诉 AI agent（广告 / 短剧 / MV 等类型）；3) agent 按官方文档沉淀的写法（输入约束、@ 引用、运镜语言、结构模板）生成提示词，拿去 Seedance 生成。有中英两个版本。
- 什么时候用 / 常见坑：Seedance 2.0 项目开工前先装它当"官方手册外挂"；内容基于字节官方文档，2.5 的新写法不一定覆盖。

**适用场景**：用 Seedance 做商单 / 广告的创作者、给客户写提示词的运营者。

**怎么用它搞钱**：即梦商单 / 教学。

**来源**：[dexhunter/seedance2-skill](https://github.com/dexhunter/seedance2-skill) · ⭐4256 · 更新于 2026-09-19

### IMGPrompt

**核心提炼**
- 解决什么问题：脑子里有画面但写不出英文提示词——不知道"丁达尔效应、胶片颗粒"这些词该怎么说。
- 核心用法（3 步）：1) 打开 prompt.newzone.top 或装桌面版；2) 选主题 → 选分类 → 点中文标签（5000+ 标签，几乎每条都有预览图，看图选词）；3) 右侧自动拼好英文 prompt，复制到 Midjourney / FLUX / Veo / Seedance / Kling。
- 什么时候用 / 常见坑：英文不行、词汇卡壳时用；翻译走免费公共接口，超长段落可能翻不出来；悬停预览图需要联网。

**适用场景**：中文创作者、给客户做提示词代写的人。

**怎么用它搞钱**：提示词代写 / 教学。

**来源**：[rockbenben/img-prompt](https://github.com/rockbenben/img-prompt) · ⭐363 · 更新于 2026-10-07

### Awesome Seedance 2.5 Prompts + Skill

**核心提炼**
- 解决什么问题：Seedance 2.5 新模型 prompt 写法没人教，又想一条龙搞定"优化 → 分镜 → 生成 → 复查"。
- 核心用法（4 步）：1) `npx skills add AtlasCloudAI/awesome-seedance-2.5-prompts-skills --skill seedance-2-5-skill`；2) 把创意 / 参考图 / 旧 prompt 丢给 agent；3) skill 按 7 段结构（参考绑定 → 动作 → 空间 → 运镜 → 风格 → 音频 → 约束）生成可用 prompt，复杂项目会用 Seedream 5.0 先出分镜图；4) 接 Atlas Cloud 执行生成并自动复查。另有一个跨模型通用的 universal-video-prompt-skill，一份 brief 可编译到多个模型。
- 什么时候用 / 常见坑：做 Seedance 2.5 长叙事 / 多参考视频时用；"执行生成"走 Atlas Cloud 需要 API key，是花钱环节。

**适用场景**：Seedance 2.5 深度用户、接 AI 视频商单的工作室。

**怎么用它搞钱**：即梦商单。

**来源**：[AtlasCloudAI/awesome-seedance-2.5-prompts-skills](https://github.com/AtlasCloudAI/awesome-seedance-2.5-prompts-skills) · ⭐234 · 更新于 2026-10-12

## 收录标准

- 来源：X 博主实战分享（原帖 / 评论区 / 引用链）及 GitHub 高星项目
- 每条格式：核心提炼（解决什么问题 / 核心用法 / 什么时候用）+ 适用场景 + 一条「怎么用它搞钱」
- Star 数为 2026-10-12 经 GitHub API 核验；持续收录中
- 去重：同一项目只收录一次，不堆 raw 链接

## 相关分类

- 总索引：[x-viral-video-skills](https://github.com/kkone1238899/x-viral-video-skills) —— 13 个分类导航
- [x-viral-video-scripts](https://github.com/kkone1238899/x-viral-video-scripts) —— 编剧 / 脚本
- [x-viral-video-hooks](https://github.com/kkone1238899/x-viral-video-hooks) —— 标题 / 5 秒钩子
- [x-viral-video-creative-direction](https://github.com/kkone1238899/x-viral-video-creative-direction) —— 创意总监
- [x-viral-video-directing](https://github.com/kkone1238899/x-viral-video-directing) —— 导演
- [x-viral-video-replication](https://github.com/kkone1238899/x-viral-video-replication) —— 复制爆款
- [x-viral-video-breakdown](https://github.com/kkone1238899/x-viral-video-breakdown) —— 拉片
- [x-viral-video-pipeline](https://github.com/kkone1238899/x-viral-video-pipeline) —— 流水线 / 生产管线
- [x-viral-video-de-ai](https://github.com/kkone1238899/x-viral-video-de-ai) —— 去 AI 味
- [x-viral-video-characters](https://github.com/kkone1238899/x-viral-video-characters) —— 人物构建
- [x-viral-video-editing](https://github.com/kkone1238899/x-viral-video-editing) —— 视听剪辑技巧
- [x-viral-video-copywriting](https://github.com/kkone1238899/x-viral-video-copywriting) —— 文案
- [x-viral-video-showcase](https://github.com/kkone1238899/x-viral-video-showcase) —— X 病毒视频合集

## 投稿

发现好的提示词优化 prompt / skill，欢迎提 Issue 或 PR（格式见 CONTRIBUTING.md）。

## 更新日志

- 2026-10-12：条目升级为小节格式（核心提炼 / 适用场景 / 搞钱 / 来源），新增 Prompt Optimizer、PromptEnhancer 两个通用向项目，共 5 个项目
- 2026-10-11：首版，3 个项目，持续收录中
