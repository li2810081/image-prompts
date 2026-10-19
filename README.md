# image-prompts

公司提示词库（图片生成提示词模板）。

## 格式

`dist/sources/*.json` 每个文件是一个提示词来源，内容为 JSON 数组：

```json
[
  {
    "id": "cp_bg_01",
    "title": "商品换纯色背景",
    "prompt": "提示词正文",
    "description": "用途说明",
    "coverUrl": "",
    "referenceImageUrls": [],
    "tags": ["商品图", "换背景"],
    "preview": "",
    "createdAt": "2026-10-19T00:00:00Z",
    "updatedAt": "2026-10-19T00:00:00Z"
  }
]
```

- 必填：`id`、`title`、`prompt`；其余可省略。
- 平台按文件 URL 作为「提示词来源」直接抓取，修改并推送后即生效。
