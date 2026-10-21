# bili-ops-media

B站账号运营的**素材同步库**，同时作为 PoYo 生图编辑模式的**公开参考图床**。

- 只放**可公开、许可清晰**的素材：CC0 / CC-BY 的 BGM 与音效、AI 生成的人设图/画面/封面。
- **不放**：账号凭据、SESSDATA、API key、私人素材、未授权内容、视频成片。
- 公开仓库，raw 链接可直接作为 PoYo 的 `image_urls` 使用。

## 目录

```
media/persona/<版本>/   人设参考图（如 v1/ref-front.png）
media/bgm/              BGM（CC0 / CC-BY / Suno 生成）
media/sfx/              音效
media/covers/           封面与标题图
licenses/               许可台账（每份素材一条）
docs/                   使用说明
```

## 原始文件 URL

```
https://raw.githubusercontent.com/lucifercon1-hue/bili-ops-media/main/media/persona/v1/ref-front.png
```

推送到 `main` 后 raw 链接通常 1–2 分钟内可用；404 时稍等重试。链接必须指向**文件本身**，不是 GitHub 页面。

## 许可

- 每份素材在 `licenses/` 有一条记录（来源、作者、许可证、署名要求、下载日期）。
- CC-BY 素材使用时，视频简介或结尾必须署名。
- 来源不明、许可含"非商用"限制的素材不得进入本仓库。
- AI 生成素材在 `licenses/` 记录模型、task_id、credits 与生成日期。

## 大小建议

- 单文件 ≤ 5 MB（参考图越小上传越快、PoYo 拉取越稳）。
- 视频成片不要放本仓库，走本地 `drafts/` + 平台投稿。
