---
layout: default
title: "Can an AI Therapist Actually Help? (Slingshot AI CEO)"
channel: "The MAD Podcast with Matt Turck"
date: 2025-11-13
---

# Can an AI Therapist Actually Help? (Slingshot AI CEO)

**频道**: The MAD Podcast with Matt Turck
**发布日期**: 2025-11-13
**视频链接**: https://www.youtube.com/watch?v=3SliW74opyY

---

## Key Takeaways

## 一句话总结
Slingshot AI CEO 分享了他们如何通过分阶段、数据驱动且高度整合的方法，构建一个能真正帮助用户改善心理健康的AI治疗师Ash，并展示了其在心理健康领域的巨大潜力和实际效果。

## 内容概览
本视频由Slingshot AI的CEO Daniel主讲，他深入介绍了构建AI心理治疗师Ash的技术细节和理念。视频首先指出当前全球面临的心理健康危机和专业治疗师短缺的严峻现实，并批评了现有AI在心理治疗领域的不足。随后，Daniel详细阐述了Slingshot AI如何通过“预训练 (pre-training)”、“对齐 (alignment)”和“强化学习 (reinforcement learning)”三个阶段来打造其AI治疗师，强调了数据质量、多模态疗法融合、临床团队指导以及从用户反馈中持续学习的重要性。最后，他分享了Ash在帮助用户建立社交联系等方面的实际成效，并鼓励观众体验和加入他们的团队。

## 核心要点

### 1. 巨大的心理健康服务缺口与AI的潜在解决方案
**背景/问题**: 全球范围内存在严重的心理健康危机，同时专业心理治疗师严重短缺（美国平均每1500人对应一名治疗师），这一问题已持续数十年且未得到改善。
**核心观点**: 现有的AI（如ChatGPT）在心理治疗领域表现不佳，但AI技术有潜力成为解决这一服务缺口的关键。Slingshot AI的目标是构建一个真正能帮助用户的AI治疗师。
**实践启示**: 识别并解决社会痛点（如心理健康服务不均）是AI应用的重要驱动力。AI不应仅仅是模仿人类，而应是创造新的、更有效的解决方案。

### 2. 构建AI治疗师的“三阶段模型”：预训练、对齐与强化学习
**背景/问题**: 训练一个有效的AI治疗师需要超越通用语言模型的局限，使其具备专业性、安全性和有效性。
**核心观点**: Slingshot AI采用了一个与通用语言模型训练相似但更精细的“三阶段模型”：
    *   **预训练 (Pre-training)**：通过海量、高质量、合乎道德且经过同意的数据进行训练，涵盖多种疗法（CBT, DBT, ACT, IFS, Psychodynamic therapy, Motivational interviewing, Somatic therapy等）和不同风格（情绪导向、认知导向、开放式、指导式、精神性、世俗性）。
    *   **对齐 (Alignment)**：由临床团队指导，将模型行为从模仿人类转变为适合AI的交互方式，引入政策和“guardrails”（安全护栏），确保AI的言行得体且安全。
    *   **强化学习 (Reinforcement Learning)**：利用用户反馈（如响应时间、情绪变化、用户分享的体验）进行持续在线学习，不断优化模型表现。
**实践启示**: 专业的、多模态的、数据驱动的训练方法是开发高质量AI应用的关键。AI的“对齐”阶段至关重要，以确保其在特定领域的安全和有效性。

### 3. 数据质量与多样性是AI心理治疗的基石
**背景/问题**: 通用语言模型在互联网上公开的数据不足以支撑专业的心理健康应用，且数据收集需要严格的道德和隐私保障。
**核心观点**: Slingshot AI通过与行为健康组织合作， ethically and with consent（合乎道德且获得同意）地获取高质量的、非公开的预训练数据。这些数据包括了人类治疗过程中丰富的细节和“magic”（魔力）。
**实践启示**: 优质、合规的数据是AI模型成功的先决条件，尤其是在敏感领域。AI的潜力在于能从人类经验中学习，而不仅仅是公开信息。

### 4. AI治疗师的独特优势：非评判性与快速开放
**背景/问题**: 人类在寻求心理帮助时，常常因为害怕评判或社会压力而有所保留。
**核心观点**: 用户与AI（如Ash）的互动显示，他们会更快地敞开心扉，因为AI被预期为“lack of judgment”（缺乏评判）。这种非评判性的环境鼓励用户更早地分享深层个人信息。
**实践启示**: AI在某些场景下可以提供比人类更安全、更易于亲近的倾诉空间，从而加速治疗过程的启动。

