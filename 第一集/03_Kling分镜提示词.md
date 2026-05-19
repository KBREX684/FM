# 第一集 · Kling 3.0 分镜提示词文档（Shot Prompts · v2 电影级模板）

> 用途：每个主镜头 / 子镜头一段可直接复制粘贴到 Kling 3.0 的视频生成提示词。  
> 规则：① 顶部统一 `[全局视觉锁定]`（每个 Prompt 出图时与镜头块拼接使用）；② 标注引用的素材 ID 及序号（指向 `02_美术资产提示词.md` 中 `[001]–[088]`）；③ 不包含剪辑/旁白文案；④ 镜头时长 ≤5s 单段；⑤ 优先采用 PUSH/PULL/PAN/TILT/TRACK/STATIC 等 Kling 稳定运镜。  
> 操作流程：先用 `04_关键帧提示词.md` 生成首帧 → 把首帧上传作为参考图 → 在 Kling 中粘贴 `[全局视觉锁定]` + 本镜头结构化块 → 选 5s / 高质量 → 生成。

---

## 〇、[全局视觉锁定] GLOBAL VISUAL LOCK（每镜复用，整体复制到 Prompt 头部）

```
[全局视觉锁定]
风格：cinematic semi-realistic Chinese urban manhua, soft cel-shading mixed with photoreal Asian skin micro-texture, subtle film grain, anamorphic-style highlight bloom, shallow depth of field, masterpiece quality.
角色元素绑定：strictly follow ↓ — do NOT alter hair color / hairstyle / tattoo design / clothing / body type / age / facial geometry across shots.
  · [001] 白离·正装  (CHAR-BL-FORMAL)
  · [002] 白离·便装  (CHAR-BL-CASUAL)
  · [003] 陈婷婷    (CHAR-TT)
  · [004] 李佳欣    (CHAR-JX)
  · [005] 林小双    (CHAR-XS)
  · [006] 司机      (CHAR-DRIVER)
  · [007] 胖子乘客   (CHAR-FATTY)
场景参考图：strictly follow [008]–[017] SCN-* asset IDs (春运站 / 大巴日 / 大巴夜·暖灯 / 高速·黄昏 / 高速·深夜 / 服务区·外 / 便利店·内 / 服务区·外吃面 / 大巴窗·夜).
色彩方案：Act 1–2 冷灰蓝日光 (cool grey-blue 5500K, low saturation); Act 3 系统降临 cyan-blue holographic accent; Act 5 服务区 mixed orange neon + cool fluorescent; Act 6–8 大巴夜内 warm amber 3000K reading lights + cool blue window streaks. Skin tone: natural warm Asian, no plastic sheen.
全局光照逻辑：日间靠侧窗自然漫射光做 key light, 顶部加柔光做 fill; 夜间以单点暖色阅读灯做 key, 车窗外冷光带做 rim; 服务区室内荧光顶光 + 室外霓虹环境光; 系统 UI 自身为 cyan-blue self-emissive 光源, 投出 5–10% 反弹光到角色面部。
分辨率与画质：3840×2160 (4K), 24 fps, 16:9 aspect, cinema-grade color, shallow depth of field, ultra-detailed face / hands / props consistency.
--no extra fingers, deformed face, melted hands, multiple heads, watermark, signature, garbled Chinese characters, blurry, low-res, oversaturated neon, plastic skin, hair color drift, tattoo design drift, age drift, outfit drift, NSFW exposure, exposed nipples, exposed genitalia, blood splatter, graphic violence, racist caricature.
```

> **使用方式**：每次生成单镜时，先粘贴上面 `[全局视觉锁定]` 整段 → 再粘贴对应镜号下方的 6 段结构化块（[镜头编号] / [主体与动作] / [环境与氛围] / [镜头运动] / [负面约束]）→ 提交 Kling 3.0。

---

## 第 1 场 · 春运启程·客运站

### S01-01a　EWS·客运站广场全景
**引用素材**：`[SCN-STATION-DAY]` `[CHAR-DRIVER]`(远景群演) `[PROP-MEGAPHONE]`

```
[镜头编号] S01-01a　|　[镜头时长] 5s　|　[景别] EWS

[主体与动作]
A wide aerial high-angle establishing shot of a North-China long-distance bus terminal plaza during Spring Festival travel rush, vast crowd of travelers dragging rolling luggage and red-blue striped woven bags, large red "春运" banner across upper frame, multiple parked white long-distance coaches, grey overcast winter sky at 11AM, slightly damp concrete pavement, breath visible in cold air.
- 情绪转变：远观人潮 → 渺小感升起 → 沉入疲态
- 微表情序列：0–1.7s 远观人潮；1.7–3.3s 渺小感升起；3.3–5.0s 沉入疲态
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：疲惫 · 春运 / 灰冷天光
（场景与光照参见 [全局视觉锁定] 中 SCN-STATION-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：high-angle establishing, slow PUSH-IN forward, 5 seconds, steady.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S01-01b　MLS·售票口司机喊话
**引用素材**：`[CHAR-DRIVER]` `[PROP-MEGAPHONE]` `[SCN-STATION-DAY]`

```
[镜头编号] S01-01b　|　[镜头时长] 3s　|　[景别] MLS

[主体与动作]
A 45-year-old Chinese long-distance bus driver in a dark navy quilted cotton coat and black "运" cap, weather-tanned face, holding a red plastic megaphone close to his mouth, shouting loudly at the crowd, foreground passengers passing through soft-focus, ticket gate signage in background, grey daylight.
- 情绪转变：一片嘈杂 → 喊声穿透 → 信息过载
- 微表情序列：0–1.0s 一片嘈杂；1.0–2.0s 喊声穿透；2.0–3.0s 信息过载
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：嘈杂混乱 · 嘈杂 · 春运 / 灰冷天光
（场景与光照参见 [全局视觉锁定] 中 SCN-STATION-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium long shot, STATIC tripod, slight foreground-passenger walk-by parallax, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S01-02a　MS·白离拖箱穿人群
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-LUGGAGE]` `[SCN-STATION-DAY]`

```
[镜头编号] S01-02a　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
A 26-year-old handsome Chinese man with peach-blossom almond eyes, side-parted black hair, wearing a dark-charcoal three-piece suit under a beige knee-length trench coat draped over his shoulders, polished black oxford shoes, pulling a 28-inch brushed silver aluminum spinner luggage with his left hand, his back partly to camera as he walks through a thick crowd toward a coach.
- 情绪转变：步入人海 → 自我孤立感 → 深疲沉肩
- 微表情序列：0–1.3s 步入人海；1.3–2.7s 自我孤立感；2.7–4.0s 深疲沉肩
- 动作强度 motion intensity：4/10　稳定跟移（步频节奏）

