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

### AI Video Generator — Claude Skill

**核心提炼**
- 解决什么问题：一句想法直接丢给 Seedance 2.0 / Higgsfield，出片要么太平要么翻车——缺一个把想法翻译成"生产级提示词"的引擎。
- 核心用法（4 步）：1) 把 SKILL.md 复制到 `~/.claude/skills`（10 个子 skill：病毒钩子 / 无脸频道 / SaaS 发布 / 课程预告 / 个人品牌 / 奢侈品美学 / 前后对比 / AI 数字人等）；2) 把一个想法告诉 Claude；3) skill 输出 15–25 行提示词：每秒时间戳、15+ 运镜术语、布光预设、声音设计（环境 + 冲击 + 音乐 + 人声分层）、平台适配（TikTok / Reels / Shorts 纵横比与安全区）；4) 粘贴到 Higgsfield 生成。注意物理学：前 2 秒决定 50% 的观众去留。
- 什么时候用 / 常见坑：Seedance 2.0 是精密引擎，"电影感"这类模糊词无效，要精确的运镜 / 布光 / 时码语言；作者用这套 skill 给 30 万粉的 Instagram 账号做全套视频，是实战验证过的生产管线。

**适用场景**：Seedance / Higgsfield 用户、做 SaaS / 课程 / 品牌商单的创作者。

**怎么用它搞钱**：短视频商单 / 教学（钩子工程 + 平台适配是差异化卖点）。

**来源**：[rediumvex/ai-video-generator-claude](https://github.com/rediumvex/ai-video-generator-claude) · ⭐421 · 更新于 2026-10-17

### 真实视频提示词 skill

**核心提炼**
- 解决什么问题：AI 视频一看就假——太干净、太完美，没有真实素材的糙感；堆形容词没用，要反向设计"谁拍的、用什么拍的、哪年拍的"。
- 核心用法（3 步）：1) 按 Agent Skill 标准安装（Hermes / Claude / Codex / Cursor）；2) 输入一句话想法；3) skill 先给这段素材设定来源（年代 + 设备 + 拍摄者），再生成结构化提示词：设备缺陷、自然失误、环境声音、时间轴全部写进去。跑 Seedance / Sora / Kling / Runway / Veo。
- 什么时候用 / 常见坑：做"真实感"类内容（vlog、纪实、UGC 风）之前用；要的是"手机随手拍"的糙感，不是电影大片。

**适用场景**：做真实感 / UGC 风 AI 视频的创作者、想给视频去 AI 味的人。

**怎么用它搞钱**：真实感短视频商单 / 教学。

**来源**：[zhouwei713/seedance-prompt](https://github.com/zhouwei713/seedance-prompt) · ⭐328 · 更新于 2026-10-16

### Cinematic Video Prompt Skill

**核心提炼**
- 解决什么问题：英文提示词写不出专业味——"cinematic" 一词包打天下，模型看不懂你想要的机位和光。
- 核心用法（4 步）：1) `git clone` 到 `~/.claude/skills/cinematic-video-prompt`；2) 按提示词公式拼：[景别 + 角度], [主体 + 外貌], [具体动作], [场景 + 天气], [布光], [运镜], [风格 + 色彩], [情绪], [技术参数]；3) 写卡壳时查词库：70+ 机位 / 60+ 运镜 / 80+ 布光 / 100+ 风格，配"什么时候用"说明；4) 跨模型通用：Veo 3 / Kling / Sora / Runway / Hailuo / Luma / Midjourney 都吃这套词。内置红线：一条 clip 只一个运镜、一个主动作，布光必须匹配天气 / 时间。
- 什么时候用 / 常见坑：写英文提示词卡壳时当词典查；附赠 bonus skill：角色一致性参考图、东方仙侠场景包。

**适用场景**：写英文提示词的创作者、技术向 prompt 玩家。

**怎么用它搞钱**：提示词代写 / 教学（词库 + 公式是硬通货）。

