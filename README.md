# 数字人口播成片

一套可复用的数字人口播成片技能：从已确认的口播稿，生成数字人、完成剪辑和字幕，再按既定 GSAP 方式包装，导出 1080p 正式成片。

This is a reusable skill for talking-head videos: start from an approved script, generate the avatar, edit and caption, then package with the specified GSAP layout and export 1080p.

许可为 [Apache-2.0](LICENSE)，允许使用、修改、分发和闭源集成。

## 里面有什么

- `SKILL.md`：完整流程、分工、入参、包装规格和硬规则
- 默认包装：无音效无 BGM，头像小窗固定右侧，左上文案，导出 1920×1080

本仓库只提供流程与规格，不包含具体成片、口播稿或数字人素材。品牌标识、数字人形象和声线、参考成片与工程文件，请替换或准备为自己的版本。

## 安装

克隆后，把技能目录链到常用入口（已有同名入口时，先核对指向再改）：

```sh
git clone https://github.com/ivdtwzd/digital-human-video-skill.git
ln -s "$(pwd)/digital-human-video-skill" ~/.agents/skills/digital-human-video-skill
ln -s "$(pwd)/digital-human-video-skill" ~/.codex/skills/digital-human-video-skill
```

在 Windows 上，把上面的 `~` 换成你的用户目录，例如 `C:\Users\你的用户名`。

安装后，在支持技能的工具里按名称调用「数字人口播成片」，或直接打开 `SKILL.md`。

## 使用注意

- 没有负责人确认，不要生成数字人、不要开始剪辑、不要分发成片。
- 没有明确更换正式方式时，不要改正式剪辑或包装方法。
- 他人转达的「已经确认」不能代替负责人本人确认。