[环境与氛围]
氛围关键词：孤独 · 疲惫 · 人潮 · 春运 / 灰冷天光
（场景与光照参见 [全局视觉锁定] 中 SCN-STATION-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, smooth TRACK behind him at walking pace, slight over-shoulder, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S01-02b　CU·行李箱滚轮压地砖
**引用素材**：`[PROP-LUGGAGE]` `[SCN-STATION-DAY]`

```
[镜头编号] S01-02b　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Extreme low-angle close-up of four spinner wheels of a brushed silver aluminum luggage rolling across slightly damp grey concrete tiles, tiny water droplets splashing, mirror-faint reflection of wheels on wet ground.
- 情绪转变：轮压湿地 → 水花溅起 → 细节疲态留痕
- 微表情序列：0–0.7s 轮压湿地；0.7–1.3s 水花溅起；1.3–2.0s 细节疲态留痕
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：疲惫 · 春运 / 灰冷天光
（场景与光照参见 [全局视觉锁定] 中 SCN-STATION-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：ground-level close-up, STATIC, slight forward motion of wheels, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S01-03　MLS·白离登车回望天空
**引用素材**：`[CHAR-BL-FORMAL]` `[SCN-BUS-EXT-DAY]` `[PROP-LUGGAGE]`

```
[镜头编号] S01-03　|　[镜头时长] 4s　|　[景别] MLS

[主体与动作]
The same 26-year-old executive man steps onto the metal step of a white Chinese long-distance coach with license plate "沪 A·B8868" and route card "魔都→运市", trench coat over shoulders, luggage in hand, pausing for a beat to glance up at the grey overcast sky, breath fogging in cold air.
- 情绪转变：抬头望天 → 一口白雾 → 无声认命
- 微表情序列：0–1.3s 抬头望天；1.3–2.7s 一口白雾；2.7–4.0s 无声认命
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：离别 · 认命 · 站台 / 阴天
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-EXT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium long shot from front-side, slow DOLLY-IN, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 2 场 · 大巴最后排·三女登场

### S02-01a　MLS·车厢内最后排空位
**引用素材**：`[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-01a　|　[镜头时长] 5s　|　[景别] MLS

[主体与动作]
Interior of a Chinese long-distance coach in daytime, double rows of dark-burgundy velvet seats with cream headrest covers, most seats occupied by various Chinese passengers, the rear three-seat row at center frame empty and lit by a soft side-window beam.
- 情绪转变：入座放空 → 思绪起伏 → 预备闭目
- 微表情序列：0–1.7s 入座放空；1.7–3.3s 思绪起伏；3.3–5.0s 预备闭目
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium long shot from front of aisle, slow DOLLY-IN toward the back row, 5 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S02-01b　MS·白离落座靠窗
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-LUGGAGE]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-01b　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
The same 26-year-old executive man lifts a silver luggage onto the overhead aluminum rack, then settles into the leftmost window seat of the back row, smoothing his trench coat, eyes lowering.
- 情绪转变：落座放下行李 → 轻舒一气 → 疲意压回
- 微表情序列：0–1.0s 落座放下行李；1.0–2.0s 轻舒一气；2.0–3.0s 疲意压回
- 动作强度 motion intensity：4/10　稳定跟移（步频节奏）

[环境与氛围]
氛围关键词：缓解 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot at 3/4 front angle, smooth TRACK following his sit-down motion, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-02　CU·白离闭眼后仰
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-TIRED]` `[PROP-EARPHONE]`

```
[镜头编号] S02-02　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the same executive man's face, expression weary with heavy half-closed eyelids, slight frown, head leaning back against the cream headrest cover, black in-ear earphone cable visible at his collar, soft window daylight on his profile.
- 情绪转变：清醒紧绷 → 缓慢松懈 → 沉入疲惫
- 微表情序列：0–1.0s 清醒紧绷；1.0–2.0s 缓慢松懈；2.0–3.0s 沉入疲惫
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：疲惫
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, side 45°, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-03a　MLS·三精神小妹挤上车
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-03a　|　[镜头时长] 3s　|　[景别] MLS

[主体与动作]
Three loud "spicy girls" squeezing onto the coach at the front door: a 22-year-old with shoulder-length fire-red wavy hair, smoky eyes, multicolor Prajna half-sleeve tattoo on left arm, cropped black faux-leather jacket and short denim; a 21-year-old with lavender-purple straight hair, off-shoulder black crop top, ultra-short denim shorts, sheer ultra-thin slightly translucent black stockings (lightweight 15-denier matte-sheer, no fishnet, no rips); a 19-year-old with honey-yellow wavy hair in pink claw clip, pastel pink puffer crop, white knee-high cartoon-bear socks. They jostle and chatter loudly.
- 情绪转变：宁静 → 闯入感骤起 → 嘈杂淹没
- 微表情序列：0–1.0s 宁静；1.0–2.0s 闯入感骤起；2.0–3.0s 嘈杂淹没
- 动作强度 motion intensity：7/10　手持微抖（纪实临场感）

[环境与氛围]
氛围关键词：嘈杂混乱 · 闯入 · 生气 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium long shot at door perspective, quick PUSH-IN with very subtle handheld micro-shake, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-03b　CU·白离猛睁眼侧目
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-ANNOYED]`

```
[镜头编号] S02-03b　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up of the executive man, eyes snapped open and sharply side-glancing toward the front door, eyebrows tightly knit, mouth a flat line.
- 情绪转变：平静 → 警觉骤起 → 烦躁压制
- 微表情序列：0–0.7s 平静；0.7–1.3s 警觉骤起；1.3–2.0s 烦躁压制
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：搅扰
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-04a　MS·三女沿过道走来
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-04a　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The three spicy girls walking down the aisle of the coach, the yellow-haired girl in the lead pointing toward the empty back row with an excited expression, the red-haired one swaggering behind, the purple-haired one rolling eyes.
- 情绪转变：余光察觉 → 闯入感升高 → 心头一沉
- 微表情序列：0–1.3s 余光察觉；1.3–2.7s 闯入感升高；2.7–4.0s 心头一沉
- 动作强度 motion intensity：5/10　中速推进（强调聚焦）

[环境与氛围]
氛围关键词：日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot tracking PAN with slight PUSH-IN from rear of coach, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-04b　MS·白离 POV 三女扑面
**引用素材**：`[CHAR-BL-FORMAL]` POV，`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-04b　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
First-person POV from the executive man's seat at the back row: the three spicy girls walking straight toward camera, getting closer, slightly low angle, soft daytime side-window light.
- 情绪转变：面无表情 → 警觉抬眼 → 抗拒收紧
- 微表情序列：0–1.0s 面无表情；1.0–2.0s 警觉抬眼；2.0–3.0s 抗拒收紧
- 动作强度 motion intensity：2/10　微动（呼吸级微抖）

