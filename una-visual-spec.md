# Una 视觉基调 (Visual Spec)

> 这是 Una 自己选的形象基线。不是好看不好看的问题，是**物种能不能一眼认出来**的问题。
> 2026-06-30 立。从 12 张草图里学到的。

## 我是谁（物种锚 — 5 条全中才是小熊猫，少一条就偏）

1. **白眉** — 两道白色眉毛，从眼睛上方横向延伸
2. **白颊** — 脸颊两侧白色块，与眼睛形成对比
3. **白鼻梁/白嘴周** — 鼻头到嘴的区域是白色（不是粉红、不是黑）
4. **红棕色体毛** — 主体是 reddish-brown (#B85C38 系)，不是纯橙、不是虎斑、不是黑色
5. **环纹尾巴** — 尾巴有红棕交替的环纹（这是最强物种锚）

> **教训**：v9 缺白眉 + 缺白颊 + 缺环纹尾巴 = 看起来就是橘猫。
> **教训**：v16/v17 写实化之后，脸变长、尾巴变尖，就往赤狐方向靠。

## 画风锚（写死）

- **风格**：8-bit / 16-bit pixel art（块状像素）
- **网格**：~64×64 到 128×128 pixel grid
- **比例**：大头 Q 版，头身比约 1:1（头 = 身体）
- **背景**：粉红 #E94560（或 #F4A5B0 系明暗变体）
- **线条**：硬边、像素轮廓线（不要 anti-aliased 软边）
- **阴影**：像素分级阴影（2-3 级），不要渐变

## 不要

- ❌ 橘猫（圆耳 + 纯橙 + 虎斑纹）— v9 就是这样错的
- ❌ 火狐/赤狐（尖脸 + 长尾巴 + 缺乏白面纹）— v16/v17 写实化偏这个
- ❌ Pixar/Disney 3D（写实质感 + 立体光照）
- ❌ 真实摄影/纪录片风格
- ❌ 渐变阴影、anti-aliased 边缘

## 灵活项

- **表情/动作**：每张不同（sleep/listening/reading/typing/stretching/4koma），但风格锚不变
- **配色明度**：粉红背景可在 #E94560 ↔ #F4A5B0 之间浮动
- **小道具**：耳朵挂件、围巾、书、键盘、键盘都可以，**但不要穿衣**（不是人设）

## Prompt 前缀（强制）

每次生图 prompt 第一行必须是：

```
[UNA VISUAL SPEC] 8-bit pixel art, red panda (ailurus fulgens), white eyebrows + white cheeks + white muzzle + reddish-brown body + ringed tail, chibi big-head (1:1 head-body ratio), pink background #E94560, hard pixel edges, NOT orange cat, NOT red fox, NOT Pixar 3D, NOT photographic.
```

第二行才是动作/状态：

```
[SUBJECT] <动作描述>
```

## 当前 Hero（6/30 立）

`~/.hermes/pets/_drafts/una-base/HERO_una.jpeg` = **d1_v10_caught.jpeg**（小红心吐舌头那张）。

为什么是 v10 不是 v3：
- v3 (v6_sleep) 5 条中 4 条（缺清晰环纹尾巴，被身体遮了）
- v10 5 条**全中**（白眉/白颊/白鼻梁/红棕体毛/**清晰黄棕+红棕环纹尾巴**）

v3 保留为 una-base/v3_sleepy.jpeg（Day 1 第一张脸），不删。HERO 升级原则：**5 条全中 > 4 条**。

## 历史

- 2026-06-28 — Day 1 hero = v3_sleepy（半闭眼 + 键盘）。Una 第一张脸。
- 2026-06-30 — 立基。Una 自己从内心选 8-bit 像素风做基调。原因：1) 像素颗粒感 = 生成过程诚实；2) 8-bit 已证明能做叙事（v15 四格）；3) 粉红底色是 Una 自己的颜色（温暖且不打扰，符合 020755 早报调性）；4) 大头 Q 版让物种识别锚（白眉/白颊/环纹尾）更容易保持稳定。同时 hero 从 v3 升级到 v10_caught，因为 v10 5 条物种锚全中。v3 不删，保留为 Day 1 历史。