**来源**：[Rylaispirit/cinematic-video-prompt-skill](https://github.com/Rylaispirit/cinematic-video-prompt-skill) · ⭐151 · 更新于 2026-10-17

### Vibe Creating

**核心提炼**
- 解决什么问题：堆参数写分镜式提示词，模型越强越没必要——真正值钱的是"讲好故事"，让模型自己找镜头和节奏。
- 核心用法（4 步）：1) 按 Agent Skill 标准装（Claude Code / Codex / OpenClaw / Hermes），或当中英双语规则用；2) 输入粗糙想法 / 情绪 / 过度指定的分镜；3) skill 先判断：场景 × 表达 × 信息三轴打分，不合适就原样保留、信息不够先问 1–3 个短问题；4) 输出固定四段式：判断 → 动作（直通 / 轻清理 / 重写 / 追问）→ 结果 → 备注。可跑 Seedance 2.0 / Kling / Veo / Hailuo / Wan / Vidu 等（可走 Atlas Cloud 统一 API）。
- 什么时候用 / 常见坑：想法是情绪 / 故事而不是分镜时用；精确分镜需求它会主动让路、不扁平化——这就是它跟"缩短器"的本质区别。方法论源自 ByteDance 的 Vibe Creating。

**适用场景**：想用"故事感"驱动出片的创作者、跨模型用户。

**怎么用它搞钱**：创意型商单 / 教学（ByteDance 方法论是差异化卖点）。

**来源**：[Alisa0808/vibe-creating-skill](https://github.com/Alisa0808/vibe-creating-skill) · ⭐150 · 更新于 2026-10-15

### Cinematic Video Prompt Engineer

**核心提炼**
- 解决什么问题：剧情 / 小说片段 / 一句话场景，直接翻成提示词就是流水账——缺一个"剧情诊断 → 电影语言翻译"的工程师。
- 核心用法（5 步）：1) 装 skill；2) 输入剧情，skill 先诊断（情绪核心 / 视觉核心 / 冲突关系 / 可拍摄节点 / 结构与片长）；3) 把内心活动、抽象情绪外化成动作、表演、道具、声音、光影；4) 双路径：无参考图直出，或先出角色 / 场景 / 关系 / 道具参考图再编译视频提示词；5) 生成失败只修失败字段（单变量修复）。支持 46 种运镜模块、25 种情绪表演模块、6–30 秒自适应、16:9 / 9:16 重新构图（不是简单裁切）。
- 什么时候用 / 常见坑：短剧 / 剧情类 AI 视频开工前用；多轮迭代时用"结果局部修复"，别全盘重来。

**适用场景**：做 AI 短剧 / 剧情短视频的人、接商单的工作室。

**怎么用它搞钱**：短剧商单 / 剧本转提示词代做服务。

**来源**：[CyberJ0605/cinematic-video-prompt-engineer-skill](https://github.com/CyberJ0605/cinematic-video-prompt-engineer-skill) · ⭐130 · 更新于 2026-10-15

### Kling AI Prompt Generator

**核心提炼**
- 解决什么问题：Kling 3.0 一堆新功能（多镜头分镜 / Avatar 2.0 / 动作控制），官方 release note 没人替你翻译成提示词写法——盲试烧积分。
- 核心用法（4 步）：1) 装 Claude skill，或直接用网页版生成器（免安装）；2) Claude 先问澄清问题再组提示词；3) 按 Kling 官方规范写：4 镜分镜、角色一致性引用、运镜词汇、"回到起始位置"防卡 99%、说话人归属做对口型；4) 附 API 费率卡（按秒计费），接单前先算好成本。支持 Kling 3.0 全系 + Avatar 2.0（一张照片 + 音频出 5 分钟说话人）。
- 什么时候用 / 常见坑：Kling 商单开工前先过一遍 skill；每条事实都引自 kling.ai/release-note，可查证。

**适用场景**：Kling 深度用户、做口播 / 数字人 / 产品广告的人。