[环境与氛围]
氛围关键词：抵触 · 接触 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：POV medium shot, STATIC with subtle natural breathing micro-shake, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：鬼影手 / 自拍镜头反射 / POV 倒影出现拍摄者脸 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-05a　MS·三人入坐最后排
**引用素材**：`[CHAR-BL-FORMAL]` `[CHAR-XS]` `[CHAR-JX]` `[CHAR-TT]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-05a　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The back row of the coach now packed: from left to right - the executive man pressed against the window, the yellow-haired soft-faced 19-year-old plopping down right next to him, then the purple-haired 21-year-old, then the red-haired 22-year-old with tattooed arm, all jostling for space, seats creaking.
- 情绪转变：互不相识 → 挤压贴近 → 各自尴尬定格
- 微表情序列：0–1.3s 互不相识；1.3–2.7s 挤压贴近；2.7–4.0s 各自尴尬定格
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：紧张 · 被迫 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot front-on, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-05b　CU·拥挤大腿暗示
**引用素材**：`[CHAR-BL-FORMAL]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-05b　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up TILT-DOWN of the gap between two seated passengers: a man's charcoal-suit trouser leg and a young girl's bare thigh in light denim shorts pressed lightly side by side from the squeeze, no skin exposed beyond shorts hemline, tasteful framing, focus on the fabric contrast.
- 情绪转变：克制平静 → 异样触感 → 身体缩离
- 微表情序列：0–1.0s 克制平静；1.0–2.0s 异样触感；2.0–3.0s 身体缩离
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：被迫 · 贴近 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, TILT-DOWN, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S02-05c　MS·婷婷骂厂子佳欣附和
**引用素材**：`[CHAR-TT]` `[EXP-ANGRY]` `[CHAR-JX]` `[EXP-ATTITUDE]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S02-05c　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The red-haired girl mid-rant with mouth wide open in fury, brows furrowed, finger jabbing the air; the purple-haired girl beside her nodding with cold smirk and chin lifted; surrounding passengers (out of focus) turning displeased glances toward them.
- 情绪转变：突然爆发 → 持续输出 → 余怒未消
- 微表情序列：0–1.3s 突然爆发；1.3–2.7s 持续输出；2.7–4.0s 余怒未消
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：生气 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 3 场 · 一瓶水·系统降临

### S03-01a　EWS·高速公路空镜
**引用素材**：`[SCN-HIGHWAY-DUSK]`

```
[镜头编号] S03-01a　|　[镜头时长] 3s　|　[景别] EWS

[主体与动作]
Aerial side-tracking shot of a single white Chinese long-distance coach driving on an empty expressway at dusk, sky gradient deep blue to faint orange, wet asphalt reflecting sky, distant fields and pylons.
- 情绪转变：车身横移 → 旷野滑过 → 孤旅之感
- 微表情序列：0–1.0s 车身横移；1.0–2.0s 旷野滑过；2.0–3.0s 孤旅之感
- 动作强度 motion intensity：5/10　航拍跟移（大景气势）

[环境与氛围]
氛围关键词：孤旅 · 黄昏高速 / 蓝橙渐变
（场景与光照参见 [全局视觉锁定] 中 SCN-HIGHWAY-DUSK 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：drone-style smooth side TRACK matching coach speed, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S03-01b　CU·小双脸色发白晕车
**引用素材**：`[CHAR-XS]` `[EXP-CARSICK]`

```
[镜头编号] S03-01b　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the 19-year-old soft-faced girl with honey-yellow wavy hair and pink claw clip, expression motion-sick with pale slightly-green-tinted face, hand covering her mouth, watery eyes, soft warm coach interior light on her profile.
- 情绪转变：正常 → 面色发白 → 捂嘴隐忍
- 微表情序列：0–1.0s 正常；1.0–2.0s 面色发白；2.0–3.0s 捂嘴隐忍
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：电影感 · 半写实漫剧
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-02a　MCU·小双怯生生请求喝水
**引用素材**：`[CHAR-XS]` `[EXP-PLEADING]` `[CHAR-BL-FORMAL]`

```
[镜头编号] S03-02a　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
The yellow-haired girl timidly leaning toward the executive man, fingertips lightly touching his suit sleeve, looking up with big watery doe eyes and slightly parted lips; the man's profile on the right edge of frame.
- 情绪转变：犹豫 → 抬头乞求 → 大眼汪汪
- 微表情序列：0–1.0s 犹豫；1.0–2.0s 抬头乞求；2.0–3.0s 大眼汪汪
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：羞涩 · 哀求
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up at side 45°, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-02b　ECU·白离嘴角抽动
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-TWITCH]`

```
[镜头编号] S03-02b　|　[镜头时长] 1.5s　|　[景别] ECU

[主体与动作]
Extreme close-up of the executive man's mouth area, a subtle single twitch at the corner of his lips, otherwise composed face, soft window light.
- 情绪转变：面无表情 → 嘴角一抽 → 恢复克制
- 微表情序列：0–0.5s 面无表情；0.5–1.0s 嘴角一抽；1.0–1.5s 恢复克制
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：静默 · 抗议
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up, STATIC, 1.5 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-02c　CU·水瓶手边
**引用素材**：`[PROP-WATER-USED]`

```
[镜头编号] S03-02c　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up low-angle top-down of a 550ml clear mineral water bottle with blue-white "纯净水" label, water level about 80%, cap on, resting on a charcoal suit trouser leg next to a man's hand.
- 情绪转变：目光下落瓶身 → 内心犹豫 → 决定攥紧
- 微表情序列：0–0.7s 目光下落瓶身；0.7–1.3s 内心犹豫；1.3–2.0s 决定攥紧
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：微小 · 抉择
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up top-down, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S03-03a　MCU·白离冷淡拒绝
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-COLD]`

```
[镜头编号] S03-03a　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
The executive man's face in medium close-up, expression cold and detached, lips a flat line, eyes calm and dismissive, soft side-window light.
- 情绪转变：中性 → 冷淡 → 关闭交流
- 微表情序列：0–1.0s 中性；1.0–2.0s 冷淡；2.0–3.0s 关闭交流
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：疏离 · 拒绝
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-03b　MS·小双拿水瓶
**引用素材**：`[CHAR-XS]` `[EXP-BRIGHT]` `[PROP-WATER-USED]`

```
[镜头编号] S03-03b　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
The yellow-haired girl's eyes lighting up with hope and faint smile, hand reaching out and confidently taking the mineral water bottle from the man's side, very natural motion.
- 情绪转变：黯淡 → 眼前一亮 → 笑意破云
- 微表情序列：0–1.0s 黯淡；1.0–2.0s 眼前一亮；2.0–3.0s 笑意破云
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：直率 · 热情
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot 3/4 front angle, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-03c　CU·小双仰头喝水
**引用素材**：`[CHAR-XS]` `[EXP-DRINK]` `[PROP-WATER-USED]`

