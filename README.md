# my_skills

私域运营 Agent Skills，适配 Claude Code / Codex / Cursor / Trae Solo。

配合 **wechat cli** 直接读取微信聊天记录和朋友圈，使用效果更佳。

---

## Skills 列表

### `/moments-diagnose` — 朋友圈内容诊断

输入你发的一条朋友圈（文字+图片描述），或描述你的发圈习惯，诊断它的：

- **定位层**：这条圈在干什么？和 IP 方向匹配吗？
- **价值层**：别人看完能得到什么？
- **信任层**：这条圈让人更信你还是更疑你？
- **转化层**：有没有让人行动的理由？
- **视觉层**：第一印象过关吗？

并给出改写建议和五层体检评分。

**触发方式：** `/moments-diagnose`、「帮我看看这条朋友圈」、「诊断我的朋友圈」、「帮我改一下这条圈」

---

### `/community-ops` — 社群运营诊断与规划

输入你的社群情况（类型/目标/现状/问题），诊断社群健康度，输出：

- 社群类型判断（引流群/粉丝群/快闪群/训练营群/交付群/铁杆粉丝群）
- 快闪群完整 3 天 SOP
- 训练营社群设计框架（三峰值体验 + 10要素规划）
- 日常活跃度维护节奏
- 优先行动清单

**触发方式：** `/community-ops`、「帮我看看这个社群」、「快闪群怎么做」、「社群不活跃怎么办」

---

## 安装方法

### Claude Code（推荐）

在你的项目目录或 `~/.claude/` 下的 `skills/` 文件夹中放入对应的 `SKILL.md` 文件：

```bash
# 下载 moments-diagnose
curl -o ~/.claude/skills/moments-diagnose/SKILL.md \
  https://raw.githubusercontent.com/orionsheep/my_skills/main/skills/moments-diagnose/SKILL.md

# 下载 community-ops
curl -o ~/.claude/skills/community-ops/SKILL.md \
  https://raw.githubusercontent.com/orionsheep/my_skills/main/skills/community-ops/SKILL.md
```

或直接 clone 整个仓库：

```bash
git clone https://github.com/orionsheep/my_skills.git
```

### Codex / Cursor / Trae Solo

将对应 `SKILL.md` 的内容作为 System Prompt 或 Agent Instruction 粘贴使用。

---

## 适用场景

| Skill | 适合谁用 |
|-------|---------|
| `moments-diagnose` | 做私域的个人IP、微商、知识博主、服务类创业者 |
| `community-ops` | 想做社群变现、训练营、快闪群发售的运营者 |

---

## License

MIT
