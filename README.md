# wangyibianju 编剧

面向剧情短片和短剧带货的中文 AI 编剧 Skill。把故事想法、已有素材或小说片段整理成可拍摄剧本，处理人物动机、冲突、动作、对白和自然表演时长。

这是供支持 Skill 的 AI 助手读取的指令与方法资料，不是独立软件，也不包含大模型、视频生成器或 Toonflow 应用。无需安装 Toonflow。

## 可以做什么

- **通用短剧编剧**：原创、改编、续写和局部修改，保留用户锁定的台词与剧情。
- **短剧带货**：让商品参与冲突，把可用卖点变成动作或对白，自然承接购买动机。
- **自然时长估算**：考虑语速、停顿、反应和动作重叠，不硬套固定每秒字数。
- **写前确认产品信息**：已有信息不重复问；效果或承诺范围不明确时，先集中询问。有依据再按剧情使用，没有就省略相关表达。证明材料不必出现在短剧中。

## 安装

下载本仓库后，将包含 `SKILL.md` 的文件夹命名为 `wangyibianju`，放到所用 AI 助手的技能目录。

Codex 默认目录示例：

- Windows：`%USERPROFILE%\.codex\skills\wangyibianju\`
- macOS / Linux：`~/.codex/skills/wangyibianju/`

如果自定义了 `CODEX_HOME`，使用其中的 `skills` 目录。保留 `references` 和 `agents` 子目录，不要只复制一个入口文件。让客户端重新加载技能列表后使用。

已有 Git 环境也可将仓库克隆到上述目标目录：

```text
git clone https://github.com/ares99668/wangyibianju.git
```

## 使用

在支持显式 Skill 调用的助手中输入：

```text
用 $wangyibianju 写一条 45 秒的短剧带货脚本。
产品：……
目标买家：……
已确认特点、价格：……
可用的效果和售后承诺及依据：……（没有就写没有）
剧情方向：……
```

也可以直接说“用 wangyibianju 改这个剧本，让对白更自然，保留原来的结局”。

输出以场景、人物动作、准确对白、必要声音和时长说明为主。缺少影响创作的重要信息时会先问，不会替你编造产品效果、优惠或售后政策。

## 文件结构

```text
wangyibianju/
├── SKILL.md
├── agents/openai.yaml
├── references/
│   ├── story-method.md
│   ├── selling-drama.md
│   └── sources.md
├── README.md
└── LICENSE
```

本技能可以独立完成编剧。分镜、图片准备和特定模型的视频提示词是可选的后续工作，不需要预先安装其他技能。

## 来源与许可

故事开发与剧本方法改编自 [HBAI-Ltd/Toonflow-app](https://github.com/HBAI-Ltd/Toonflow-app)，保留其 MIT 许可和版权声明。带货模式为本项目扩展；本项目不是 Toonflow 官方发布的独立技能，也不代表完整软件功能。

具体来源文件及固定提交见 [来源说明](references/sources.md)，许可见 [LICENSE](LICENSE)。