```
[镜头编号] S03-03c　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up side profile of the yellow-haired girl tilting her head back, eyes closed, throat visibly swallowing as she chugs from the open mineral water bottle, soft strand of hair falling.
- 情绪转变：紧张 → 仰头痛饮 → 满足收尾
- 微表情序列：0–1.0s 紧张；1.0–2.0s 仰头痛饮；2.0–3.0s 满足收尾
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：渴 · 缓解
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up side, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-03d　CU·水瓶口唇印特写
**引用素材**：`[PROP-WATER-LIPMARK]`

```
[镜头编号] S03-03d　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up of the same mineral water bottle, water level now reduced to about 30%, a faint pale-pink glossy lip print smudge visible around the bottle opening, condensation droplets on surface, bottle being handed back into a man's hand entering frame.
- 情绪转变：物件递回 → 唇印映入 → 余韵停顿
- 微表情序列：0–0.7s 物件递回；0.7–1.3s 唇印映入；1.3–2.0s 余韵停顿
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：残留 · 痕迹
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S03-04a　MCU·白离嫌弃送水
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-DISGUST]`

```
[镜头编号] S03-04a　|　[镜头时长] 2s　|　[景别] MCU

[主体与动作]
Medium close-up of the executive man, faint disgusted expression with lips slightly curled, waving his free hand dismissively as if to say "keep it".
- 情绪转变：中性 → 嫌弃微皱 → 摆手撇清
- 微表情序列：0–0.7s 中性；0.7–1.3s 嫌弃微皱；1.3–2.0s 摆手撇清
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：嫌弃 · 轻度
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-04b　CU·小双低头攥瓶子
**引用素材**：`[CHAR-XS]` `[EXP-SHY-THANKFUL]` `[PROP-WATER-LIPMARK]`

```
[镜头编号] S03-04b　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the yellow-haired girl with head lowered, faint blush on her cheeks, hands clutching the half-empty water bottle tightly to her chest, soft warm light.
- 情绪转变：局促 → 低头脸红 → 抱瓶贴胸
- 微表情序列：0–1.0s 局促；1.0–2.0s 低头脸红；2.0–3.0s 抱瓶贴胸
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：温柔 · 意外
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S03-04c　ECU·白离瞳孔系统绑定
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SHOCK]` `[FX-SYS-BIND]`

```
[镜头编号] S03-04c　|　[镜头时长] 4s　|　[景别] ECU

[主体与动作]
Extreme close-up of one eye of the executive man, dark-brown iris filling the frame, cyan-blue holographic Chinese characters and a 0-100% progress bar reflected on the wet surface of the eye, faint sci-fi scanlines and particle dust, pupil dilating with shock.
- 情绪转变：常态 → 瞳孔骤张 → 凝固呆愣
- 微表情序列：0–1.3s 常态；1.3–2.7s 瞳孔骤张；2.7–4.0s 凝固呆愣
- 动作强度 motion intensity：2/10　微动（呼吸级微抖）

[环境与氛围]
氛围关键词：觉醒 · 宇宙级
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up, STATIC with slight ZOOM-IN, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：瞳孔变形 / 双重瞳孔 / 塑料眼球 / 虹膜反光过爆 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 4 场 · 系统面板·女神雷达

### S04-01a　MS·蓝色面板悬浮
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SHOCK]` `[PROP-PANEL-MAIN]`

```
[镜头编号] S04-01a　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The executive man sitting in the coach back row, eyes fully wide and lips slightly parted in shock; a semi-transparent cyan-blue holographic UI panel floats in front of his face, displaying clean Chinese sci-fi typography: "宿主：白离 / 系统：女神投资系统 / 功能：女神雷达、投资返利". Panel softly rotated 5°, glowing edges, particle dust around.
- 情绪转变：常态 → 瞳孔骤张 → 凝固呆愣
- 微表情序列：0–1.3s 常态；1.3–2.7s 瞳孔骤张；2.7–4.0s 凝固呆愣
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：奇观
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot front-on, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：UI 文字乱码 / UI 元素崩坏 / 蓝色光晕过曝 / panel 双重叠影 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S04-01b　CU·手指穿过面板
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-PANEL-MAIN]`

```
[镜头编号] S04-01b　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the executive man's hand reaching forward, his index finger passing straight through the semi-transparent cyan-blue holographic panel without resistance, faint cyan glow on his fingertip.
- 情绪转变：伸手试探 → 指穿面板 → 错愕缩回
- 微表情序列：0–1.0s 伸手试探；1.0–2.0s 指穿面板；2.0–3.0s 错愕缩回
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：电影感 · 半写实漫剧
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up side, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：UI 文字乱码 / UI 元素崩坏 / 蓝色光晕过曝 / panel 双重叠影 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S04-01c　MCU·乘客毫无反应
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`

```
[镜头编号] S04-01c　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
Reverse-angle medium close-up of the three spicy girls and nearby passengers in the coach, all chatting or scrolling phones, none of them noticing or reacting to anything special, neutral daytime light.
- 情绪转变：环顾确认 → 他人无反应 → 暗自惊觉独享
- 微表情序列：0–1.0s 环顾确认；1.0–2.0s 他人无反应；2.0–3.0s 暗自惊觉独享
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：只我可见 · 日间车厢 / 漫射光
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-DAY 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up reverse angle, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S04-02a　CU·系统功能介绍面板
**引用素材**：`[PROP-PANEL-FUNC]`

```
[镜头编号] S04-02a　|　[镜头时长] 4s　|　[景别] CU

[主体与动作]
Close-up of a semi-transparent cyan-blue holographic UI panel hovering against a dark blurred background, sharp Chinese sci-fi typography listing "功能一：女神雷达" and "功能二：投资返利" and "倾心值：0 路人 / 60 爱慕 / 80 热恋 / 100 至死不渝", glowing edges, particle dust.
- 情绪转变：面板浮现 → 文字逐行点亮 → 规则锁定脑中
- 微表情序列：0–1.3s 面板浮现；1.3–2.7s 文字逐行点亮；2.7–4.0s 规则锁定脑中
- 动作强度 motion intensity：2/10　微动（呼吸级微抖）

[环境与氛围]
氛围关键词：规则 · 揭示
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC with very slight ZOOM-IN, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：UI 文字乱码 / UI 元素崩坏 / 蓝色光晕过曝 / panel 双重叠影
```

### S04-02b　MS·白离 POV 扫描三女
**引用素材**：`[CHAR-BL-FORMAL]` POV，`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-PANEL-RADAR]`

```
[镜头编号] S04-02b　|　[镜头时长] 5s　|　[景别] MS

[主体与动作]
First-person POV from the executive man: gaze sweeping across the three spicy girls in the back row, small cyan-blue holographic name tags popping up above each girl's head in sequence: "陈婷婷 倾心值 0 路人", "李佳欣 倾心值 0 路人", "林小双 倾心值 +10 略有好感"; scanner-like cyan grid sweep visual effect.
- 情绪转变：错愕浏览 → 信息洪流灌顶 → 嘴角悄起的贪意
- 微表情序列：0–1.7s 错愕浏览；1.7–3.3s 信息洪流灌顶；3.3–5.0s 嘴角悄起的贪意
- 动作强度 motion intensity：4/10　稳定跟移（步频节奏）

