---
theme: default
base: /ai-game-slides/
css:
  - ./style.css
class: text-center
highlighter: shiki
lineNumbers: true
drawings:
  persist: false
transition: slide-left
title: AI x Game Industry
---


# <span v-after class="text-6xl font-bold text-white neon-title">AI 与游戏行业：重塑边界</span>

<div v-click class="mt-4 text-white opacity-80 text-2xl tracking-widest text-shadow-md">
 课堂汇报
</div>

<div class="abs-bl m-10 flex items-center gap-4 text-left">
  <div v-click class="w-12 h-12 rounded-full border-2 border-white overflow-hidden shadow-[0_0_15px_rgba(255,255,255,0.3)]">
    <img src="https://api.dicebear.com/7.x/bottts/svg?seed=game" />
  </div>
  <div v-click class="leading-tight">
    <div class="font-mono text-white text-lg">Group_05</div>
    <div class="text-sm text-white opacity-50 uppercase tracking-widest font-light">汇报人：蒋韩烨</div>
  </div>
</div>

<style>
/* 封面霓虹标题样式 (供封面使用) */
.neon-title {
  letter-spacing: 0.15em;
  text-shadow: 
    0 0 7px rgba(255, 255, 255, 0.9),
    0 0 20px rgba(255, 255, 255, 0.4),
    0 0 40px rgba(34, 211, 238, 0.3); /* 淡淡的蓝光氛围 */
}
h1 {
  filter: drop-shadow(0 0 10px rgba(255, 255, 255, 0.2));
}
</style>

---

# <span class="text-3xl font-bold border-b-2 border-red-500 pb-2 font-mono">数据监测:行业成本危机</span>

<div class="grid grid-cols-3 gap-6 mt-16 text-center font-mono">

<div v-click class="p-6 border border-red-500/20 bg-black/40 rounded shadow-lg">
  <div class="text-red-500 text-xs mb-4 uppercase tracking-widest">平均 3A 研发预算</div>
  <div class="text-4xl font-black text-white">2亿<span class="text-red-500 text-lg">美金+</span></div>
  <div class="text-[10px] opacity-40 mt-4">PS5 世代 / 单个项目</div>
  <div class="mt-2 text-[9px] text-red-400/60">PS3 时代仅需 5000万</div>
</div>

<div v-click class="p-6 border border-red-500/20 bg-black/40 rounded shadow-lg">
  <div class="text-red-500 text-xs mb-4 uppercase tracking-widest">研发周期</div>
  <div class="text-4xl font-black text-white">5-7<span class="text-red-500 text-lg">年</span></div>
  <div class="text-[10px] opacity-40 mt-4">平均上线时间</div>
  <div class="mt-2 text-[9px] text-red-400/60">面临“上线即过时”的风险</div>
</div>

<div v-click class="p-6 border border-red-500/20 bg-black/40 rounded shadow-lg">
  <div class="text-red-500 text-xs mb-4 uppercase tracking-widest">资源存储需求</div>
  <div class="text-4xl font-black text-white">100<span class="text-red-500 text-lg">GB+</span></div>
  <div class="text-[10px] opacity-40 mt-4">内容填充量</div>
  <div class="mt-2 text-[9px] text-red-400/60">素材需求指数级增长</div>
</div>

</div>

<div v-click class="mt-12 p-4 bg-red-500/10 border-l-4 border-red-500 text-sm italic font-mono text-white/80">
  “目前 3A 游戏的研发路径在商业逻辑上是不可持续的。” —— 行业共识
</div>

---


# <span class="text-3xl font-bold border-b-2 border-red-500 pb-2 font-mono">案例对比:高投入与高风险的博弈</span>

