# 视频拆解与复刻清单

整理了一批用于「拆解参考视频、再复刻」的开源项目，以及 X 上相关的帖子。星标数为 2026-10-30 的数据。

## GitHub 开源项目

| 项目 | 星标 | 语言 | 一句话说明 |
| --- | --- | --- | --- |
| [edenfunf/reelmimic](https://github.com/edenfunf/reelmimic) | 273 | JavaScript | 丢进一个喜欢的视频，拆解后生成同风格的新视频 |
| [dingtom336-gif/viral-video-replicator](https://github.com/dingtom336-gif/viral-video-replicator) | 53 | 无代码（Claude Code 技能） | 爆款带货视频逆向分析，生成 Seedance 2.0 复刻提示词 |
| [keng1304/video-breakdown](https://github.com/keng1304/video-breakdown) | 7 | Python | 拆解镜头、运镜、色彩、音乐，生成 Seedance 和 Kling 提示词 |
| [getvrex/video-analyst](https://github.com/getvrex/video-analyst) | 3 | Python | 用 Gemini 分析视频，输出 Veo 3 复刻方案 |
| [lewisluc87-hub/video-to-prompt](https://github.com/lewisluc87-hub/video-to-prompt) | 1 | Python | 本地镜头检测与 OCR，生成 Sora、Runway、Veo 提示词 |

## 怎么用

- **reelmimic**：需要 Node 22.18+、Python 3.10+，并在本机装好 Claude Code 或 Codex CLI。把参考视频（文件、手机录屏或 YouTube 链接）交给它并说明想做什么，它先拆解剪辑节奏、镜头、转场和色彩，给出分镜方案供你确认，再由多个 AI 代理分工制作并逐镜头复核。MIT 许可。
- **viral-video-replicator**：Claude Code 技能。流程是 FFmpeg 抽帧、语音转录、视觉分析，最后生成 Seedance 2.0 提示词，支持 4 种素材替换模式，并附即梦平台的操作指引。仓库没有声明许可证。
- **video-breakdown**：Claude Code 技能。重启 Claude Code 后直接说「拆解这支片」并附上 YouTube 链接或本地 mp4，输出每镜起止、景别、运镜、色彩指纹、音乐结构以及 Seedance 和 Kling 提示词。MIT 许可。
- **video-analyst**：下载 YouTube 或 TikTok 视频，用 Gemini 2.5 Flash 分析，输出逐场景的复刻方案，包含 Veo 3 视频提示词、Nano Banana 2 图像提示词和配音文本，内置多种画风。仓库没有声明许可证。
- **video-to-prompt**：命令行工具，运行 `video2prompt clip.mp4` 即可得到逐镜头提示词；加 `--no-llm` 完全离线，加 `--mode breakdown` 得到逐场景拆解。MIT 许可。

## X 上的相关帖子

- [xilo：像素级拆解工作流](https://x.com/xilo2991/status/2110601513223782418)，不 1:1 复刻，只学参考视频的节奏和状态
- [blune66：hypit + Codex 拆解爆款视频](https://x.com/blune66/status/2107731501043548671)，不到 2 分钟把创作逻辑逐帧结构化
- [youguqi2023：视觉思考模型视频拆解](https://x.com/youguqi2023/status/2111271945358786815)
- [RockTheWind：把喜欢的视频丢给 GPT 逐项拆解](https://x.com/RockTheWind/status/2109848876803072264)，拆开场、镜头、节奏、台词、表情
- [MoyuAI：开源 Video to Prompt 工具](https://x.com/MoyuAI/status/2108307949244596621)，带时间码的分镜级提示词




