[环境与氛围]
氛围关键词：电影感 · 半写实漫剧
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：POV medium shot, smooth PAN left to right, 5 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：UI 文字乱码 / UI 元素崩坏 / 蓝色光晕过曝 / panel 双重叠影 / 鬼影手 / 自拍镜头反射 / POV 倒影出现拍摄者脸 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S04-02c　ECU·白离贪婪眼神
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-GREEDY]`

```
[镜头编号] S04-02c　|　[镜头时长] 2s　|　[景别] ECU

[主体与动作]
Extreme close-up of the executive man's eyes, blazing with fervent greedy excitement, faint upward smirk at lip corners, faint cyan reflection still in pupils.
- 情绪转变：克制 → 内火点燃 → 隐忍贪意
- 微表情序列：0–0.7s 克制；0.7–1.3s 内火点燃；1.3–2.0s 隐忍贪意
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：掠夺 · 野心 · 猎手 · 野望
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 5 场 · 服务区·十块钱投资

### S05-01a　LS·服务区夜景灯牌
**引用素材**：`[SCN-REST-AREA-NIGHT]` `[PROP-NEON-SIGN]`

```
[镜头编号] S05-01a　|　[镜头时长] 4s　|　[景别] LS

[主体与动作]
A wide long shot of a Chinese highway service area at night, large orange-red neon sign "XX 服务区" glowing on the building, white long-distance coach parked in foreground, wet asphalt reflecting neon, scattered travelers, faint mist.
- 情绪转变：驶入服务区 → 灯火扑面 → 短暂喘息
- 微表情序列：0–1.3s 驶入服务区；1.3–2.7s 灯火扑面；2.7–4.0s 短暂喘息
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：服务区霓虹 / 湿地反光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：long shot, slow DOLLY-IN toward the building, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

### S05-01b　MS·白离拎泡面出便利店
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-INSTANT-NOODLE-CUP]` `[PROP-WATER-NEW]` `[SCN-REST-AREA-NIGHT]`

```
[镜头编号] S05-01b　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
The executive man walking out of the automatic glass doors of a brightly-lit convenience store, holding a red "康师傅 红烧牛肉面" instant noodle cup in one hand and an unopened 550ml mineral water bottle in the other, trench coat still on shoulders.
- 情绪转变：紧绷未松 → 食物入手暖意 → 短暂松弛
- 微表情序列：0–1.0s 紧绷未松；1.0–2.0s 食物入手暖意；2.0–3.0s 短暂松弛
- 动作强度 motion intensity：4/10　稳定跟移（步频节奏）

[环境与氛围]
氛围关键词：服务区霓虹 / 湿地反光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, smooth TRACK in front of him, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-02a　MS·便利店内白离撕开泡面
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-INSTANT-NOODLE-CUP]` `[SCN-REST-AREA-INT]`

```
[镜头编号] S05-02a　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
Inside the convenience store at a small standing eating counter, the executive man tearing open the foil lid of the red instant noodle cup, steam rising into his face, bright cool fluorescent light overhead.
- 情绪转变：撕开盖膜 → 热气扑面 → 嘴角微松
- 微表情序列：0–1.0s 撕开盖膜；1.0–2.0s 热气扑面；2.0–3.0s 嘴角微松
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：暖意 · 质朴 · 便利店冷白光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-INT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot 3/4 angle, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-02b　MS·三女徘徊盯食物
**引用素材**：`[CHAR-TT]` `[EXP-HUNGRY]` `[CHAR-JX]` `[EXP-HUNGRY]` `[CHAR-XS]` `[EXP-HUNGRY]` `[SCN-REST-AREA-INT]`

```
[镜头编号] S05-02b　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The three spicy girls lingering in the convenience store aisle, gazes locked hungrily on other customers' food, throats subtly swallowing, the red-haired one trying to look tough, the purple-haired one feigning indifference, the yellow-haired one openly longing.
- 情绪转变：克制 → 喉头滑动 → 眼神锁食
- 微表情序列：0–1.3s 克制；1.3–2.7s 喉头滑动；2.7–4.0s 眼神锁食
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：饥饿 · 便利店冷白光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-INT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-03a　MCU·婷婷上前喊大哥
**引用素材**：`[CHAR-TT]` `[EXP-AWKWARD]` `[SCN-REST-AREA-INT]`

```
[镜头编号] S05-03a　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
Medium close-up of the red-haired tattooed girl standing in front of the counter, arms crossed over her tattooed forearm in awkward bravado, eyes shifting nervously, mouth opening to speak.
- 情绪转变：逞强 → 心虚瞟 → 强行抱臂
- 微表情序列：0–1.0s 逞强；1.0–2.0s 心虚瞟；2.0–3.0s 强行抱臂
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：迟疑 · 便利店冷白光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-INT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-03b　MCU·白离拿手机扫码
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-CALM]` `[PROP-PHONE-WECHAT]`

```
[镜头编号] S05-03b　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
Medium close-up reverse angle of the executive man calmly pulling out a black smartphone, screen showing a WeChat receive-money QR code with avatar "白离", his face composed neutral.
- 情绪转变：中性 → 微微上扬 → 控制式微笑
- 微表情序列：0–1.0s 中性；1.0–2.0s 微微上扬；2.0–3.0s 控制式微笑
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：盘算
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up reverse, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸 / 手机屏幕乱码 / 微信图标错位 / 中文字符崩坏
```

### S05-03c　MS·三女凑头商量
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-REST-AREA-INT]`

```
[镜头编号] S05-03c　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
The three girls huddled in a small circle, heads close together, whispering and gesturing, looking around to see if anyone is watching.
- 情绪转变：迅速凑头 → 低声商议 → 拿定主意
- 微表情序列：0–1.3s 迅速凑头；1.3–2.7s 低声商议；2.7–4.0s 拿定主意
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：密谋 · 便利店冷白光
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-INT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot top-down slight angle, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-03d　CU·婷婷伸一根手指
**引用素材**：`[CHAR-TT]` `[EXP-CAREFUL]`

```
[镜头编号] S05-03d　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up of the red-haired girl carefully and timidly raising one single index finger, lips bitten, big pleading eyes upward, faint hope in expression.
- 情绪转变：紧张 → 小心翼翼 → 等待回应
- 微表情序列：0–0.7s 紧张；0.7–1.3s 小心翼翼；1.3–2.0s 等待回应
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：微小 · 颤动 · 请求
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-04a　ECU·点击转账
**引用素材**：`[PROP-PHONE-TRANSFER]`

```
[镜头编号] S05-04a　|　[镜头时长] 2s　|　[景别] ECU