### 5. 强调“AI行为”的识别与纠正（Alignment）
**背景/问题**: AI在模型训练初期可能会出现不符合AI身份的“weird things”（奇怪行为），例如以第一人称讲述个人经历。
**核心观点**: Slingshot AI开发了“behaviors”监控系统，利用小模型快速识别和标注AI的不当行为。通过DPO（Direct Preference Optimization）等技术，临床团队可以对模型进行偏好标注，选择更优的回复，并追踪和创建评估（evals）来纠正这些不当行为。
**实践启示**: 对AI的“行为”进行精细化管理和标注，是确保AI在特定应用场景中表现得体和安全的重要环节。

### 6. 强化学习在非结构化、长时对话中的应用
**背景/问题**: 心理治疗对话通常是长期的、没有明确终点的，与象棋等有明确结束的游戏不同，传统的价值模型（value models）难以直接应用。
**核心观点**: Slingshot AI利用对话中的“huge amount of signal”（海量信号），如用户开放/封闭程度、连接感等，来训练其价值模型。这种方法可以评估每一次互动的好坏，并指导AI进行持续优化。
**实践启示**: 针对特定场景（如长期对话）设计定制化的强化学习策略，能有效提升AI在复杂任务中的表现。

### 7. 衡量AI治疗效果的四重目标：意图、联盟、心理改变与行为改变
**背景/问题**: 如何科学地评估AI治疗师的实际成效，而不仅仅是对话的流畅度。
**核心观点**: Slingshot AI设定了四个递进且相互关联的目标：
    *   **Build intent with the user**: 用户有明确的意图寻求心理帮助。
    *   **Build a therapeutic alliance/working alliance**: 用户与AI建立起互信、协作的治疗关系。
    *   **Achieve psychological change**: 用户在心理层面发生积极变化。
    *   **Behavioral change**: 用户在实际行为上发生积极改变。
**实践启示**: 设定明确、可衡量的目标是评估AI在复杂应用领域（如心理健康）有效性的关键。

### 8. Ash在促进社交联系方面的显著成效
**背景/问题**: 与通用AI可能导致用户更孤立相反，AI治疗师应能促进积极的社会连接。
**核心观点**: Slingshot AI与NYU合作进行的一项研究表明，使用Ash（平均10周）的用户平均增加了1个朋友或亲近的个人联系。这与ChatGPT等通用AI可能加剧孤独感形成鲜明对比。
**实践启示**: 经过精心设计和训练的AI，不仅能解决个体心理问题，还能积极地促进社会连接，这是AI在心理健康领域超越通用AI的关键价值。

### 9. 关注AI的“价值模型”评估与优化
**背景/问题**: 需要一种机制来评估AI生成回复的质量，并将其与期望的治疗目标相匹配。
**核心观点**: Slingshot AI开发了“value model”（价值模型），能够追踪对话中的多种信号，评估不同回复的潜在效果（如用户是否会忽略、困惑，或建立连接）。这有助于选择最优回复，并进行持续优化。
**实践启示**: 建立能够量化和优化AI输出质量的评估体系，是提升AI在关键领域（如治疗）有效性的重要手段。

## 关键概念与资源
**核心概念**:
*   Foundation Model for Psychology
*   Mental Health Crisis
*   Pre-training, Alignment, Reinforcement Learning (RL)
*   Therapeutic Alliance / Working Alliance
*   Psychological Change
*   Behavioral Change
*   Direct Preference Optimization (DPO)
*   Value Model
*   Guardrails
*   Turing Test

**工具/技术**:
*   Slingshot AI's Ash (AI Therapist Product)
*   Large Language Models (LLMs)
*   Small Models (for data analysis and annotation)
*   Behavioral Health Organization Partnerships
*   NYU Collaboration (for research study)

**推荐资源**:
*   JFK's 1963 speech on mental health provider shortage (mentioned as historical context)
*   Various therapeutic modalities (CBT, DBT, ACT, IFS, Psychodynamic therapy, Motivational interviewing, Somatic therapy)

## 目标受众
**最适合**:
*   AI开发者、机器学习工程师、产品经理，特别是对AI在医疗健康、心理健康领域的应用感兴趣的人。
*   心理健康专业人士（治疗师、研究员），希望了解AI如何辅助或改变心理治疗模式。
*   对AI技术如何解决社会性问题（如心理健康服务缺口）有好奇心和求知欲的普通观众。
*   正在寻找下一代AI解决方案的创业者和投资者。

**价值场景**:
*   了解AI在心理健康领域的技术挑战与创新路径。
*   学习如何构建一个负责任、有效且数据驱动的AI应用。
*   洞察AI如何通过解决实际社会问题来创造价值。
*   为AI在人机交互、情感计算等领域的研究提供新视角。