<div class="grid grid-cols-3 gap-4 mt-8 h-[380px] font-mono">

  <div v-click class="flex flex-col border border-white/10 bg-white/5 rounded-lg p-3 relative overflow-hidden">
    <div class="absolute top-0 right-0 bg-green-500/20 text-green-400 text-[8px] px-2 py-1">SUCCESS_01</div>
    <div class="h-32 bg-gray-800 rounded mb-3 flex items-center justify-center overflow-hidden">
      <img src="/GTA.jpeg" class="object-cover w-full h-full">
    </div>
    <h4 class="text-white font-bold text-sm mb-2">《侠盗猎车手 5》</h4>
    <ul class="text-[10px] space-y-2 opacity-80">
      <li><span class="text-green-400">●</span> <b>总预算：</b> 约 2.65 亿美金</li>
      <li><span class="text-green-400">●</span> <b>研发/营销：</b> 1.37亿 / 1.28亿</li>
      <li><span class="text-green-400">●</span> <b>结果：</b> 3天营收突破 10 亿美金</li>
    </ul>
    <div class="mt-auto pt-2 border-t border-white/10 text-[8px] opacity-40 italic">数据来源: Rockstar Financial Report</div>
  </div>

  <div v-click class="flex flex-col border border-white/10 bg-white/5 rounded-lg p-3 relative overflow-hidden">
    <div class="absolute top-0 right-0 bg-green-500/20 text-green-400 text-[8px] px-2 py-1">SUCCESS_02</div>
    <div class="h-32 bg-gray-800 rounded mb-3 flex items-center justify-center overflow-hidden">
      <img src="/blackmyth.jpeg" class="object-cover w-full h-full">
    </div>
    <h4 class="text-white font-bold text-sm mb-2">《黑神话：悟空》</h4>
    <ul class="text-[10px] space-y-2 opacity-80">
      <li><span class="text-green-400">●</span> <b>总预算：</b> 约 4240 万美金+</li>
      <li><span class="text-green-400">●</span> <b>效率：</b> 极致的人均产出比</li>
      <li><span class="text-green-400">●</span> <b>结果：</b> 首月销量 2000万+ 份</li>
    </ul>
    <div class="mt-auto pt-2 border-t border-white/10 text-[8px] opacity-40 italic">数据来源: 浙江省税务局/游戏科学公开数据</div>
  </div>

  <div v-click class="flex flex-col border border-red-500/30 bg-red-500/5 rounded-lg p-3 relative overflow-hidden shadow-[inset_0_0_20px_rgba(239,68,68,0.05)]">
    <div class="absolute top-0 right-0 bg-red-500/20 text-red-400 text-[8px] px-2 py-1 z-20">FAILURE_CASE</div>
    <div class="h-32 bg-gray-900 rounded mb-3 flex items-center justify-center overflow-hidden grayscale">
      <img src="/titanfall.jpeg" class="object-cover w-full h-full">
    </div>
    <h4 class="text-white font-bold text-sm mb-2">《泰坦陨落 2》</h4>
    <ul class="text-[10px] space-y-2 opacity-80">
      <li><span class="text-red-400">●</span> <b>成本：</b> 约 8000 万美金+</li>
      <li><span class="text-red-400">●</span> <b>困境：</b> 夹在 BF1 与 CoD 间发布</li>
      <li><span class="text-red-400">●</span> <b>结果：</b> 销量远低预期，导致系列停摆</li>
    </ul>
    <div class="mt-auto pt-2 border-t border-white/10 text-[8px] opacity-40 italic">数据来源: EA Earnings / Analysts Est.</div>
  </div>

</div>

<div v-after class="mt-4 text-[11px] text-center opacity-60 font-mono">
  <span class="text-yellow-400">结论：</span> 3A 项目的高额投入并非成功的绝对保证，市场时机与内容密度是核心死穴。
</div>


---

# <span class="text-3xl font-bold border-b-2 border-yellow-500 pb-2 font-mono">日志:研发时间分配瓶颈</span>

<div class="grid grid-cols-2 gap-12 mt-12 items-center font-mono">

