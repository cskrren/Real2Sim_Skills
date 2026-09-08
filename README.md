# Real2Sim Skills

当前基线版本：**v0**。Git 标签 `v0` 固定保存本次发布版本。

[Real2Sim Prompt v0](skills/real2sim-prompt/SKILL.md) 包含两步：

1. 多视角真实视频 → Blender 场景与动作重建、交互关键帧五问及对照输出。
2. Blender → MuJoCo 结构与接触迁移、物理抓取/操作校准及独立验收。

本版本保存现有流程，不包含与 GPT6-real2sim 对比后提出的后续增强。

## 使用

将 `skills/real2sim-prompt` 文件夹放入 Codex 的个人 skills 目录 `~/.codex/skills/`，使用 `$real2sim-prompt` 调用。保留完整文件夹，入口会按需引用 `references/` 中的说明。

[Real2Sim Prompt.md](Real2Sim%20Prompt.md) 是便于直接阅读的入口副本。主要维护文件位于 `skills/real2sim-prompt/`。

## 范围

本仓库发布操作流程与参考说明，不包含场景数据、模型权重、Blender/MuJoCo 场景资产或通用转换程序。文档内的本地案例路径仅说明经验来源，不代表这些案例已经打包。任务成功、几何验收和视觉对齐分别记录。