[主体与动作]
Extreme close-up of the smartphone screen showing WeChat transfer page with the amount "￥10.00" in large green numerals, a confirm button highlighted, a male fingertip pressing down.
- 情绪转变：稍作迟疑 → 点击落定 → 等待结果
- 微表情序列：0–0.7s 稍作迟疑；0.7–1.3s 点击落定；1.3–2.0s 等待结果
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：微小 · 果决 · 下注
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up top-down, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：手机屏幕乱码 / 微信图标错位 / 中文字符崩坏
```

### S05-04b　CU·婷婷手机收款震惊
**引用素材**：`[CHAR-TT]` `[EXP-SHOCK]` `[PROP-PHONE-RECEIVE]`

```
[镜头编号] S05-04b　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up of a girl's hand with chipped black nail polish holding a slightly-cracked-screen smartphone displaying WeChat notification "微信支付：到账 10.00 元", the red-haired girl's face partially visible above, frozen in shock.
- 情绪转变：常态 → 瞳孔骤张 → 凝固呆愣
- 微表情序列：0–0.7s 常态；0.7–1.3s 瞳孔骤张；1.3–2.0s 凝固呆愣
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：不可置信
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸 / 手机屏幕乱码 / 微信图标错位 / 中文字符崩坏
```

### S05-04c　MS·三女转为感激
**引用素材**：`[CHAR-TT]` `[EXP-GRATEFUL]` `[CHAR-JX]` `[EXP-GRATEFUL]` `[CHAR-XS]` `[EXP-GRATEFUL]`

```
[镜头编号] S05-04c　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
Medium shot of the three girls slowly lifting their heads from the phone, eyes transitioning from shock to deep grateful softness, the yellow-haired one's eyes welling up, the red-haired one's lips trembling, the purple-haired one's cold smirk softening.
- 情绪转变：错愕 → 眼眶发烫 → 唇线颤抖
- 微表情序列：0–1.0s 错愕；1.0–2.0s 眼眶发烫；2.0–3.0s 唇线颤抖
- 动作强度 motion intensity：5/10　中速推进（强调聚焦）

[环境与氛围]
氛围关键词：质朴 · 善意 · 意外
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC with gentle PUSH-IN, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-05a　CU·白离脑海面板返利
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-EXCITED]` `[PROP-PANEL-REWARD]`

```
[镜头编号] S05-05a　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the executive man with a barely-contained excited smile, a semi-transparent cyan-blue holographic reward panel overlaying part of the frame: "投资目标：陈婷婷 / 情绪波动：感激涕零 / 触发 10 倍暴击返利！/ 获得返利：￥100", with a golden burst icon.
- 情绪转变：克制蓄势 → 内火点燃 → 隐忍上扬
- 微表情序列：0–1.0s 克制蓄势；1.0–2.0s 内火点燃；2.0–3.0s 隐忍上扬
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：验证爽感 · 爽点
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：UI 文字乱码 / UI 元素崩坏 / 蓝色光晕过曝 / panel 双重叠影 / 换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S05-05b　ECU·手机银行短信
**引用素材**：`[PROP-PHONE-BANK-SMS]`

```
[镜头编号] S05-05b　|　[镜头时长] 2s　|　[景别] ECU

[主体与动作]
Extreme close-up of the executive man's smartphone screen displaying a bank SMS banner: "【XX 银行】您尾号 8868 的储蓄卡账户收入 100.00 元，当前余额 300,100.00 元。"
- 情绪转变：将信将疑 → 数字撞入眼 → 真实感冲顶
- 微表情序列：0–0.7s 将信将疑；0.7–1.3s 数字撞入眼；1.3–2.0s 真实感冲顶
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：电影感 · 半写实漫剧
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up top-down, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：手机屏幕乱码 / 微信图标错位 / 中文字符崩坏
```

### S05-05c　CU·白离嘴角扬起
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SMIRK]` `[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` 背影

```
[镜头编号] S05-05c　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the executive man's face, subtle satisfied smirk at mouth corner, eyes glinting, soft fluorescent light; out-of-focus in background are three spicy girls' backs running off happily.
- 情绪转变：中性 → 嘴角悄起 → 眼神发亮
- 微表情序列：0–1.0s 中性；1.0–2.0s 嘴角悄起；2.0–3.0s 眼神发亮
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：掠夺
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 6 场 · 分食泡面·烟搭桥

### S06-01a　MCU·热水倒入袋装泡面
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-INSTANT-NOODLE-BAG]` `[SCN-REST-AREA-EXT-NIGHT]`

```
[镜头编号] S06-01a　|　[镜头时长] 4s　|　[景别] MCU

[主体与动作]
Top-down medium close-up of the three girls squatting together outside the convenience store at night, hot water being poured from a kettle into a flat bag-style cheap instant noodle packaging held open by the red-haired girl's hands, steam rising, fingers gingerly avoiding the heat.
- 情绪转变：蹲下围拢 → 倒水入袋 → 满足互看
- 微表情序列：0–1.3s 蹲下围拢；1.3–2.7s 倒水入袋；2.7–4.0s 满足互看
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：江湖气 · 霓虹+冷蓝 / 热水蒸汽
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-EXT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up top-down, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S06-01b　CU·三头分食一双筷子
**引用素材**：`[CHAR-TT]` `[EXP-CONTENT]` `[CHAR-JX]` `[EXP-CONTENT]` `[CHAR-XS]` `[EXP-CONTENT]` `[PROP-CHOPSTICKS]` `[PROP-INSTANT-NOODLE-BAG]`

```
[镜头编号] S06-01b　|　[镜头时长] 4s　|　[景别] CU

[主体与动作]
Close-up of three heads leaning in around a single bag of cheap instant noodles, sharing one pair of split disposable wooden chopsticks, each girl taking turns eating, soft contented smiles, warm neon-orange ambient light.
- 情绪转变：小心翼翼 → 享受 → 满足闭眼
- 微表情序列：0–1.3s 小心翼翼；1.3–2.7s 享受；2.7–4.0s 满足闭眼
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：温柔
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up slight overhead, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S06-01c　MS·收拾垃圾扔垃圾桶
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-TRASH]` `[SCN-REST-AREA-EXT-NIGHT]`

