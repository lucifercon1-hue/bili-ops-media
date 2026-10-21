# PoYo 参考图 URL 用法

PoYo 的编辑模式要求 `image_urls` 是公开 HTTP(S) 地址。本仓库（public）的 raw 链接可直接使用。

## URL 规则

```
https://raw.githubusercontent.com/lucifercon1-hue/bili-ops-media/main/<path>
```

例：

```
media/persona/v1/ref-front.png
→ https://raw.githubusercontent.com/lucifercon1-hue/bili-ops-media/main/media/persona/v1/ref-front.png
```

## 使用注意

1. 推送后 raw 链接有 1–2 分钟缓存，404 时等待重试。
2. 必须用 `raw.githubusercontent.com` 的文件直链，**不要**用 `github.com/.../blob/...` 页面地址。
3. 参考图为多张时按 `image_urls` 数组传入（上限以模型 describe 为准，`gpt-image-2.5-flare` 最多 16 张）。
4. 人设图定稿后只升级版本、不覆盖旧文件；新版本路径如 `media/persona/v2/`。
5. 本地保留同名备份，避免链接失效或仓库迁移。