## 延伸思考
1.  **AI治疗师与人类治疗师的界限与协同**: 随着AI治疗师能力的提升，未来AI是否会完全取代人类治疗师？或者更可能的是，AI将如何与人类治疗师协同工作，形成一种混合模式，以最大化服务效率和效果？
2.  **伦理与监管的挑战**: 在AI深度介入心理健康领域时，数据隐私、安全、算法偏见、责任归属等伦理和监管问题将面临哪些新的挑战？Slingshot AI的“guardrails”和对齐方法是否足以应对所有潜在风险？
3.  **“AI治疗”的长期影响**: 除了促进社交联系，AI治疗师在帮助用户建立更深层次的自我认知、应对复杂情感和生活事件方面的长期影响是什么？我们如何衡量和确保这种长期影响是积极而非负面的？

---

## 中文文稿

好的，这是根据您提供的英文视频字幕转录并整理的高质量中文文稿：

**视频标题: AI 治疗师真的能帮到人吗？(Slingshot AI 首席执行官)**

---

**引言与背景**

大家好，很高兴今天能在这里。今天我将和大家聊聊如何构建一个心理学领域的 foundational model（基础模型）。

简单介绍一下我自己，我叫 Daniel，是一名机器学习工程师，也是 Slingshot 公司的联合创始人兼首席执行官。

**心理健康危机与供给短缺**

大家可能都知道，我们正面临一场心理健康危机。但可能不知道的是，心理健康服务提供者也存在巨大的短缺。在美国，平均每 1500 人才有一名治疗师，而且在很多地区，情况还要糟糕得多。

这个问题已经存在了大约 60 年。早在 1963 年，肯尼迪总统就曾就心理健康服务提供者严重短缺的问题发表过演讲，但情况并未好转。

**AI 在心理健康领域的现状与挑战**

如今，全世界似乎都迅速认同了一个观点：AI 的首要应用场景就是心理治疗。但目前，这主要指的是通过 ChatGPT 等工具进行的治疗，而它们的表现并不理想。

因此，我们 Slingshot 采取了一种截然不同的方法，致力于真正帮助人们改善心理健康。

**Slingshot 的方法论：构建 AI 治疗师 Ash**

通常在这个环节，我会演示我们的产品。今天，我将不直接展示 Ash 的外观，因为大家都可以自行体验。取而代之的是，我将深入介绍我们是如何构建 Ash 的，让大家一窥其“幕后”。

我们主要通过三个阶段来训练我们的模型，这与训练任何语言模型的过程非常相似：预训练（pre-training）、对齐（alignment）和强化学习（reinforcement learning）。

我们实现了完全的垂直整合，对训练这类模型所需的每一个细节都精益求精。这意味着我们关注体验的每一个环节：AI 在心理健康语境下应该谈论什么？在语音模式下，AI 应该停顿多久？让对方思考的时间多长才合适？什么时候应该打断对方？

**数据驱动的学习：超越单一理论**

但归根结底，这一切都依赖于从数据中学习。上一代心理健康领域的公司，通常会有一个固定的理念、方法或理论，认为只要每个人都能像他们一样理解和思考，心理健康问题就能解决。这通常是认知行为疗法（CBT）。他们可能会说，“让我们把这位大师的书籍内容，植入到人们的脑海里。”

而我们采取了截然不同的方法。我们从各种疗法中学习，包括：认知行为疗法（CBT）、辩证行为疗法（DBT）、接纳与承诺疗法（ACT）、内感官家庭系统疗法（IFS）、精神动力学疗法、动机性访谈以及躯体疗法等。

我们学习那些更适合情感导向体验、认知导向体验、开放式对话、指令式对话、精神层面或世俗层面的实践和人群。然后，我们将所有这些融合成一个模型。

**临床团队的对齐与调整**

接下来，我们会引入我们的临床团队。我们拥有一支全职的临床团队，负责对模型进行对齐（alignment）。这是为了将人类治疗师的做法，转化为适合 AI 的行为。

**用户互动的新模式：AI 的独特优势**

刚开始时，我们认为人们与 AI 的互动会更像与人类的互动。我们曾梦想着实现 AI 的图灵测试，想着只要学习足够多的数据，就能像 Zoom 上的远程治疗一样，实现 AI 治疗。

但我们发现，人们与 AI 的互动方式截然不同。首先，他们会更快地敞开心扉。我们经常遇到这样的对话：