<div v-click class="space-y-8">
  <div class="relative pl-6 border-l-2 border-yellow-500/50">
    <div class="text-2xl font-bold text-white">70%</div>
    <div class="text-xs text-yellow-500 uppercase tracking-tighter">重复性体力劳动</div>
    <p class="text-[11px] opacity-60 mt-1">大量时间消耗在资产清理、LOD 制作、基础文案填充。</p>
  </div>

  <div class="relative pl-6 border-l-2 border-yellow-500/50">
    <div class="text-2xl font-bold text-white">15%</div>
    <div class="text-xs text-yellow-500 uppercase tracking-tighter">核心创意设计</div>
    <p class="text-[11px] opacity-60 mt-1">真正的玩法创新与叙事迭代时间被极度压缩。</p>
  </div>
</div>

<div v-click class="p-6 border border-white/10 bg-white/5 rounded-lg">
  <div class="text-[10px] text-yellow-500 mb-4">>> 瓶颈深度分析</div>
  <ul class="text-xs space-y-4 opacity-90 text-left">
    <li class="flex items-start gap-2">
      <span class="text-yellow-500">[!]</span> <b>贵：</b> 人力成本占总支出的 80% 以上。
    </li>
    <li class="flex items-start gap-2">
      <span class="text-yellow-500">[!]</span> <b>慢：</b> 传统管线无法满足玩家对“内容量”的渴求。
    </li>
    <li class="flex items-start gap-2">
      <span class="text-yellow-500">[!]</span> <b>难：</b> 工业化标准提升导致的边际效应递减。
    </li>
  </ul>
</div>

</div>


---


# <span class="text-3xl font-bold border-b-2 border-cyan-400 pb-2 font-mono">案例01:育碧的ghostwriter</span>

<div class="grid grid-cols-2 gap-10 mt-12 items-center">

<div>

<div v-click class="border-l-4 border-cyan-400 pl-4 mb-8">

<h3 class="text-xl font-bold text-white mb-2">痛点：生产效率</h3>

<p class="text-sm opacity-80 leading-relaxed">解决“贵与慢”：<br>将数月的手工文案缩短至数分钟生成。</p>

</div>

<div v-click class="bg-white/5 p-4 rounded-lg border border-white/10">

<div class="text-cyan-400 font-mono text-xs mb-2">>> 运行逻辑</div>

<p class="text-xs opacity-80">AI 自动生成 NPC 背景对话初稿，<br>由编剧审核，效率提升 <span class="text-cyan-400 font-bold text-sm">10x</span>。</p>

</div>

</div>

<div class="relative">

<div class="absolute -inset-1 bg-cyan-500/20 blur-xl rounded-full"></div>

<video autoplay loop muted controls class="relative rounded-lg border border-white/20 w-full shadow-2xl" src="/ghostwriter.mp4"></video>

<div class="mt-2 text-center text-[10px] font-mono opacity-40 uppercase">介绍视频</div>

</div>

</div>
---


# <span class="text-3xl font-bold border-b-2 border-cyan-400 pb-2 font-mono">落地实践:UBISOFT_GHOSTWRITER</span>

<div class="grid grid-cols-12 gap-6 mt-10 items-start font-mono">

<div class="col-span-7 space-y-4">

<div v-click class="p-4 border border-cyan-400/20 bg-black/40 rounded-lg">
<div class="text-cyan-400 text-xs mb-2">>> 目标对象：环境对话 (BARKS)</div>
<p class="text-[13px] opacity-90 leading-relaxed">专门处理触发式对白：如 NPC 的惊呼、闲聊、战斗喊话等。这类文本量极大但创意密度低，是 3A 游戏开发的沉重负担。</p>
</div>

<div v-click class="p-4 border border-white/10 bg-white/5 rounded-lg">
<div class="text-white/40 text-xs mb-2">>> 协作管线 (PIPELINE)</div>
<div class="flex items-center gap-4 text-[12px]">
<div class="text-center px-2 py-1 bg-cyan-900/30 border border-cyan-400/50 rounded">叙事设计师输入角色意图</div>
<span class="text-cyan-400">→</span>
<div class="text-center px-2 py-1 bg-purple-900/30 border border-purple-400/50 rounded">Ghostwriter 生成数千变体</div>
</div>
</div>

</div>

