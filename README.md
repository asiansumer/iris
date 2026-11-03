<p align="center">
  <img src="images/icon-app.png" width="112" alt="Iris 的图标：一朵鸢尾花">
</p>

<h1 align="center">Iris</h1>

<p align="center">一个只用声音交流、会长期记住我的个人 AI。<br>长期目标：数字世界的我。</p>

<p align="center">
  <img src="images/app/iris-call.gif" width="250" alt="和 Iris 通话：花随着在听、在说变化">
  &nbsp;&nbsp;&nbsp;
  <img src="images/clio-pen.gif" width="296" alt="Clio 的笔：我说话时它一边听一边记">
</p>

<p align="center"><sub>左：和 Iris 通话。右：Clio 的笔，我说话时它边听边记。</sub></p>

> 这个仓库放的是项目介绍、架构和截图，**不含源代码**。项目还在原型阶段，在我自己的 iPhone 和 Mac 上运行。

## 为什么做

从 AI 刚出现，我就想要一个属于自己的 AI，之后每隔一段时间就试一次。2026 年 2 月我用 OpenClaw 搭过一版，后来因为额度、Telegram 兼容、各种 bug，还有记忆的重点一直不清楚，就放下了。

这一次我换了顺序：**先把记忆设计清楚，再写代码。**

我想要的效果是：几个月后我问它“我最开始为什么做这个项目”，它能分清哪个是最早的念头、哪次是尝试、为什么放弃、什么时候重新开始，并且拿得出我当时的原话。

## 目标

长期目标是“数字世界的我”。它持续积累我的经历、做选择的原因、目标以及这些东西的变化，主动加深对我的理解，通过一套我自己设计的语音体验和我交流。

**档案长期保留，理解可以纠正，模型和界面可以更换。**

落到具体的事情上：

- **说过的就留下。** 我说过的话先可靠保存，再去整理。每条都有出处，能找回、能纠正、能恢复。模型认为“不重要”，不能成为丢掉原话的理由。
- **分清来源。** 当时说的、事后回忆的、AI 推测的，分开存，回答时也分开说。AI 的猜测不能变成证据，同一件事讲两遍也不会变成两条证据。
- **能改正。** 纠正一处，依赖它的摘要、画像、待问的问题和还没播出的语音都会跟着更新。旧的错误不会因为换了个问法又冒出来。
- **按问题回忆。** 问“当时为什么”就去找起源；问“现在怎样”就看最新的决定；问“我是不是总这样”，要找跨时间的例子，也要找反例。不能只看哪条最近、哪条字面最像。
- **只用声音。** 没有文字聊天。什么时候接话、怎么被打断、用什么声音，都是自己设计的。
- **有分寸地主动。** 问题要有依据、挑时机，不拿提问的数量衡量效果。

## 两个角色

|  | **Iris** | **Clio** |
| --- | --- | --- |
| 是谁 | 和我说话的那个 AI | 管记忆的、数字版的我 |
| 在哪 | 主界面，打开 App 就是 Iris | “我”页里的一个入口 |
| 样子 | 一朵鸢尾花，也是 App 里唯一有颜色的东西 | 一支墨色的笔，边听边写 |
| 声音 | Anna（ElevenLabs） | 我自己的克隆声音 |
| 做什么 | 聊天、回忆，在合适的时候问我问题 | 整理每一条新记忆；觉得不对就找 Iris 商量；空闲时自己想事情 |

Clio 发现记忆不对劲时会去找 Iris 商量，比如和已有的记忆冲突、时间或人物说不清、Iris 的备注比我的原话说得更肯定。商量最多四句，结论只有四种：照记、改了再记、先放着等问我、不记。选“先放着”就必须附上要问我的问题，之后由 Iris 找合适的时候来问。

这段商量可以在 App 里**旁听**，Iris 和 Clio 各用自己的声音念出来。跟 Clio 说话，就是现实中的我在和数字版的我讨论问题。