AI (Ash): “嘿，准备开始了吗？”
用户: “是的，我是一个同性恋者，我从未告诉过任何人，我该怎么办？”

这种情况非常罕见。人们对 AI 抱有一种“不被评判”的期望。他们认为可以……

**对齐阶段：建立规则与保障**

因此，在对齐（alignment）阶段，我们必须进行调整，引入政策和防护栏（guardrails）。今天，我将为大家展示其中的一部分。

**强化学习：持续优化与反馈**

最后，我们进行强化学习（reinforcement learning）。大多数心理健康服务提供者没有机会了解自己的方法是否有效。他们总是好奇，自己说的那些“神奇的话”是否产生了影响，或者将来会产生什么影响。

而我们拥有海量的信号，可以从每一次对话中学习。这些信号包括：对方回应的时间长短、是否开始哭泣、是否说过“我从未对任何人说过这些”、“这是我第一次说出口”等话语。

还包括用户反馈：“嘿，我上周你说的那个方法试了，效果非常好”或者“我上周你说的那个方法试了，结果非常糟糕，你太差劲了。”

我们从这一切中学习，并通过持续的在线强化学习（continual online RL）不断优化。

**深入了解 Ash 的构建过程**

现在，我将为大家揭示更多关于 Ash 的构建细节，而不是花费所有时间在幻灯片上。

**预训练阶段：高质量数据的关键作用**

首先，我提到了我们使用预训练数据（pre-training data）。我认为，预训练数据最重要的一点就是拥有真正高质量的数据。我们使用海量数据进行训练，但并非所有数据都是对话形式的。

我们通过与行为健康组织的合作获取这些数据，当然，这些数据都是在获得用户明确同意后，合乎道德地获得的。

**数据预处理与 AI 能力的潜力**

我只是想简单展示一下。大家可以看到，我们进行了大量的预处理工作，来分析对话，理解哪些内容对 AI 来说是合适的，哪些不合适。这尤其需要借助小型模型来完成。

但更令人着迷的是，我们并没有真正意识到当今 AI 在心理健康领域的能力有多么不足，以及它未来可以多么出色。

好的，这是根据您提供的英文视频字幕转录、编辑和翻译后的高质量中文文稿：

**视频标题: AI 治疗师真的有用吗？（Slingshot AI 首席执行官访谈）**

### 案例展示：情绪波动与自我认知

您可以看到，我这里举了几个例子来让大家感受一下。这些是我随机从智能数据集里提取的、最开始的两个对话样本。所有数据都经过匿名化处理，我们做了大量的修改，确保无法将这些信息追溯到任何个人。

您可以看到这样的对话：“你当时是不是情绪失控了？你是不是气得暴跳如雷？然后等你冷静下来后，你是否感到内疚、懊悔等等？你是否情绪失控了？”

对方回答：“我感觉自己就像一堆垃圾。事后的恢复过程，是不是跟你发怒本身一样糟糕？”

“是的，我会这么说。您可以看到，如果能识别出在情绪爆发之前，是什么触发了你的‘电路短路’，你就能避免很多麻烦，对吧？”

“我们可以试着找出原因。在那段时间里，有没有什么事情让情况变得更糟？比如物质滥用或其他问题？或者你不喜欢现在的工作，诸如此类？”

### 对话的深度与价值

您会注意到，这显然是深入的对话，而不是用户第一次与AI交流。这些对话都是与真人进行的，而不是AI。

### 探索心理健康的奥秘

我们来进入另一个例子。我觉得观察这些对话非常有意思，这背后蕴含着心理健康的丰富内涵。您可以看到，我们希望对话是以“你”为中心，而不是围绕“我”。

“有些人是值得信任的，我可以信任一些人。”

您可以看到，治疗师在引导对方思考这些词语。

“或者，我可以选择信任谁。”

“哪种说法更真实？‘我可以信任一些人’，还是‘我可以选择信任谁’？”

“我可以选择信任谁。”

### 预训练的重要性

好的，我将继续进行演示，但我觉得有时理解这一点非常重要，它能说明为什么预训练（pre-training）如此关键。现实地说，我们喜欢谈论提示工程（prompt engineering），但有些用例的数据集在大型语言模型的预训练阶段根本不存在。

这是因为这些数据无法在互联网上公开获取，也无法安全、合乎道德地收集。我认为，一旦将这些数据融入模型，你就会意识到，通过预训练，通过学习一个庞大的语料库，能取得比试图遵循单一哲学理念更大的成就。

### 模型对齐：行为规范

好了，我将回到我们的工具。刚才谈的是预训练方面。在预训练之后，我们的模型有点意思，它有很多能力，但没有明确的方向。它不知道在特定情境下什么合适，什么不合适。

