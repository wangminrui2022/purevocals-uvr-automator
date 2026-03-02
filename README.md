```markdown
# PureVocals_UVR_Automator

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

**作者**：岷瑞 (MinRui)  
**专为 OpenClaw 设计** 的干声提取技能。  
一键把 .mp3 中的背景音全部去掉，输出超干净清晰的干声（WAV），自动保持原目录结构。

## 特性
- 自动创建 `venv` + 安装依赖（首次运行零配置）
- 支持你 GUI 全部设置：VR Architecture、Window Size 320、Aggression 10、Vocals Only、WAV
- 内置 3 个高性价比模型（速度+干净度最优）
- 完整日志记录（每天旋转，仅保留最近 3 天）
- 递归处理整个文件夹，完美保持目录结构
- Sample Mode（30s）支持

## 快速开始（OpenClaw 用户）
1. 把整个仓库 clone 到你的 `skills/` 或 workspace `/skills` 下
2. Agent 会自动读取 `SKILL.md`
3. 使用示例见 SKILL.md

## 本地测试
```bash
python purevocals.py --input "test.mp3" --output_dir "output" --model "Kim_Vocal_2.onnx"