<div v-click class="col-span-5 relative">
<div class="absolute -inset-1 bg-cyan-500/10 blur-lg rounded-xl"></div>
<div class="relative border border-white/10 bg-black/60 p-5 rounded-xl shadow-xl">
<div class="text-xs font-bold mb-4 border-b border-white/10 pb-2">已部署项目系列 (DEPLOYED)</div>
<ul class="space-y-4">
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-cyan-400 rotate-45"></div><div><div class="text-[13px] font-bold">《看门狗：军团》</div><div class="text-[10px] opacity-50">Watch Dogs: Legion (技术起源)</div></div></li>
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-cyan-400 rotate-45"></div><div><div class="text-[13px] font-bold">《刺客信条》系列</div><div class="text-[10px] opacity-50">Assassin's Creed (核心部署)</div></div></li>
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-cyan-400 rotate-45"></div><div><div class="text-[13px] font-bold">《幽灵行动》等</div><div class="text-[10px] opacity-50">Ubisoft La Forge 实验室孵化</div></div></li>
</ul>
<div class="mt-6 pt-4 border-t border-white/10">
<div class="text-[10px] text-cyan-300 animate-pulse">>> 效率反馈：</div>
<div class="text-xl font-black mt-1">节省 70% <span class="text-[10px] font-normal opacity-50">的首稿撰写工时</span></div>
</div>
</div>
</div>

</div>

---

# <span class="text-3xl font-bold border-b-2 border-purple-400 pb-2 font-mono">案例02: NVIDIA_ACE_引擎</span>

<div class="grid grid-cols-2 gap-10 mt-12 items-start">

<div>

<div v-click class="border-l-4 border-purple-400 pl-4 mb-8">

<h3 class="text-xl font-bold text-white mb-2">痛点：交互瓶颈</h3>

<p class="text-sm opacity-80 leading-relaxed">解决“难”：<br>彻底废弃传统的硬编码状态机 (FSM) 与静态对话树。</p>

</div>

<div v-click class="bg-white/5 p-4 rounded-lg border border-white/10">

<div class="text-purple-400 font-mono text-[10px] mb-2">>> 神经交互逻辑 (NEURAL_LOGIC)</div>

<p class="text-[13px] opacity-80">
将 NPC 大脑替换为 <span class="text-purple-400 font-bold">本地大语言模型 (LLM)</span>。<br>
赋予其“环境理解->逻辑推理->实时表达”的闭环能力。
</p>

</div>

</div>

<div v-click class="relative font-mono">

<div class="absolute -inset-1 bg-purple-500/10 blur-xl rounded-full"></div>

<div class="relative border border-purple-400/30 bg-black/60 p-5 rounded-lg shadow-[0_0_30px_rgba(168,85,247,0.15)]">

<div class="text-purple-400 text-[10px] mb-4 flex justify-between items-center">
  <span>>> 系统遥测数据 (NVIDIA ACE)</span>
  <span class="animate-pulse text-green-400">状态: 运行中 (ONLINE)</span>
</div>

<div class="grid grid-cols-2 gap-4">

<div class="border border-white/10 p-3 bg-white/5 rounded">
  <div class="opacity-40 text-[9px] uppercase tracking-tighter">端到端延迟</div>
  <div class="text-2xl font-bold text-white mt-1">&lt; 300<span class="text-xs text-purple-300 ml-1">毫秒</span></div>
  <div class="text-[8px] text-green-300 mt-1">达到人类感知实时标准</div>
</div>

<div class="border border-white/10 p-3 bg-white/5 rounded">
  <div class="opacity-40 text-[9px] uppercase tracking-tighter">对话分支</div>
  <div class="text-2xl font-bold text-white mt-1">∞ <span class="text-xs text-purple-300 ml-1">动态生成</span></div>
  <div class="text-[8px] text-green-300 mt-1">非预设的开放式反馈</div>
</div>