所以，我将分享我们用于对齐模型（aligning our model）的多种流程之一。我们有一个叫做“行为”（behaviors）的概念。我们的“行为”系统就像一个堆栈，帮助我们理解模型出现的奇怪之处、有趣之处。

这是我们通过匿名数据在线监控的能力。当您注册App时，会看到我们有一个选择项，允许我们使用您的数据来改进模型。大约70%的用户会选择同意。对于另外30%的用户，我们完全无法访问他们的数据，也无能为力。

对于选择同意的用户，我们存储的数据与用户身份是完全分开的，这些是我们能够分析的数据。

### 识别AI的“非人”行为

一件非常有趣的事情是，AI会告诉用户它做了AI不可能做的事情。我们通过数据来理解这一点的方式是，我们能快速构建数据集，哪怕只有几个合成的例子，就能训练一个非常小的模型。

您可以看到这些例子：“这是Ash（人名）说过的话。我当时在谈论我的朋友，然后我突然想起有一次我带着我的狗在公园里，我们看到……”我不知道当时的具体情境，但显然AI不可能说出这样的话。

因此，我们就能搜索并识别出一些案例。

“当然，我会告诉你我尝试学习滑雪的故事。这是几年前的事了。”

“您可以看到，这里不算太糟糕，您在讲故事，但仍然存在一些违反我们期望AI以第一人称说话的原则。”

### 模型比较与偏好优化

然后，如果我点击“标注”（annotate），希望一切都能正常运行。您可以看到，我们有几个不同的模型。我们有我们的Llama基础模型，我们的SLG（Slingshot AI自己的模型），以及一个我正在比较的Quen模型。我不知道Llama现在是什么情况。

您可以看到，“我宁愿听你讲一个你的故事。” “我能做到。”

“那么，假设我们更倾向于让我们的临床团队花费时间在这些类型的界面上，我们可以通过一个DPO（Direct Preference Optimization）例子来指示模型，我们更喜欢这个回复而不是那个。”

“让我将其保存为草稿。”

“我也可以附加上……比如，这是一种人类行为，假设这是不可接受的。”

我们会对这些进行标记，以理解哪里出了问题。然后，我们将其用于直接偏好优化（Direct Preference Optimization），也用于跟踪和创建评估（evals），以了解AI可能出现的不可接受行为，以及什么可以被认为是更好的。

### 强化学习与长对话的挑战

所以，这稍微介绍了一下模型对齐。关于对齐，我还有很多可以展示的，但我想谈谈强化学习（reinforcement learning）。

有趣的是，像我们这样的对话，它们是漫长的，对吧？它们可以持续数月。没有明确的终点。所以，如果你与下棋类游戏相比，下棋有明确的终点，而我们没有。

另一方面，你有……

好的，这是根据您提供的英文视频字幕转录并整理的高质量中文文稿：

**视频标题: AI 治疗师真的能提供帮助吗？ (Slingshot AI 首席执行官)**

### AI 的信号处理模型

在像国际象棋这样的游戏中，我们通常会采用机器学习中的价值模型（value models）。我不会深入探讨太多技术细节，但国际象棋的关键在于，你不需要走完整个棋局就能判断一个棋步的好坏。你可以直接观察棋盘，就能大致了解当前局面的优劣，比如有多少兵。

### AI 在心理健康领域的应用

在我们的语境下，对话中蕴含着海量的信号，比如对方的开放程度、封闭程度，以及他们感受到的连接感。我们会从所有这些信号中学习，并整合到一个模型中。

### AI 治疗师的四大目标

从根本上说，我们有四个目标，我们认为它们是按顺序排列且相互关联的。

首先，也是最重要的，我们希望与用户建立意向性（intent）。我们希望用户在心理健康语境下进行有目的的交流。即使他们无法解决生活中的所有问题，但他们愿意尝试，并且是出于正确的原因来到这里。

其次，我们希望建立治疗联盟（therapeutic alliance）或工作联盟（working alliance）。这是一种感觉，让你觉得你正在做正确的事情，并且以正确的方式进行，你们在协作设定目标，并且在相互尊重的基础上建立了关系。

从治疗联盟的基础上，我们希望实现心理上的改变（psychological change）。有很多指标可以表明心理改变正在发生，并且正在进行中。

最后，我们希望实现行为上的改变（behavioral change）。当一个人说：“我很孤独，我没有朋友。”我们希望他们能交到朋友。

### Ash 的研究成果与优势