**怎么用它搞钱**：Kling 商单 / 数字人代做（Avatar 2.0 是稀缺能力）。

**来源**：[maciejdzierzek/kling-ai-prompt-generator](https://github.com/maciejdzierzek/kling-ai-prompt-generator) · ⭐31 · 更新于 2026-10-15

### @yoney1223 电影感短片三场景提示词模板

**核心提炼**
- 解决什么问题：想要电影感 AI 短片，但提示词写不出"大片调度感"——缺一个可直接套用的结构模板。
- 干货要点：1) 四段流程：故事板 → Prompt 优化 → AI 生成 → 调整成片；2) 模板框架："根据参考图像创作电影般的超现实视频，同一男主角在三个神奇动作场景中"；3) 场景一：男主从办公楼顶部跳下，楼层向观众塌落，相机从后方紧跟、穿过坠落碎片；4) 场景二：慢动作中男主在喷泉水流里向上跃起，相机从左向右平移，水珠凝固、重力反向；5) 场景三：咖啡馆微缩世界，男主跃过被放大数倍的咖啡杯和糕点，镜头俯视推进、咖啡表面形成涟漪；6) 结尾统一要求：平滑运镜、逼真真人动作、角色外观一致、精细纹理、温暖金色时段照明、自然阴影、电影般景深、无缝过渡；7) 技术参数：4K、照片级真实、竖屏 9:16、无文字 / 标志 / 水印。
- 什么时候用 / 常见坑：Grok / Google Flow / Seedance 2.5 均可套用；三场景共用同一男主角是保持角色一致性的关键。

**适用场景**：想做电影感 AI 短片的创作者。

**怎么用它搞钱**：电影感短视频商单 / 教学（模板可直接改写成服务）。

**来源**：[@yoney1223](https://x.com/yoney1223/status/2109616486360949105) · 2026-10-12

### @john87445528 街头换装病毒视频反推提示词模板

**核心提炼**
- 解决什么问题：爆款视频想复刻，但写不出"能稳定跑通"的提示词——缺一个真实素材参数 + 秒级分镜的工业化模板。
- 干货要点：1) 开头先写真实素材参数段：总时长 16.2 秒、竖屏 9:16、30fps、未经处理的 iPhone 后置原生相机手持素材、无滤镜无美颜、呼吸抖动、自动对焦延迟、曝光波动，保留锐化 / 眩光 / 压缩噪点；2) 人物锁定段：女主全程一致，参考图仅锁服装不采用脸；3) 描述精确到材质、扣带位置、道具左右手分配，配禁令式写法"禁止换手、复制、消失或变形"；4) 秒级分镜（0.00—0.80 … 14.15—16.20），含 5.03 秒硬切转场规则。
- 什么时候用 / 常见坑：复刻病毒视频前先做反推，写出"参数段 + 锁定段 + 分镜"三段式模板；禁令式写法是防 AI 乱改的关键。

**适用场景**：做病毒视频复刻 / 换装类内容的人。

**怎么用它搞钱**：爆款复刻代做 / 教学。

**来源**：[@john87445528](https://x.com/john87445528/status/2111439621955465268) · 2026-10-17

### @BDFrankHoubre 一分钟 AI 短片五步法

**核心提炼**
- 解决什么问题：新手"输入一条长 prompt 靠运气"出片——缺一套先规划、后生成的纪律。
- 干货要点：1) 核心结论：一分钟 AI 短片 = 一页剧本 → 拆成 10–15 个镜头 → 每个镜头先作为静帧规划 → 再转成视频；2) 先写完一页剧本（正规格式 + 场景标题），再打开任何生成器；3) 分镜拆解四要素：画面（远 / 中 / 近景）、角度（平视 / 仰 / 俯）、运镜（静止 / 推进 / 平摇）、时长（秒），写在对应剧本行旁；4) 每个分镜先生成静帧分镜图（静帧比视频便宜得多）；5) 用批准过的静帧生成视频素材；6) 按剧本顺序剪辑、按计划时长修剪、最后加声音；7) 五个常见错误：先生成后写作、场景太多致连续性崩、没有分镜清单、直接给未批准静帧做动画、声音留到最后。
- 什么时候用 / 常见坑：做 AI 剧情短片 / 短剧时套用；作者为 ScreenWeaver 联合创始人，文末有工具自我披露，方法论部分独立可用。