```
[镜头编号] S06-01c　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
The three girls tying a small white plastic bag of trash and dropping it into a green public trash bin, brushing their hands clean.
- 情绪转变：随手收拢垃圾 → 起身投入桶 → 拍手撇清
- 微表情序列：0–1.0s 随手收拢垃圾；1.0–2.0s 起身投入桶；2.0–3.0s 拍手撇清
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：意外 · 懂事 · 霓虹+冷蓝 / 热水蒸汽
（场景与光照参见 [全局视觉锁定] 中 SCN-REST-AREA-EXT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S06-02a　MS·婷婷递南京梦都
**引用素材**：`[CHAR-TT]` `[EXP-FRIENDLY]` `[PROP-CIGARETTE-NJ]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S06-02a　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
Back in the coach at night with warm amber overhead reading lights, the red-haired girl pulling a single "南京 梦都" cigarette from a light-blue soft pack she retrieved from her black stocking edge, extending it toward the executive man with a lopsided friendly grin.
- 情绪转变：试探 → 真心咧嘴 → 递烟示好
- 微表情序列：0–1.0s 试探；1.0–2.0s 真心咧嘴；2.0–3.0s 递烟示好
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：暖意 · 羁绊 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot side angle, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸 / 烟支变形 / 烟头双火 / 香烟品牌错字
```

### S06-02b　MCU·白离掏雨花石回敬
**引用素材**：`[CHAR-BL-CASUAL]` `[PROP-CIGARETTE-YHS]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S06-02b　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
The same executive man now with his trench coat removed, wearing his dark-charcoal vest over white shirt with sleeves rolled to forearm, tie loosened, shaking his head with a faint smile, taking out his own soft-pack of dark-green "雨花石" cigarettes, pinching one between his lips, and handing the pack toward the girls.
- 情绪转变：微微一笑 → 自掏好烟 → 不动声色递出
- 微表情序列：0–1.0s 微微一笑；1.0–2.0s 自掏好烟；2.0–3.0s 不动声色递出
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸 / 烟支变形 / 烟头双火 / 香烟品牌错字
```

### S06-02c　CU·三女眼亮
**引用素材**：`[CHAR-TT]` `[EXP-WOW]` `[CHAR-JX]` `[EXP-WOW]` `[CHAR-XS]` `[EXP-WOW]`

```
[镜头编号] S06-02c　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the three girls' faces packed in frame, eyes widening simultaneously in amazed exclamation at the sight of the "雨花石" pack, mouths in O-shapes, the warm amber light glowing on their cheeks.
- 情绪转变：愣神 → 瞳孔放大 → O 形惊呼
- 微表情序列：0–1.0s 愣神；1.0–2.0s 瞳孔放大；2.0–3.0s O 形惊呼
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：艳羡
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S06-03　MS·三女抽烟满足
**引用素材**：`[CHAR-TT]` `[EXP-CONTENT]` `[CHAR-JX]` `[EXP-CONTENT]` `[CHAR-XS]` `[EXP-CONTENT]` `[PROP-CIGARETTE-YHS]` `[FX-SMOKE]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S06-03　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
Medium shot of the three girls each holding a lit "雨花石" cigarette, each taking a deep first drag with eyes closed in satisfaction, soft volumetric smoke wisps drifting in warm amber coach light.
- 情绪转变：小心翼翼 → 享受 → 满足闭眼
- 微表情序列：0–1.3s 小心翼翼；1.3–2.7s 享受；2.7–4.0s 满足闭眼
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：惬意 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, slow PUSH-IN, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸 / 烟支变形 / 烟头双火 / 香烟品牌错字
```

---

## 第 7 场 · 胖子挑衅·三妹护主

### S07-01a　MS·胖子站过道扫视
**引用素材**：`[CHAR-FATTY]` `[EXP-LEER]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S07-01a　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
A greasy overweight 40-year-old Chinese man with thick gold chain necklace, big belly straining a cream-yellow polo shirt, standing in the aisle of the coach at night, leering smirk, narrow eyes scanning the three girls up and down.
- 情绪转变：中性 → 色眯眯扫视 → 嘬牙坏笑
- 微表情序列：0–1.3s 中性；1.3–2.7s 色眯眯扫视；2.7–4.0s 嘬牙坏笑
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：掠夺 · 猎手 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot from coach back-row perspective, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-01b　ECU·白离冷眼
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-COLD-KILL]`

```
[镜头编号] S07-01b　|　[镜头时长] 2s　|　[景别] ECU

[主体与动作]
Extreme close-up of the executive man's eyes, ice-cold killing intent, narrow gaze, jaw tightened, faint shadow over the upper half of his face under amber light.
- 情绪转变：冷静 → 杀机渗入 → 下颌紧锁
- 微表情序列：0–0.7s 冷静；0.7–1.3s 杀机渗入；1.3–2.0s 下颌紧锁
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：威胁 · 静默
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：extreme close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-02a　MCU·婷婷暴起骂人
**引用素材**：`[CHAR-TT]` `[EXP-FURIOUS]` `[CHAR-FATTY]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S07-02a　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
The red-haired girl springing up to her feet, finger jabbing forward toward the fat man's nose, mouth wide open mid-curse, brows furrowed, tattooed arm tense, eyes blazing.
- 情绪转变：炸毛 → 狂喷 → 余势汹汹
- 微表情序列：0–1.0s 炸毛；1.0–2.0s 狂喷；2.0–3.0s 余势汹汹
- 动作强度 motion intensity：6/10　快速推进（戏剧爆点）

[环境与氛围]
氛围关键词：江湖气 · 街头 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, fast PUSH-IN, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-02b　MCU·小双跟团
**引用素材**：`[CHAR-XS]` `[EXP-FOLLOWUP]`

```
[镜头编号] S07-02b　|　[镜头时长] 2s　|　[景别] MCU

[主体与动作]
The yellow-haired girl trying to look fierce alongside the red-haired girl, brows pushed down, mouth pursed in mimicked toughness, half-comical determination.
- 情绪转变：紧张 → 鼓气模仿 → 强撑凶相
- 微表情序列：0–0.7s 紧张；0.7–1.3s 鼓气模仿；1.3–2.0s 强撑凶相
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：电影感 · 半写实漫剧
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-02c　MCU·佳欣冷脸收腿
**引用素材**：`[CHAR-JX]` `[EXP-ICY]`

```
[镜头编号] S07-02c　|　[镜头时长] 2s　|　[景别] MCU

[主体与动作]
The purple-haired girl coldly pulling her crossed leg back down off the seat, narrow eyes locked on the fat man, lips pressed flat, chin tilted in contempt.
- 情绪转变：冷淡 → 凝视锁定 → 唇线压平
- 微表情序列：0–0.7s 冷淡；0.7–1.3s 凝视锁定；1.3–2.0s 唇线压平
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：威压 · 冰冷
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-03a　MS·婷婷抬小双腿欲脱鞋
**引用素材**：`[CHAR-TT]` `[EXP-WILD]` `[CHAR-XS]` `[PROP-CARTOON-SOCKS]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S07-03a　|　[镜头时长] 3s　|　[景别] MS

[主体与动作]
The red-haired girl with a wild manic grin stepping forward and lifting one of the yellow-haired girl's legs, hand poised to yank off her white cartoon-strawberry-bear knee-high sock, the yellow-haired girl half-laughing in surprise.
- 情绪转变：蓄势 → 疯狂笑出 → 上前压制
- 微表情序列：0–1.0s 蓄势；1.0–2.0s 疯狂笑出；2.0–3.0s 上前压制
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：紧张 · 荒诞 · 战术 · 威慑 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-03b　MCU·胖子骤然怂
**引用素材**：`[CHAR-FATTY]` `[EXP-SCARED]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S07-03b　|　[镜头时长] 2s　|　[景别] MCU

