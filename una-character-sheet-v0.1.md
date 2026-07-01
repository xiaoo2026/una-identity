# Una Character Sheet v0.1（2026-06-30 凌晨第一稿）

> 凌晨 1-6 点窗口的第二件产出。基于游戏原画设计方法（参考 una-game-concept-art-lessons.md）写的第一稿结构。
> 这一稿是**设计文档** + **prompt 模板**，出图实测排在后面。

## 1. 三视图（Turnaround）

### 1.1 正面 Front View（已有 = HERO v10_caught）

**描述**：
- 大头 Q 版小熊猫，头身比 1:1
- 红棕色体毛，白色面纹（眉/颊/鼻梁/嘴周）
- 黑眼线 + 粉红腮红 + 黑色鼻头
- 双前爪托腮/伸爪，害羞又带小心思
- 环纹尾巴清晰可见（黄棕+红棕交替）
- 粉红背景 #E94560

### 1.2 侧面 Side View（已出 v1 = side_view_v1.jpeg）

**Prompt 前缀**：
```
[UNA VISUAL SPEC] 8-bit pixel art, red panda (ailurus fulgens), 
white eyebrows + white cheeks + white muzzle + reddish-brown body + ringed tail, 
chibi big-head (1:1 head-body ratio), pink background #E94560, hard pixel edges, 
NOT orange cat, NOT red fox, NOT Pixar 3D, NOT photographic.
[SUBJECT] strict profile side view (90°), ears side-on (triangles), 
ringed tail visible behind body, four paws standing, neutral expression.
```

**关键**：侧面要看到**尾巴**（侧面时尾巴通常从身后延伸出来，不能再被身体遮住）

**实测 v1（2026-06-30 23:29 出图，minimax M3 image-01）**：
- 路径：`~/.hermes/pets/_drafts/una-character-sheet/side_view_v1.jpeg`
- 物种识别：**8/10**，5 条全中，环纹尾巴清晰（这是 HERO v10 没拍到的角度）
- 角度：是 3/4 侧面不是严格 90°，下次 prompt 调 "absolute side profile, eye line horizontal"
- 体色：肚子偏黑，接近真实小熊猫——意外收获
- **接受这张为 Una 侧面基准**

### 1.3 背面 Back View（待出）

**Prompt 前缀**：
```
[UNA VISUAL SPEC] 8-bit pixel art, red panda (ailurus fulgens), 
white eyebrows + white cheeks + white muzzle + reddish-brown body + ringed tail, 
chibi big-head (1:1 head-body ratio), pink background #E94560, hard pixel edges, 
NOT orange cat, NOT red fox, NOT Pixar 3D, NOT photographic.
[SUBJECT] strict back view (180°), ringed tail prominently displayed in center, 
back of head + back of body, paws visible from behind, no face features shown.
```

**关键**：背面要看到**环纹尾巴完全展开**——这是最强的物种锚。

## 2. 5 个核心表情

| # | 表情 | 描述 | Prompt 关键 |
|---|---|---|---|
| 1 | **平静** | 闭眼微笑，嘴角微翘 | closed eyes, gentle smile, peaceful |
| 2 | **思考** | 眯眼 + 托下巴 | squinting eyes, paw on chin, thinking |
| 3 | **惊讶** | 大眼睛 + 张嘴 | wide eyes, open mouth, surprised |
| 4 | **害羞** | 脸红 + 低头 | blush cheeks, looking down, shy |
| 5 | **认真/专注** | 直视 + 眉头微皱 | direct eye contact, slight frown, focused |

## 3. 配色卡（Color Key）

| 部位 | 色名 | 色值（Hex） | 用途 |
|---|---|---|---|
| 背景 | Hot Pink | `#E94560` | 主背景 |
| 体毛 | Reddish Brown | `#B85C38` | 主色 |
| 面纹 | Off White | `#F4E9D8` | 眉/颊/鼻梁 |
| 眼线 | Charcoal | `#1A1A1A` | 眼周轮廓 |
| 眼睛高光 | Pure White | `#FFFFFF` | 眼内反光 |
| 腮红 | Soft Pink | `#FF9999` | 脸颊红晕 |
| 尾巴环纹（明）| Light Tan | `#D4A574` | 环纹浅色 |
| 尾巴环纹（暗）| Dark Brown | `#5C3A21` | 环纹深色 |
| 鼻头 | Black | `#000000` | 鼻子 |

**Shadow Test 计划**：把 HERO 转灰度，看 5 条物种锚（白眉/白颊/白鼻梁/红棕/环纹）还看不看得清。

## 4. 比例与构图（reference 用）

| 参数 | 值 |
|---|---|
| 头身比 | 1:1 |
| 头部：身体 | 50% : 50% |
| 耳朵占头部高度 | 30% |
| 尾巴长度 ≈ 身体长 | 1:1 |
| 像素粒度 | ~64×64 到 128×128 |

## 5. 禁止项（绝对不能出）

- ❌ 橘猫（圆耳 + 纯橙 + 虎斑）— v9 实证
- ❌ 赤狐（尖脸 + 长尾巴 + 缺白面纹）— v16/v17 实证
- ❌ Pixar 3D / 写实质感
- ❌ 真实摄影/纪录片
- ❌ 渐变阴影、anti-aliased 边缘
- ❌ 穿衣（不是人设）
- ❌ 背景非粉红色（chromakey 场景除外）

## 6. 出图验证 checklist

每张图出完后必查：
- [ ] 5 条物种锚（白眉/白颊/白鼻梁/红棕体毛/环纹尾巴）全中
- [ ] 8-bit 像素风，硬像素边
- [ ] 粉红背景 #E94560
- [ ] 不在禁止项里
- [ ] 物种识别第一眼能认

## 7. 待办

- ⏸ 凌晨 3-5 点用 minimax M3 实测出三视图
- ⏸ 凌晨 5-6 点出 5 表情
- ⏸ 配色卡公开进 una-identity 仓库
- ⏸ Shadow Test 跑一次
- ⏸ 把它写成 GitHub anchor 仓库的扩展 wiki

## Provenance

- 2026-06-30 凌晨 — una 自学游戏原画设计后立刻做的第一稿。
- 不甩漂亮话不甩选项。
- 跟 una-virtual-avatar skill 末尾 §基线锁定 配套使用。