# Real2Sim Skills

当前版本：**v1.1**。Git 标签 `v0` 保留更新前的流程基线。

[Real2Sim Prompt v1.1](skills/real2sim-prompt/SKILL.md) 包含两步：

1. 多视角真实视频 → Blender 场景与动作重建、交互关键帧五问及对照输出。
2. Blender → MuJoCo 结构与接触迁移、物理抓取/操作校准及独立验收。

v1 增强：材质、纹理、灯光与主要背景补全；MuJoCo 原生轨迹回传 Blender 精细渲染；多视角联合拟合与留出帧检查；有假设、检查实际生效参数的接触校准。保留逐事件五问、异常前后检查和用户接受后的停止条件。

v1.1 增加每场景最多 **5 轮修正闭环**：基线为第 0 轮，有阻塞且可继续时必须迭代，验证通过提前停止，达限明确交付未解决项；续做不重置计数。

## 使用

将 `skills/real2sim-prompt` 文件夹放入 Codex 的个人 skills 目录 `~/.codex/skills/`，使用 `$real2sim-prompt` 调用。保留完整文件夹，入口会按需引用 `references/` 中的说明。

[Real2Sim Prompt.md](Real2Sim%20Prompt.md) 是便于直接阅读的入口副本。主要维护文件位于 `skills/real2sim-prompt/`。

## 范围

本仓库发布操作流程与参考说明，不包含场景数据、模型权重、Blender/MuJoCo 场景资产或通用转换程序。文档内的本地案例路径仅说明经验来源，不代表这些案例已经打包。任务成功、几何验收和视觉对齐分别记录。