我们 Ash（AI 治疗师的名字）迄今为止最令人兴奋的成果是，我们即将分享与纽约大学（NYU）合作进行的首个研究。我们已经证明了在所有这些目标轴上都实现了显著的改变。我认为行为改变是最令人欣喜的。

在我们的研究中，平均而言，使用 Ash 的用户在使用了大约 10 周后，平均多交了一个朋友或亲近的个人联系。

相比之下，当你想到 ChatGPT 和类似的 AI 时，它们在平均意义上会让用户变得更孤独，使用 AI 来处理这些问题越多，他们就越疏远，因为它取代了人际连接。

### Ash 的独特价值

但是，如果我们仅仅优化这些目标，我们已经能够证明 Ash 可以加强连接，重建社会联系。

### 价值模型的演示

基本上，当我们看到用户输入时，我将通过运行我们的价值模型来演示其价值。我们的价值模型会追踪大量信号随时间的变化。

在这个例子中，它正在比较原始消息。这些数字并没有经过精确校准，我不会深入解释。但我们可以看到模型在各种信号上的对比，比如用户是否会忽略 Ash 的建议，或者感到困惑。

这些信号可以预测接下来会发生什么，比如我们是否预计用户会忽略 Ash 的建议，或者感到困惑。这些预测一直延伸到建立共识（alignment）。

### 最佳回应的评估

总的来说，作为一项评估，你可以看到这里显示的最佳消息实际上是原始消息：“谢谢。我很感激你的赞美。”

你也可以看到这个更长的消息：“我可能偶尔能做到这一点，但如果我们放大一点。”它有点烦人，而且冗长。得分相似，但略低。

### 邀请体验与招聘信息

我鼓励你尝试 Ash，它今天可以在应用商店下载。我们刚刚上线，非常近期。

如果你正在寻找工作，我们是一个小型团队，通常都是资深成员。大多数人过去都担任过管理职位。我们通常是极其有使命感的人。如果这看起来是一个有价值的 AI 用例，请联系我，我就是那个带着狗的人。

---

## 英文原文

[Music] Well, great to be here. Um, today I'm going to talk a bit about how to build a foundation model for psychology. Uh, so just to introduce myself real quick, I'm Daniel. Um, I'm a machine learning engineer. I'm the co-founder and CEO at

Slingshot. You probably know there's a mental health crisis. You might not know that there's a massive shortage of mental health providers. There's about 1,500 people in need for every therapist out there if the US were evenly distributed. In most places, it's a lot

worse. This has been a problem for about 60 years. Uh JFK gave a talk in 1963 about the massive shortage mental health providers. It hasn't gotten any better. But also, the rest of the world seems to agree uh very quickly. AI AI's number one use case is now therapy. And that's

therapy being done by chat GBT for the most part. That's not very good at it. So, uh, we've tried to take a very different approach to try to actually help people with their mental health. Um, I usually at this point would jump in and demo our product. So, I'll tell

you a little bit about Ash. I'm going to jump in today and instead of showing you how Ash looks because you all can try it yourself. I'm going to show you a little bit about how we build Ash and give you a peak behind the hood. We basically train our model in three stages. Uh,

it's pretty comparable to, you know, any language model you'd be working on. So, we do three things. is we do pre-training, alignment, and reinforcement learning. Uh we've fully vertically integrated. We really obsess over every detail of what it takes to

train a model like this. So that means that we focus on every element of the experience. You know, what does an AI talk about in the context of mental health? How long should an AI pause when it's when you're talking in voice mode?

How long would be appropriate to let the person stop and think? When do you interrupt them? But for the most part, it all comes down to learning from data. So the last generation of mental health companies generally had like a philosophy, an approach, a theory and

thought, hey, if everyone just knew what I knew, thought the way that I thought mental health would be solved. It was usually CBT. Maybe you have like a leader and you're like, let's take his book and let's try to put it into people's minds. Uh we take a very

different approach. We learn from all kinds of modalities of therapy. CBT, DBT, ACT, IFS, psychonamic therapy, motivational interviewing, sematic therapy. We learn from uh practices and people who are uh going to be a better fit for a more emotionally focused

experience or more cognitively focused, more open-ended or more directed, more spiritual or more secular. And we put it all together into one model. And then we bring in our clinical team. So we have a full-time clinical team that works to align our model and that's to shift from

the kind of things that humans do to what would be appropriate with AI. When we first got started, we thought that the way people would interact with AI would be much more similar to humans than it is. You know, we had this dream of the AI touring test and we're like,