## 截图

### 通话

<img src="images/app/call-states.jpg" alt="通话页的三种状态：等待、在听、在说，浅色和深色各一组">

左起依次是等待、在听、在说，浅色和深色各一组。整个界面只有花有颜色。花会跟着我的声音和 Iris 的声音动，字幕只在最终转写完成后显示一次。

### 页面

<img src="images/app/pages-light.jpg" alt="Iris 页、我页、Clio 页和旁听，浅色">
<img src="images/app/pages-dark.jpg" alt="同样四个页面，深色">

从左到右：

- **Iris 页**：Iris 写下的“我现在理解的你”，每一段都标着依据了几句原话。
- **我**：搜索原话和记忆，查看统计。
- **Clio**：笔、Clio 在想的事，以及和 Iris 商量过的事。
- **旁听**：Iris 和 Clio 的商量，用各自的声音念出来。

<details>
<summary>iPad mini</summary>
<img src="images/app/ipad-mini-iris-page.jpg" width="480" alt="iPad mini 上的 Iris 页">
</details>

### Clio 的笔

<img src="images/clio-pen-strip.jpg" alt="Clio 的笔在一来一回中的几个时刻">

- 平时，Clio 用小而淡的字写自己的事。
- 我开口时，它另起一行，压低笔尖等着，差不多一个音节写一个字母。声音越大，笔画越粗。
- 想事情的时候，笔悬在纸上打小圈。
- 轮到 Clio 说话时，字写得更大、更放开。

墨刚落下时最深，十秒后干掉消失。带声音的完整一来一回见 [clio-pen-exchange.mp4](images/clio-pen-exchange.mp4)，两边的声音都是本机的示例声音。

### 本机 Dashboard

档案的权威副本在 Mac 上，Dashboard 也只在本机打开。它用一次性链接登录，主密钥不会写进网页。在这里可以查看每条记忆的来源、版本和纠正，也能看到经历、等待我确认的问题，以及 Iris 和 Clio 之间的交流。

<img src="images/dashboard/dashboard-overview.png" alt="Dashboard 概览">

<table>
  <tr>
    <td><img src="images/dashboard/dashboard-memories.png" alt="记忆列表"></td>
    <td><img src="images/dashboard/dashboard-memory-detail.png" alt="一条记忆的来源与版本"></td>
  </tr>
  <tr>
    <td align="center"><sub>整理后的记忆</sub></td>
    <td align="center"><sub>一条记忆的原话、来源和版本</sub></td>
  </tr>
  <tr>
    <td><img src="images/dashboard/dashboard-questions.png" alt="待确认的问题"></td>
    <td></td>
  </tr>
  <tr>
    <td align="center"><sub>待确认的问题，以及 Iris 和 Clio 的交流</sub></td>
    <td></td>
  </tr>
</table>

<sub>Dashboard 截图用的是一份单独的演示档案，不是我的真实档案。</sub>

## 架构

```mermaid
flowchart LR
  subgraph Phone["iPhone（SwiftUI）"]
    UI["通话 · Iris 页 · 我 · Clio"]
    VOICE["录音、临时字幕、插话判断"]
    OUTBOX[("待发送队列")]
  end

  subgraph Mac["常开的 Mac（FastAPI）"]
    API["HTTP API<br/>Bearer 鉴权"]
    ARCHIVE[("SQLite 档案<br/>原话 · 录音 · 版本 · 纠错")]
    CHAT["Iris 聊天队列"]
    WORK["Clio 后台队列<br/>整理 → 商量 → 想法"]
    ASR["Qwen3-ASR<br/>本机转写"]
    DASH["本机 Dashboard"]
  end

  CODEX["Codex 订阅<br/>模型推理"]
  TTS["ElevenLabs<br/>流式合成"]

  UI --> VOICE --> OUTBOX -->|"局域网"| API
  API --> ARCHIVE
  API --> ASR
  API --> CHAT --> CODEX
  WORK --> CODEX
  WORK --> ARCHIVE
  CHAT -->|"按句流式返回"| UI
  API -->|"PCM 边收边播"| TTS
  DASH --> API
```