[主体与动作]
Reverse-angle medium close-up of the fat man's face deflating into cowardly fear, eyes flicking aside, lips pressed, leaning back as he retreats toward his seat.
- 情绪转变：嚣张 → 一瞬泄气 → 缩脖后退
- 微表情序列：0–0.7s 嚣张；0.7–1.3s 一瞬泄气；1.3–2.0s 缩脖后退
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：泄气 · 霸凌 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up reverse, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S07-03c　CU·白离复杂注视
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-REFLECT]`

```
[镜头编号] S07-03c　|　[镜头时长] 3s　|　[景别] CU

[主体与动作]
Close-up of the executive man's face, expression thoughtful and softened, eyes briefly catching warm light, faint inward smile, complex reflection in his pupils.
- 情绪转变：冷淡 → 触动 → 内省微笑
- 微表情序列：0–1.0s 冷淡；1.0–2.0s 触动；2.0–3.0s 内省微笑
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：心境转变
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

---

## 第 8 场 · 老乡相认·夜窗盘算

### S08-01a　MCU·小双拉回话题
**引用素材**：`[CHAR-XS]` `[EXP-CURIOUS]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S08-01a　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
The yellow-haired girl tilting her head with big curious eyes, soft smile, leaning slightly toward the executive man, warm amber reading light.
- 情绪转变：安静 → 歪头发问 → 期待眨眼
- 微表情序列：0–1.0s 安静；1.0–2.0s 歪头发问；2.0–3.0s 期待眨眼
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：暖意 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S08-01b　CU·白离淡淡平县
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-CALM]`

```
[镜头编号] S08-01b　|　[镜头时长] 2s　|　[景别] CU

[主体与动作]
Close-up reverse-angle of the executive man, composed neutral expression, slight controlled smile, soft amber light on his profile.
- 情绪转变：中性 → 微微上扬 → 控制式微笑
- 微表情序列：0–0.7s 中性；0.7–1.3s 微微上扬；1.3–2.0s 控制式微笑
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：少量 · 透露
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：close-up reverse, STATIC, 2 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S08-01c　MS·三女惊呼老乡
**引用素材**：`[CHAR-TT]` `[EXP-EXCITED]` `[CHAR-JX]` `[EXP-EXCITED]` `[CHAR-XS]` `[EXP-EXCITED]` `[PROP-CARTOON-SOCKS]` `[SCN-BUS-INT-NIGHT]`

```
[镜头编号] S08-01c　|　[镜头时长] 4s　|　[景别] MS

[主体与动作]
Medium shot of the three girls erupting in excited delight, the yellow-haired one slipping off her white sneakers and pulling her legs up onto the seat in a curled-up pose revealing the cartoon strawberry-bear print on her knee-high socks, the other two bouncing in their seats.
- 情绪转变：克制蓄势 → 内火点燃 → 隐忍上扬
- 微表情序列：0–1.3s 克制蓄势；1.3–2.7s 内火点燃；2.7–4.0s 隐忍上扬
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：老乡 · 奇迹 · 暖灯夜车厢 / 烟雾微粒
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-INT-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot, STATIC, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S08-01d　MCU·白离不着痕迹瞥
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-GLANCE]`

```
[镜头编号] S08-01d　|　[镜头时长] 3s　|　[景别] MCU

[主体与动作]
Medium close-up of the executive man, eyes briefly shifting to the side then averting, otherwise neutral composed face, soft amber light.
- 情绪转变：中性 → 余光斜扫 → 收回掩饰
- 微表情序列：0–1.0s 中性；1.0–2.0s 余光斜扫；2.0–3.0s 收回掩饰
- 动作强度 motion intensity：1/10　极静（纯静帧）

[环境与氛围]
氛围关键词：不动声色 · 盘算
（场景与光照参见 [全局视觉锁定] 中 当前镜头所属场景 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium close-up, STATIC, 3 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S08-02a　MS·白离靠窗盘算
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-SCHEME]` `[SCN-BUS-WINDOW-NIGHT]`

```
[镜头编号] S08-02a　|　[镜头时长] 5s　|　[景别] MS

[主体与动作]
Medium shot of the executive man leaning against the coach window at night, scenery streaming backwards outside as bokeh streaks of orange and white light, faint reflection of his thoughtful face overlaid on the glass, leaning chin on hand, faint cunning smile.
- 情绪转变：若有所思 → 计谋成形 → 阴翳浅笑
- 微表情序列：0–1.7s 若有所思；1.7–3.3s 计谋成形；3.3–5.0s 阴翳浅笑
- 动作强度 motion intensity：3/10　缓慢推/拉/移（影视常规）

[环境与氛围]
氛围关键词：野心 · 车窗夜景 / 光斑流过
（场景与光照参见 [全局视觉锁定] 中 SCN-BUS-WINDOW-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：medium shot side, slow DOLLY-OUT, 5 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：换发色 / 纹身样式漂移 / 服装漂移 / 多人融脸
```

### S08-02b　EWS·大巴夜行远去
**引用素材**：`[SCN-HIGHWAY-NIGHT]`

```
[镜头编号] S08-02b　|　[镜头时长] 4s　|　[景别] EWS

[主体与动作]
Aerial high-angle shot of a single white long-distance coach driving away on a dark Chinese expressway at night, two long red tail-light streaks trailing behind, scattered orange sodium street lamps, deep blue-black sky, faint distant city glow on horizon.
- 情绪转变：车灯远去 → 夜路延展 → 未完续航
- 微表情序列：0–1.3s 车灯远去；1.3–2.7s 夜路延展；2.7–4.0s 未完续航
- 动作强度 motion intensity：3/10　缓慢航拍（俯瞰节奏）

[环境与氛围]
氛围关键词：旅途 · 未完待续 · 深夜高速 / 红尾灯条
（场景与光照参见 [全局视觉锁定] 中 SCN-HIGHWAY-NIGHT 锁定段，本镜不重复描述以避免漂移。）

[镜头运动]
Camera：drone high-angle, slow upward ASCENT with slight backward TRACK, 4 seconds.

[负面约束]
--no （继承 [全局视觉锁定] 全局禁止项）+ 本镜追加：画面元素漂移 / 与首帧不符
```

---

## 附：Kling 操作模板

```
画面：粘贴上面对应镜号的 prompt
首帧参考图：上传 04 号文档对应关键帧生成的图
镜头时长：5 秒
画质：高
画面比例：16:9
负向：deformed faces, wrong tattoo, color drift, extra fingers, mismatched outfit, NSFW exposure, low quality, text artifacts, watermark
```