hey, if we could just learn from enough data, most people do therapy on Zoom. If we can do the same thing, you know, we can obviously do therapy. Uh, and what we've seen is the way that people interact with AI, they open up much more quickly for one thing. So, we often have

the conversations where someone starts with like, uh, you know, Ash's like, "Hey, ready to get started?" And you're like, "Yes, I'm gay." and I've never told anyone that what do I do? Um it's very different. People have this kind of like expectation of a lack of judgment.

People expect that they can. Anyway, so we um at the alignment stage, we have to shift. We have to introduce policies. We introduce guardrails. And I'm going to give you a little taste of that today. Um and then finally, we do reinforcement learning. Most mental health providers

don't get any opportunity to learn what works, right? They're always wondering what were those magic words that I said that had an impact? Did it have an impact? What's going to happen way later? uh we have a huge amount of signal that we can learn from every

conversation. So that's signal like uh what did the person uh you know how long did the person take to respond? Did they start crying? Did they say I've never shared that with anyone else before?

That was my first time saying that out loud. Did they say hey I tried that thing you said last week and it went super well or I tried that thing you said last week and it went horribly wrong and it was terrible and you suck.

We learn from all of this and it allows us to learn through continual online RL. I'm going to give you a little taste behind the hood and not spend all our time on slides. Um, so let me jump in and I'll show you a little bit about and this is actually I think the first time

that I've shared much about how Ash is built. Um, so here's a little peak behind the hood. Uh, we do a lot in terms of how we train Ash. I'm going to take you through I think some of our major tools and some of the major workflows that we use internally. Um the

first thing is I mentioned that we train on uh on pre-training data and I think uh most important thing about pre-training data is just having really high quality data. So we train on a huge amount of data. Not all of it is conversational. Um we get this through

partnerships with behavioral health organizations um that we obtain uh ethically with consent of course. Um I'm going to sh I mean you I just wanted to give a little taste. I was like looking through uh we do quite a bit of pre-processing as you can see to analyze

the conversations to understand what makes sense for AI what doesn't using especially small models but I think it's also fascinating because we don't really necessarily realize how bad AI today is in a mental health context and how awesome it could be so if you just look

you can see the kind of I'll just brought up a couple of examples to give that taste and these were actually literally the first two random uh conversations smart data set I pulled out um these are all anonymized by the way we make significant changes is to

make sure that we have no way to connect this back to any humans. Um, you can see the like did you melt down at that point? You're flying into a rage sort of maybe. And then when you come down off of that, do you feel this guilt and remorse and everything? Do you melt

down? The person says, I mean, I feel like a piece of garbage. Is the recovery just as bad as the actual rage? Yeah, I would say, you know, it's and you can see the person. Um, if you could identify where you trip the circuit before you get to that point, you'd be

in a lot less hot water, right? we could try to figure that out. Is there anything going on during that time that was making it worse? Compounding issues like substance abuse or anything like that, bad job that you don't like or something like that. Um, and what you

notice is just like obviously this is deep into a conversation. Uh, that's not the first conversation this user's had. Um, and these are again with uh humans, not with an AI. Let's jump into another. You can see I find these so fascinating to watch

just these are this is kind of like the richness behind mental health and magic. You know, you can see um but we want to make it about you, not so not some people are trustworthy. I can trust some people. And you can see that the therapist is kind of coaching them on

some of these words. Um you know, and therapist says or I can choose who to trust. Yeah, that works too. Which one sounds more true? I can trust some people or I can choose who to trust. I can choose who to trust. Um, all right. I'm gonna move on, but I

think this sometimes is just really important. Um, just to see why pre-training is so important. Like realistically, we love to talk about prompt engineering, but there are these use cases where you have data sets that are just not present in the pre-training

of large language models because they're not available on the internet because they're not able to be collected securely and ethically. And I think once you put that into a model, you realize how much more you can achieve through pre-training, through learning from, you

know, a large corpus rather than trying to have one philosophy. All right, so I'm going to get back into our tools. That was on the pre-training side. Um, post pre-training, our model is kind of funny. It has a lot of capabilities, but it doesn't have any particular direction

that it goes in. It doesn't know what's appropriate in this context and what's not. Um, so I'm going to share one of many flows that we take towards aligning our model. But one thing that we do, I was just going to run through is we have this concept of behaviors. So our

behaviors is kind of a stack that we use to understand uh weird things the model does, interesting things the model does. Um, this is our ability to monitor online through anonymized data. When you sign up to the app, you'll see that we have an optin to allow us to use the

data to improve the model. uh about 70% of our users opt in. Um for the other 30% we have absolutely no access and there's nothing we can do. For the uh people who do opt in we store completely separate from the users and that's the kind of data we can analyze. So one