- **iPhone 是薄客户端。** 它负责说话、播放、查看和纠正。没传到 Mac 的话先存在手机里，拿到 Mac 的保存回执后才算“后台已保存”。手机不维护第二套记忆。
- **Mac 持有唯一的权威档案。** 原话和录音保存后不再改动。整理出来的记忆有版本、有来源，纠正会作为修订事件记下来。
- **两条队列分开。** Iris 的聊天优先；Clio 的整理、商量和每天的想法只在聊天空闲时领取任务，不拖慢回复。
- **模型可以替换。** 推理目前用本机登录的 Codex 订阅，转写用 Mac 上的 Qwen3-ASR 配合个人词表，语音用 ElevenLabs。规则和档案都属于这个项目，不依赖某一家的记忆功能。

更细的说明见 [docs/architecture.md](docs/architecture.md)，内容包括一轮语音对话怎么走、记忆模型、保存状态、纠错如何传递、Clio 的商量，以及 API 一览。

## 技术栈

| 部分 | 用了什么 |
| --- | --- |
| iPhone / iPad | SwiftUI，iOS 17+，没有第三方运行时依赖；花和笔都用 Canvas 实时绘制 |
| 后端 | Python 3.12、FastAPI、SQLite（schema 5），依赖用 uv 锁定 |
| 推理 | 本机 Codex（ChatGPT 订阅），不会悄悄切换成付费 API |
| 转写 | Mac 上的 Qwen3-ASR 0.6B 加个人词表；Apple 语音识别负责临时字幕和插话 |
| 语音 | ElevenLabs 流式 PCM：Iris 用 Anna，Clio 用我的克隆声音 |
| Dashboard | 本机静态页面，一次性链接换取 8 小时的 HttpOnly 会话 |

## 现在做到哪（2026-11-03）

- 后端 v0.5 在我的 Mac 上运行，iPhone 通过局域网连接，已经装到我的手机上试用。
- **已经有的：** 语音通话，流式回复和分句播放，插话判断，记忆的来源、版本和纠错，Iris 页，“我”页的统计、搜索和导出，独立的 Clio 对话，Iris 和 Clio 的商量与旁听，Clio 每天的想法，聊天结束后的记忆归并，本机 Dashboard。
- **延迟：** 真机上从说完话到第一段回复开始播放，最近四轮在 2.5 到 5.1 秒之间。首次冷启动还要更慢。
- **还没验证：** 戴耳机、锁屏和长时间打断的情况。外网访问和云备份暂时搁置。

## 接下来

按优先顺序：

1. **让记忆质量可以检验。** 统一材料分类：真实自述、愿望、举例、推断、转写疑点。再用现有资料建一套固定的回归测试，每次换模型或改提示词都重跑一遍。
2. **让晚到的补述回到原来那段经历。** 分开记录事情发生的时间、我讲述的时间和导入的时间，也记下“不确定”具体到哪一级。
3. **只问值得打扰我的问题。** 每个问题都要对应一个具体的知识缺口，有提问时机和冷却时间。
4. **让语音体验可以反复测量。** 把断句、识别、首字、首段音频和播放拆开分别计时，用固定的录音集复测。
5. **确认档案能完整搬走。** 定期在独立目录里演练恢复，核对原话、录音、出处、版本和纠正都没有变。

再往后：通过 Cloudflare Tunnel 在外面也能访问，加上云备份，需要时再迁到云服务器（保持单主写入）；之后逐步加入电脑和文件等更多来源。

## 关于这个仓库

这里只有介绍、架构文档和截图，源代码没有放进来。App 截图来自设计预览和模拟器，Dashboard 截图用的是演示档案。
