# 来源与改编边界

上游：[HBAI-Ltd/Toonflow-app](https://github.com/HBAI-Ltd/Toonflow-app)。核查日期：2026-11-13。固定源码提交：`6086cdffceb704a632eca143dd16cd461a78cdac`。原项目采用 MIT 许可，版权声明见本技能目录 LICENSE。

本技能由 Codex 按用户要求改编，不是 Toonflow 官方发布的独立 Skill，也不是完整软件的功能复制。

所参考的上游文件：

- [packages/skills/workflow/references/sourceAndScript.md](https://github.com/HBAI-Ltd/Toonflow-app/blob/6086cdffceb704a632eca143dd16cd461a78cdac/packages/skills/workflow/references/sourceAndScript.md)
- [packages/skills/workflow/references/methods/storyDevelopment.md](https://github.com/HBAI-Ltd/Toonflow-app/blob/6086cdffceb704a632eca143dd16cd461a78cdac/packages/skills/workflow/references/methods/storyDevelopment.md)
- [packages/skills/workflow/references/methods/screenAdaptation.md](https://github.com/HBAI-Ltd/Toonflow-app/blob/6086cdffceb704a632eca143dd16cd461a78cdac/packages/skills/workflow/references/methods/screenAdaptation.md)

保留故事因果、可拍摄表达和自然时长估算方法；重写为独立对话流程，移除画布私有工具、节点标识、应用数据库及特定模型参数依赖。本仓库只包含编剧技能，未迁移导演台、三维 UI、渲染、模型服务或后台自动化。

2026-11-13 项目扩展：新增短剧带货模式，包括商品参与冲突、卖点演示、自然成交承接，以及写前确认效果／承诺依据的规则，见 [selling-drama.md](selling-drama.md)。依据用于写前核实，不强制在片中展示证明材料。这部分是 wangyibianju 的扩展，不是上游功能声明。