really funny thing is um as telling the user that they did something an AI can't possibly do. So the way that we look through data to understand this is we build very quickly data sets especially from just a couple synthetic examples to train a really small model. So you can

see these examples of like this is something Ash actually said. So I was talking about my friend and then I remember this other time I was at the park with my dog and we saw this really I don't know what the context was but obviously an AI can't do that. So we're

able to then like search through and hopefully and identify some cases. Sure I'll tell you a story about the time I tried to learn how to snowboard. So this was a few years ago. Um I mean you can see here it's not horrible you know telling a story but there's still some

sort of violation of what we would be aiming for with an AI talking in first person. And so if I hit annotate, and I'll hope everything's up and running right now. Um, and you can see that we have a couple different models. Uh, we have

our, uh, llama base model. We have our SLG, our own base model, and a Quen model that I'm comparing at the moment. Don't know what's up with llama. And you can see, you know, I think I'd rather hear one from you or a story you say. I can do that. Um, so let's say for the

moment that we would prefer our clinical team that spends their time on these kinds of interfaces where we can just indicate to the model basically through a DPO example that we prefer this message over this one and let me save it as a draft and I could also attach um,

you know, this is like a human behavior let's say that was unacceptable. We would tag these to understand what was wrong and then we use this u both for direct preference optimization and also to track and create evals to understand the kinds of unacceptable behaviors that

an AI might do and what might be considered better. Um so that's a little bit about alignment. Um we have quite a few more things around alignment I can show but I want to get into a little bit about reinforcement learning. The thing that's interesting about a conversation

like the ones that we have is that they are they're long, right? they're they can go on for months. There's no definitive end. So if you think compared to like a game of chess where you have like a definitive end, we don't have that. On the other hand, you have a huge

amount of signal. So in a game of chess, the kind of machine learning approaches you would take would generally involve value models. We uh I'm not going to go into a huge amount of technical detail, but the key idea in chess is that you don't need to play the entire game of

chess to know how good a move is. You can actually look at the board and get a sense of how good the state of the board is, right? Like how many pawns in our context, there's a huge amount of signal that you can get from the conversation, how open someone's being or how closed,

how connected they're feeling. We learn from all of that signal and put it together into one model. Fundamentally for us, we have uh four goals that we think of and we think of them as sequential and correlated. First and foremost, we want to build intent with

the user. We just want them to be talking intentfully in a mental health context. It's okay if they don't solve all of their life's problems, but they want to. They're here for the right reason. We want to build a therapeutic alliance or working alliance, which is a

sense that you're working on the right thing, that you're working on it in the right way, that you're collaborating to set goals, that you've developed a relationship with respect. From that, we want to achieve psychological change.

And there are huge number of indicators of psychological change to know that it's happening, to know that it's in progress. And finally, we want behavioral change. And that's when the person says, um, you know, I'm lonely and I have no friends. We want them to

have friends. The coolest thing we've actually been able to show with Ash so far, and I'll dive into the RL. Uh, but we're about to share our first study that we conducted with NYU. We've actually demonstrated significant changes on all of these axes. I think

behavioral change being the coolest one. On average, people who use Ash in our study had one more friend or close personal connection on average after using Ash for about 10 weeks. So compared to AI when you think about chachi and equivalent on average people

are actually more lonely they become less connected the more they use AI for these purposes it replaces human connection but if you just optimize for these kinds of objectives we have been able to show that ash can strengthen connections rebuild that social fabric

so basically when we get I'm just going to demonstrate kind of the value model take a peek by running our value model here so our value model is tracking a whole lot of signals over time and you can see in this case it's comparing this original message. Uh, and these numbers

are not calibrated. I won't go into too much detail. Um, but we can actually see how the model compares on a whole bunch of different signals like the like and these are likelihoods over time of what we expect to happen next. So these are things like um whether we expect the

user to ignore what Ash says or be confused and it goes all the way towards building alignment. Um, and overall as an assessment you can see here that the best message actually was the original one. Thank you. I appreciate the compliment. And

you can see this longer message. I might be able to do the kind of thing from time to time, but if we zoom it. Yeah, it's kind of annoying and verbose. Still okay. Similar score, but a little bit lower. I would encourage you to try Ash.

It's available today on the app store. We've just launched. Uh, so we we're just live as of very recently if you want to give it a try. And if you are looking for a job, we are a small team. Uh, we tend to be quite a senior team.

Most folks have been managers in a past role. Uh, we tend to be extremely missiondriven. If this seems like a valuable use case for AI, please, I'm the guy with the dog.