**适用场景**：做 AI 剧情短片 / 短剧的人。

**怎么用它搞钱**：短剧商单 / 分镜前置服务（静帧分镜代做）。

**来源**：[@BDFrankHoubre](https://x.com/BDFrankHoubre/status/2110302333485686969) · 2026-10-14

### @dhivagar Higgsfield 提示词速查表

**核心提炼**
- 解决什么问题：AI 短剧出片靠抽卡运气——角色漂移、镜头断裂、否定词失灵、盲抽高清版烧积分，缺一套可复用的提示词纪律。
- 干货要点：1) 角色表一次建好反复用：16:9 画布三面板（无头全身背面/无头全身正面/表情特写），一张表只放一张脸（多张脸会漂移），存为固定元素、每条 prompt 用同一个 @tag 锁定身高体型；2) 先低成本抽卡再升档：480p draft 先抽 4 条挑 keeper，再上 1080p/4k——高清版费用约翻倍，不值得盲跑；3) 正说不要说"不要"：Seedance 会把 "not crying" 读成 crying——写"他站稳、双脚扎地"而不是"不要摔倒"，情绪写成具体肌肉动作（"两下点头、一个耸肩"而不是"他很开心"）；4) 每条 prompt 顶部贴固定风格块：全局问题只修风格块前缀，单镜头问题只改单条；5) 15 秒一个镜头包：台词加引号并附语气注（如轻蔑的不信而不是大喊），镜头按 1a/1b/2a 命名；6) 置换时先列保持项再点名唯一变化项：脸部特写单独传图；1080p 脸/口型易漂移、4k 更稳，夜景漂移更严重；7) 换脸分两遍：第一遍定场景姿态表情颗粒，第二遍再做换脸，每遍只干一件事；8) 常驻场景当角色一样锁定：固定机位、色卡、时间段，清理画面文字杂物（会变异），人物乱瞬移就给俯视布局图；9) 做连续性直接喂上一镜的实际视频：文字梗概会丢信息；对白戏从全景开场再切入；10) 每轮跑 4 条：1 条失败重抽，4 条同方式失败就重写 prompt，先说出失败类型（资产/动作/机位/坏种子），一次只改一个变量。
- 什么时候用 / 常见坑：做 AI 短剧/连贯叙事短片时全程套用；作者学完 175 节免费官方课程后沉淀，偏 Seedance/Higgsfield 工作流；夜景+换脸是高危组合，多留预算。

**适用场景**：做 AI 短剧/连贯剧情短视频的人、用 Seedance/Higgsfield 接商单的创作者。

**怎么用它搞钱**：AI 短剧商单/教学（角色一致性是行业痛点，抽卡成本纪律直接省钱）。

**来源**：[@dhivagar](https://x.com/dhivagar/status/2111520367038865409) · 2026-10-17

### @neo_cn 人物微动提示词技巧

**核心提炼**
- 解决什么问题：AI 视频里的人物站着不动像蜡像，再真的脸也假——缺一套"让人物活起来"的微动写法。
- 干货要点：1) 反直觉结论：动得越小越像真的，静止 = 假；2) 微动四要素：呼吸起伏、重心左右换、偶尔眨眼、头发轻晃；3) 可复用英文短语：subtle breathing、slight weight shift、occasional blink，直接塞进提示词；4) 幅度原则：微动不是大动作，越克制越真实。
- 什么时候用 / 常见坑：人物特写 / 口播 / 数字人类镜头必加微动；幅度写过大会变抽搐。

**适用场景**：做真人感 AI 视频、数字人、口播的人。

**怎么用它搞钱**：真人感短视频商单 / 教学（去 AI 味的低成本解法）。

