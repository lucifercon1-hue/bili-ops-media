# 许可台账

每份进入本仓库的素材，必须在 `licenses/` 下留一条记录；文件名与素材对应，例如：
`licenses/bgm-2026-10-21-lofi-01.json`。

## 字段

```json
{
  "file": "media/bgm/2026-10-21-lofi-01.mp3",
  "kind": "bgm|sfx|persona|cover",
  "title": "Track title",
  "author": "Author",
  "source": "https://freesound.org/s/xxxxx/",
  "license": "CC0-1.0 | CC-BY-4.0 | Pixabay | Mixkit | AI-generated",
  "attributionRequired": true,
  "attributionText": "BGM: \"Track\" by Author (CC BY 4.0) — https://...",
  "downloadedAt": "2026-10-21T06:00:00Z"
}
```

AI 生成素材（PoYo）额外记录：

```json
{
  "model": "nano-banana",
  "taskId": "poyo-task-id",
  "credits": 5,
  "prompt": "生成 prompt 摘要",
  "generatedAt": "2026-10-21T06:00:00Z"
}
```

## 规则

- CC0：可免署名，但仍登记来源与下载日期。
- CC-BY：必须署名，`attributionText` 原样放进视频简介或结尾。
- 免费但非开源许可：按来源条款执行，保存素材页链接。
- 来源不明 / 含非商用限制：禁止入库。