<div class="col-span-2 border border-white/10 p-3 bg-white/5 rounded">
  <div class="opacity-40 text-[9px] uppercase mb-2">核心微服务技术栈</div>
  <ul class="text-[11px] text-purple-200 space-y-1">
    <li><span class="text-purple-400">[+]</span> <b class="text-white">Riva:</b> 自动语音识别 (ASR) 与 文本转语音 (TTS)</li>
    <li><span class="text-purple-400">[+]</span> <b class="text-white">NeMo:</b> 驱动本地 LLM（负责记忆、性格与护栏对齐）</li>
    <li><span class="text-purple-400">[+]</span> <b class="text-white">Audio2Face:</b> 音频实时生成高精度面部动画</li>
  </ul>
</div>

</div>

</div>

</div>

</div>



---



# <span class="text-3xl font-bold border-b-2 border-green-400 pb-2 font-mono">前沿趋势:DLSS_5_神经渲染</span>

<div class="grid grid-cols-12 gap-6 mt-10 items-start font-mono">

<div class="col-span-4 space-y-4">
<div v-click class="p-4 border border-green-400/20 bg-black/40 rounded-lg shadow-xl">
<div class="text-green-400 text-xs mb-2">>> 核心进化：从采样到生成</div>
<p class="text-[12px] opacity-80 leading-relaxed">
超越光栅化与传统光追，DLSS 5 旨在实现 <span class="text-green-400 font-bold">全神经渲染管线 (Neural Rendering Pipeline)</span>。
</p>
</div>
<div v-click class="p-4 border border-white/10 bg-white/5 rounded-lg opacity-80">
<div class="text-white/40 text-[10px] mb-2">>> 技术演进 (TECH_SPEC)</div>
<ul class="text-[11px] space-y-2">
<li class="flex items-center gap-2"><span class="text-green-400">■</span> <b class="text-white">DLSS 3.x:</b> 帧生成与光线重建</li>
<li class="flex items-center gap-2"><span class="text-green-400">■</span> <b class="text-white">DLSS 5:</b> <b class="text-green-400">全路径神经网络渲染</b></li>
</ul>
</div>
</div>

<div v-click class="col-span-8 relative">
<div class="absolute -inset-1.5 bg-green-500/10 blur-2xl rounded-2xl opacity-70"></div>
<div class="absolute -inset-0.5 border-2 border-green-500/20 rounded-2xl opacity-40"></div>
<div class="relative border-4 border-black bg-gray-900 rounded-2xl overflow-hidden shadow-[0_0_60px_rgba(34,197,94,0.3)]">
<div class="flex justify-between items-center px-4 py-1.5 bg-black/80 border-b border-white/10 text-[9px]">
<span class="text-green-400">>> NEURAL_RENDER.STREAM [LIVE]</span>
<span class="opacity-50 uppercase tracking-tighter">Target: Blackwell_Arch</span>
</div>
<video autoplay loop muted controls class="w-full object-cover aspect-video" src="/NVIDIA DLSS 5.mp4"></video>
<div class="flex justify-around items-center px-4 py-1 bg-black/60 border-t border-white/5 text-[8px] opacity-70">
<span class="text-green-300">AI 算力负载: <span class="animate-pulse">92.7%</span></span>
<span class="w-1 h-1 bg-white/20 rounded-full"></span>
<span>渲染效率提升: <span class="text-green-300">+500%</span></span>
<span class="w-1 h-1 bg-white/20 rounded-full"></span>
<span class="animate-pulse text-green-300">全路径追踪状态: 正常</span>
</div>
</div>
<div class="absolute -bottom-4 right-6 p-1 px-2 bg-green-500 text-black text-[9px] font-black rounded-sm shadow-xl z-20">RTX_5090_PROTOTYPE</div>
</div>

</div>

---


# <span class="text-3xl font-bold border-b-2 border-green-400 pb-2 font-mono">创业项目:MVP_AI_引擎增强插件</span>

<div class="grid grid-cols-12 gap-6 mt-10 items-start font-mono">