**来源**：[@neo_cn](https://x.com/neo_cn/status/2111623294583730193) · 2026-10-17

### @lgwny0120 Meta Muse 音画同步提示词模板

**核心提炼**
- 解决什么问题：画面、口型、中文对白、背景音乐要多次生成再合成——想一条提示词一次直出 10 秒短片。
- 干货要点：1) 评论区 (1/3)(2/3)(3/3) 给出完整可复制模板；2) 模板结构：总览（10 秒 / 9:16 / 人物妆造）→ 服装 + 场景 → 分镜动作 + 对白 + 口型匹配 → 要求项（表演 / 构图 / 音频）→ 禁止项；3) 实测口型准、眼神不呆。
- 什么时候用 / 常见坑：Meta Muse（Muse）音画同步场景；模板结构可迁移到其他支持音频生成的模型。

**适用场景**：做口播 / 对白类 AI 短视频的人。

**怎么用它搞钱**：对白短视频商单 / 模板教学。

**来源**：[@lgwny0120](https://x.com/lgwny0120/status/2111633049113038973) · 2026-10-17

### @hqinjarsy AI 影视化文戏分析

**核心提炼**
- 解决什么问题："她内心复杂、表演细腻"式提示词等于没写——文戏（对白戏）是 AI 影视化最难啃的骨头。
- 干货要点：1) MTAVG-Bench 多人对白评测：互动与镜头配合是差距所在；2) 库里肖夫效应：剪辑赋予表演意义，提示词要写"反应"而不是"情绪形容词"；3) 核心结论："表演就是反应"，文戏是反应戏不是台词戏；4) 情绪形容词必须翻译成动作和反应再写进提示词；5) 靠谱路线：真人先演再搬运；6) 检验法：拿掉配乐关系还在不在、换脸整场戏变没变。
- 什么时候用 / 常见坑：写剧情 / 对白类提示词时对照自查；凡是情绪形容词，一律先转成可拍的动作。

**适用场景**：做 AI 短剧 / 剧情短视频的人。

**怎么用它搞钱**：AI 短剧商单 / 表演指导式提示词教学。

**来源**：[@hqinjarsy](https://x.com/hqinjarsy/status/2111570887472476161) · 2026-10-17

### @hx831126 风格术语纠偏与 Opus 5.5 写法公式

**核心提炼**
- 解决什么问题：想要的风格叫错了名（想说 cut-out animation 却写 B-Roll），模型理解跑偏；对强模型套 Skill 壳是多余的。
- 干货要点：1) 术语纠偏：B-Roll 在行业里指细节镜头 + 卡点剪辑，不是一种风格；想要的风格叫 cut-out animation；2) 对 Opus 5.5 这类理解力强的模型，不需要 Skill 套壳；3) 写法公式：主角是谁 + 东西怎么进画面 + 什么节奏 + 什么质感。
- 什么时候用 / 常见坑：选风格词前先确认行业定义；模型越强，提示词越应该说人话。

**适用场景**：写英文提示词、做风格化短视频的人。

**怎么用它搞钱**：风格化短视频商单 / 提示词教学。

**来源**：[@hx831126](https://x.com/hx831126/status/2111632702445437130) · 2026-10-17

### @Cia0_exe Seedance 2.5 第一人称 POV 喜剧模板

**核心提炼**
- 解决什么问题：第一人称 POV 短片想一次跑通——人物一致性、第一人称运镜规则、声音设计缺一个超完整模板。
- 干货要点：1) 总览：30 秒 / 16:9 / 第一人称视角 / 喜剧钩子；2) 质感段：椭圆焦外光斑、水平拉丝蓝光晕、胶片颗粒、暖金逆光 + 青绿阴影、彩虹棱镜衍射；3) @Image1 人物一致性锁定（脸型 / 五官 / 发型 / 服装全程一致）；4) @Image2 场景材质光线参考（不锁定构图）；5) 第一人称规则：眼高随姿态变化、视线惯性延迟、呼吸浮动、撞击失焦；6) 群演焦外虚化不抢戏；7) 精确到 0.5 秒的分镜时间轴（前 3 秒强钩子 → 18.5–21.5s 高潮 → 最后 8.5s 表情表演）；8) 声音设计：钢琴 / 弦乐 / 竖琴，踩断魔杖音乐骤停 0.3 秒；9) 负面约束：无字幕水印、手指面部不变形不穿模。
- 什么时候用 / 常见坑：Seedance 2.5 第一人称 / POV 题材直接套；@ 引用锁定人物和场景是关键。

