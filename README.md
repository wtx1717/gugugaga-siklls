

# Gugugaga Style Skill

你想拥有一只会自动搬石、会把朋友沉默解释成隐藏剧情、还会把熬夜说成 `地球online` 版本缺陷的赛博咕企鹅吗？

现在它来了。

这是一个用于生成中文抽象短视频口播的 Codex skill。它不负责让你变得正常，它负责把“朋友不回消息”“睡前玩手机”“考试”“吃饭”“假期结束”这些日常小事，稳定加工成一段有口癖、有系统、有自我拆台、最后还能 `咕咕嘎嘎。` 收住的短口播。

## 这是什么

简单说，这是一个“咕咕嘎嘎式口播生成器”：

- 把朋友写成可攻略对象、受害者、沉默的隐藏 Boss。
- 把抽象视频写成 `石`，并给它安排文献价值、修为价值和友谊价值。
- 把生活写成 `嘎啦game`，把现实写成 `地球online`。
- 把手机、床、被子、外卖、考试、天气都写成有剧情的系统对象。
- 生成时尽量学结构和口吻，不整段复刻原始素材。

## 仓库结构

```text
skills/gugugaga-style/
  SKILL.md
  agents/openai.yaml
  references/
    meme-glossary.md
    style-mechanics.md
docs/
  distillation-notes.md
examples/
  sample-prompts.md
  sample-outputs.md
```

这里放的是成品 skill、公开说明和少量示例。原始视频、OCR 输出、训练批注这些“炼石炉残渣”保留在本地 `private/`，默认不提交到公开仓库。

## 安装

把 `skills/gugugaga-style` 复制到 Codex skills 目录：

```powershell
Copy-Item -Recurse .\skills\gugugaga-style $env:USERPROFILE\.codex\skills\
```

如果你的环境支持从仓库导入 skill，也可以直接指向本仓库里的 `skills/gugugaga-style`。

## 使用方式

推荐用固定前缀触发，别让企鹅猜谜：

核心触发短语：

~~~text
以咕咕嘎嘎的方式
~~~

具体使用如下：

```text
以咕咕嘎嘎的方式说朋友不回消息
```

也可以换题材：

```text
以咕咕嘎嘎的方式说熬夜玩手机
```

默认输出是一个标题加一段短口播。它会优先调用这些系统：

- `石/屎` 黑话系统
- `朋友/好感度` 关系系统
- `嘎啦game` 日常攻略系统
- `地球online` 现实网游系统
- 手机、睡觉、吃饭、考试、古文、修仙、二游等混搭母题

## 示例

输入：

```text
以咕咕嘎嘎的方式说朋友不回消息
```

可能会得到：

```text
朋友你这个已读不回是隐藏剧情吗

我操了老铁
我又有重大发现了
朋友不回消息
不是他不想理我
是我还没把好感度刷到解锁语音

你们玩嘎啦game的时候
见过刚点开角色就进结局的吗
没有吧

所以朋友沉默
其实是在给我留攻略空间
我现在继续发石
属于主线推进

朋友你就享受吧
咕咕嘎嘎。
```

更多示例在 [examples/sample-prompts.md](examples/sample-prompts.md) 和 [examples/sample-outputs.md](examples/sample-outputs.md)。

## 正经提醒

这只企鹅虽然抽象，但仓库管理还是正经的：

- 这个 skill 是风格蒸馏结果，不包含完整原始语料。
- 生成时应避免长段复刻源素材。
- 涉及擦边、冒犯性网络黑话、未成年人相关二次元梗时，应保持隐晦或避开。
- 如果要公开训练过程，建议只写方法论，不提交完整字幕、视频和批注原文。

## License

本仓库使用 MIT License。别人可以使用、复制、修改、分发这个 skill，但需要保留许可证和版权声明。