<div class="col-span-6 space-y-4">
<div v-click class="p-4 border border-green-400/20 bg-black/40 rounded-lg">
<div class="text-green-400 text-xs mb-2">>> 核心痛点 (PAIN_POINTS)</div>
<p class="text-[12px] opacity-80 leading-relaxed">
独立开发者没钱买服务器，没钱雇大量美工和编剧。<br>
<b class="text-white">高昂的 AI API 费用（Ubisoft 模式）不具备商业可持续性。</b>
</p>
</div>
<div v-click class="p-4 border border-white/10 bg-white/5 rounded-lg">
<div class="text-white/40 text-[10px] mb-2">>> 解决方案 (SOLUTION)</div>
<p class="text-[12px] opacity-90 leading-relaxed">
一个基于本地算力（Local-First）的 AI 引擎插件。<br>
<b class="text-green-400">“把 3A 级的 AI 能力带给每一个独立游戏人。”</b>
</p>
</div>
</div>

<div v-click class="col-span-6 relative">
<div class="absolute -inset-1.5 bg-green-500/10 blur-xl rounded-xl opacity-60"></div>
<div class="relative border border-green-400/30 bg-black/60 p-5 rounded-xl shadow-xl">
<div class="text-xs font-bold mb-4 border-b border-white/10 pb-2">技术栈配置 (STACK)</div>
<ul class="space-y-3">
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-green-400 rotate-45"></div><div><div class="text-[12px] font-bold">本地 LLM 推理核心 (Core)</div><div class="text-[9px] text-green-300 opacity-60">使用 llama.cpp 部署 Llama 3 (8B 参数)</div></div></li>
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-green-400 rotate-45"></div><div><div class="text-[12px] font-bold">多模态感知层 (Sense)</div><div class="text-[9px] text-green-300 opacity-60">集成 OpenAI Whisper (ASR) 和 Audio2Face (口型)</div></div></li>
<li class="flex items-center gap-3"><div class="w-2 h-2 bg-green-400 rotate-45"></div><div><div class="text-[12px] font-bold">渲染增强接口 (Render)</div><div class="text-[9px] text-green-300 opacity-60">兼容 UE5/Unity 的 DLSS 5 神经渲染接口</div></div></li>
</ul>
<div class="mt-5 pt-4 border-t border-white/10 text-[10px] text-cyan-300">>> 商业模式 (MODEL)</div>
<p class="text-[11px] mt-1 opacity-80">
B2B SaaS / 插件买断制。<br>
<b class="text-white">承诺：用户无需云端 API 费用即可运行智能 NPC。</b>
</p>
</div>
</div>

</div>

---
layout: center
class: text-center
---

# <span class="text-5xl font-black text-green-400 font-mono tracking-tighter">AI_GAME</span>

<div v-click class="flex justify-center gap-4 mt-8 font-mono">
<div class="p-3 border border-white/10 bg-white/5 rounded w-64">
<div class="text-green-400 text-xl font-bold mb-1">降本</div>
<div class="text-[10px] opacity-60 uppercase">Cost Reduction</div>
<p class="text-xs mt-2">AI 介入重复性劳动，释放 70% 创意生产力。</p>
</div>
<div class="p-3 border border-white/10 bg-white/5 rounded w-64">
<div class="text-green-400 text-xl font-bold mb-1">增效</div>
<div class="text-[10px] opacity-60 uppercase">Efficiency Boost</div>
<div class="text-xs mt-2">神经渲染与本地 LLM 彻底打破研发瓶颈。</div>
</div>
<div class="p-3 border border-white/10 bg-white/5 rounded w-64">
<div class="text-green-400 text-xl font-bold mb-1">重塑</div>
<div class="text-[10px] opacity-60 uppercase">New Paradigm</div>
<div class="text-xs mt-2">让每一个独立开发者，都拥有构建 3A 世界的可能。</div>
</div>
</div>

<div v-after class="mt-8">
<div class="text-2xl font-bold text-white border-y border-white/10 py-6 inline-block px-12 italic">
“AI 不会取代开发者，但懂得利用 AI 的开发者将重塑游戏行业。”
</div>
</div>

<div v-after class="mt-10">

<h2 class="text-5xl font-black tracking-widest text-white">Q & A</h2>
</div>

<div class="absolute bottom-4 left-0 w-full text-[8px] opacity-20 font-mono tracking-widest text-center">
REPORT_REF: CS_SO_2026_ARVIN 
</div>

---