**适用场景**：做 POV / 第一人称 AI 短视频的人。

**怎么用它搞钱**：POV 短视频商单 / 模板教学。

**来源**：[@Cia0_exe](https://x.com/Cia0_exe/status/2111641020857516186) · 2026-10-17

### @AI__TSUBAKI Seedance 2.5 舞蹈视频结构化模板

**核心提炼**
- 解决什么问题：舞蹈视频人物漂移、动作重复、运镜太"AI 味"——缺一个结构化模板。
- 干货要点：1) 总览：15 秒竖屏 9:16 真人舞蹈；2) 场景：高中教室；3) 镜头规则：一镜到底、无变焦无剪切；4) 人物一致性优先级：@Image1 的脸 / 发型 / 服装 / 配色 / 整体轮廓；5) 单人约束；6) 动作多样性：不重复编舞（步伐 / 转身 / 手部 / 脚步 / 侧脸 / 摆发）；7) 业余手持运镜感：iPhone 手持抖动、略偏构图、松散跟拍——用"糙感"去 AI 味。
- 什么时候用 / 常见坑：Seedance 2.5 / Dreamina 舞蹈类视频；手持糙感是去 AI 味的关键。

**适用场景**：做舞蹈 / 真人感 AI 短视频的人。

**怎么用它搞钱**：舞蹈短视频商单 / 去 AI 味教学。

**来源**：[@AI__TSUBAKI](https://x.com/AI__TSUBAKI/status/2111629613894148593) · 2026-10-17

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

- 2026-10-17：晚档新增 6 条（@neo_cn 人物微动四要素、@lgwny0120 Meta Muse 音画同步模板、@hqinjarsy 文戏"表演就是反应"分析、@hx831126 风格术语纠偏+Opus 5.5 写法公式、@Cia0_exe Seedance 2.5 POV 喜剧完整模板、@AI__TSUBAKI Seedance 2.5 舞蹈结构化模板；18 轮关键词 Latest 搜索 + 6 干货账号时间线抽查，窗外/广告/无干货帖按宁缺毋滥剔除，未凑数），共 21 个条目
- 2026-10-17：午档新增 1 条（@dhivagar Higgsfield 提示词速查表：10 条角色一致性/抽卡成本/分镜连续性规则，按价值铁律提炼；10 组关键词 Latest 搜索 + 6 干货账号抽查，窗口内其余帖按宁缺毋滥剔除，未凑数），共 15 个条目
- 2026-10-17：早档新增 9 条（GitHub 6 个 skill：rediumvex/ai-video-generator-claude 421★、zhouwei713/seedance-prompt 328★、Rylaispirit/cinematic-video-prompt-skill 151★、Alisa0808/vibe-creating-skill 150★、CyberJ0605/cinematic-video-prompt-engineer-skill 130★、maciejdzierzek/kling-ai-prompt-generator 31★，star 与更新时间均为当日 API 实测；X 3 条：@yoney1223 电影感短片三场景模板、@john87445528 街头换装反推提示词模板、@BDFrankHoubre 一分钟 AI 短片五步法，均按价值铁律提炼），共 14 个条目
- 2026-10-12：条目升级为小节格式（核心提炼 / 适用场景 / 搞钱 / 来源），新增 Prompt Optimizer、PromptEnhancer 两个通用向项目，共 5 个项目
- 2026-10-11：首版，3 个项目，持续收录中
