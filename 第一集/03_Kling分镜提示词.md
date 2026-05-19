# 第一集 · Kling 3.0 分镜提示词文档（Shot Prompts）

> 用途：每个主镜头 / 子镜头一段可直接复制粘贴到 Kling 3.0 的视频生成提示词。  
> 规则：① 顶部统一 STYLE PREFIX；② 标注引用的素材 ID（指向 `02_美术资产提示词.md`）；③ 不包含剪辑/旁白文案；④ 镜头时长 ≤5s 单段；⑤ 优先采用 PUSH/PULL/PAN/TILT/TRACK/STATIC 等 Kling 稳定运镜。  
> 操作流程：先用 `04_关键帧提示词.md` 生成首帧 → 把首帧上传作为参考图 → 在 Kling 中粘贴本镜头 prompt → 选 5s / 高质量 → 生成。

---

## 〇、STYLE PREFIX（每个 Prompt 都已内嵌，可整体复制）

```
Style: cinematic semi-realistic Chinese urban manhua, ultra-detailed faces with consistent character design, soft volumetric light, shallow depth of field, film grain, 8k photoreal, 16:9.
Consistency: characters and props strictly follow the referenced asset IDs; do not alter hair color, clothing, tattoos or facial features.
```

---

## 第 1 场 · 春运启程·客运站

### S01-01a　EWS·客运站广场全景  
**引用素材**：`[SCN-STATION-DAY]` `[CHAR-DRIVER]`(远景群演) `[PROP-MEGAPHONE]`
```
[Style+Consistency prefix]
A wide aerial high-angle establishing shot of a North-China long-distance bus terminal plaza during Spring Festival travel rush, vast crowd of travelers dragging rolling luggage and red-blue striped woven bags, large red "春运" banner across upper frame, multiple parked white long-distance coaches, grey overcast winter sky at 11AM, slightly damp concrete pavement, breath visible in cold air.
Camera: high-angle establishing, slow PUSH-IN forward, 5 seconds, steady.
Mood: bleak weary holiday rush.
```

### S01-01b　MLS·售票口司机喊话  
**引用素材**：`[CHAR-DRIVER]` `[PROP-MEGAPHONE]` `[SCN-STATION-DAY]`
```
[Style+Consistency prefix]
A 45-year-old Chinese long-distance bus driver in a dark navy quilted cotton coat and black "运" cap, weather-tanned face, holding a red plastic megaphone close to his mouth, shouting loudly at the crowd, foreground passengers passing through soft-focus, ticket gate signage in background, grey daylight.
Camera: medium long shot, STATIC tripod, slight foreground-passenger walk-by parallax, 3 seconds.
Mood: noisy chaotic terminal.
```

### S01-02a　MS·白离拖箱穿人群  
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-LUGGAGE]` `[SCN-STATION-DAY]`
```
[Style+Consistency prefix]
A 26-year-old handsome Chinese man with peach-blossom almond eyes, side-parted black hair, wearing a dark-charcoal three-piece suit under a beige knee-length trench coat draped over his shoulders, polished black oxford shoes, pulling a 28-inch brushed silver aluminum spinner luggage with his left hand, his back partly to camera as he walks through a thick crowd toward a coach.
Camera: medium shot, smooth TRACK behind him at walking pace, slight over-shoulder, 4 seconds.
Mood: lonely fatigue in crowd.
```

### S01-02b　CU·行李箱滚轮压地砖  
**引用素材**：`[PROP-LUGGAGE]` `[SCN-STATION-DAY]`
```
[Style+Consistency prefix]
Extreme low-angle close-up of four spinner wheels of a brushed silver aluminum luggage rolling across slightly damp grey concrete tiles, tiny water droplets splashing, mirror-faint reflection of wheels on wet ground.
Camera: ground-level close-up, STATIC, slight forward motion of wheels, 2 seconds.
Mood: travel-weary detail.
```

### S01-03　MLS·白离登车回望天空  
**引用素材**：`[CHAR-BL-FORMAL]` `[SCN-BUS-EXT-DAY]` `[PROP-LUGGAGE]`
```
[Style+Consistency prefix]
The same 26-year-old executive man steps onto the metal step of a white Chinese long-distance coach with license plate "沪 A·B8868" and route card "魔都→运市", trench coat over shoulders, luggage in hand, pausing for a beat to glance up at the grey overcast sky, breath fogging in cold air.
Camera: medium long shot from front-side, slow DOLLY-IN, 4 seconds.
Mood: resigned departure.
```

---

## 第 2 场 · 大巴最后排·三女登场

### S02-01a　MLS·车厢内最后排空位  
**引用素材**：`[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
Interior of a Chinese long-distance coach in daytime, double rows of dark-burgundy velvet seats with cream headrest covers, most seats occupied by various Chinese passengers, the rear three-seat row at center frame empty and lit by a soft side-window beam.
Camera: medium long shot from front of aisle, slow DOLLY-IN toward the back row, 5 seconds.
Mood: anticipation of a long ride.
```

### S02-01b　MS·白离落座靠窗  
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-LUGGAGE]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
The same 26-year-old executive man lifts a silver luggage onto the overhead aluminum rack, then settles into the leftmost window seat of the back row, smoothing his trench coat, eyes lowering.
Camera: medium shot at 3/4 front angle, smooth TRACK following his sit-down motion, 3 seconds.
Mood: relief tinged with weariness.
```

### S02-02　CU·白离闭眼后仰  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-TIRED]` `[PROP-EARPHONE]`
```
[Style+Consistency prefix]
Close-up of the same executive man's face, expression weary with heavy half-closed eyelids, slight frown, head leaning back against the cream headrest cover, black in-ear earphone cable visible at his collar, soft window daylight on his profile.
Camera: close-up, side 45°, STATIC, 3 seconds.
Mood: bone-deep tiredness.
```

### S02-03a　MLS·三精神小妹挤上车  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
Three loud "spicy girls" squeezing onto the coach at the front door: a 22-year-old with shoulder-length fire-red wavy hair, smoky eyes, multicolor Prajna half-sleeve tattoo on left arm, cropped black faux-leather jacket and short denim; a 21-year-old with lavender-purple straight hair, off-shoulder black crop top, ultra-short denim shorts, sheer ultra-thin slightly translucent black stockings (lightweight 15-denier matte-sheer, no fishnet, no rips); a 19-year-old with honey-yellow wavy hair in pink claw clip, pastel pink puffer crop, white knee-high cartoon-bear socks. They jostle and chatter loudly.
Camera: medium long shot at door perspective, quick PUSH-IN with very subtle handheld micro-shake, 3 seconds.
Mood: chaotic invasion of energy.
```

### S02-03b　CU·白离猛睁眼侧目  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-ANNOYED]`
```
[Style+Consistency prefix]
Close-up of the executive man, eyes snapped open and sharply side-glancing toward the front door, eyebrows tightly knit, mouth a flat line.
Camera: close-up, STATIC, 2 seconds.
Mood: intrusive disturbance.
```

### S02-04a　MS·三女沿过道走来  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
The three spicy girls walking down the aisle of the coach, the yellow-haired girl in the lead pointing toward the empty back row with an excited expression, the red-haired one swaggering behind, the purple-haired one rolling eyes.
Camera: medium shot tracking PAN with slight PUSH-IN from rear of coach, 4 seconds.
Mood: incoming trouble.
```

### S02-04b　MS·白离 POV 三女扑面  
**引用素材**：`[CHAR-BL-FORMAL]` POV，`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
First-person POV from the executive man's seat at the back row: the three spicy girls walking straight toward camera, getting closer, slightly low angle, soft daytime side-window light.
Camera: POV medium shot, STATIC with subtle natural breathing micro-shake, 3 seconds.
Mood: dread of contact.
```

### S02-05a　MS·三人入坐最后排  
**引用素材**：`[CHAR-BL-FORMAL]` `[CHAR-XS]` `[CHAR-JX]` `[CHAR-TT]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
The back row of the coach now packed: from left to right - the executive man pressed against the window, the yellow-haired soft-faced 19-year-old plopping down right next to him, then the purple-haired 21-year-old, then the red-haired 22-year-old with tattooed arm, all jostling for space, seats creaking.
Camera: medium shot front-on, STATIC, 4 seconds.
Mood: forced intimacy of strangers.
```

### S02-05b　CU·拥挤大腿暗示  
**引用素材**：`[CHAR-BL-FORMAL]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
Close-up TILT-DOWN of the gap between two seated passengers: a man's charcoal-suit trouser leg and a young girl's bare thigh in light denim shorts pressed lightly side by side from the squeeze, no skin exposed beyond shorts hemline, tasteful framing, focus on the fabric contrast.
Camera: close-up, TILT-DOWN, STATIC, 3 seconds.
Mood: discomfort from forced proximity.
```

### S02-05c　MS·婷婷骂厂子佳欣附和  
**引用素材**：`[CHAR-TT]` `[EXP-ANGRY]` `[CHAR-JX]` `[EXP-ATTITUDE]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
The red-haired girl mid-rant with mouth wide open in fury, brows furrowed, finger jabbing the air; the purple-haired girl beside her nodding with cold smirk and chin lifted; surrounding passengers (out of focus) turning displeased glances toward them.
Camera: medium shot, STATIC, 4 seconds.
Mood: loud disrespectful energy.
```

---

## 第 3 场 · 一瓶水·系统降临

### S03-01a　EWS·高速公路空镜  
**引用素材**：`[SCN-HIGHWAY-DUSK]`
```
[Style+Consistency prefix]
Aerial side-tracking shot of a single white Chinese long-distance coach driving on an empty expressway at dusk, sky gradient deep blue to faint orange, wet asphalt reflecting sky, distant fields and pylons.
Camera: drone-style smooth side TRACK matching coach speed, 3 seconds.
Mood: solitary travel.
```

### S03-01b　CU·小双脸色发白晕车  
**引用素材**：`[CHAR-XS]` `[EXP-CARSICK]`
```
[Style+Consistency prefix]
Close-up of the 19-year-old soft-faced girl with honey-yellow wavy hair and pink claw clip, expression motion-sick with pale slightly-green-tinted face, hand covering her mouth, watery eyes, soft warm coach interior light on her profile.
Camera: close-up, STATIC, 3 seconds.
Mood: vulnerable nausea.
```

### S03-02a　MCU·小双怯生生请求喝水  
**引用素材**：`[CHAR-XS]` `[EXP-PLEADING]` `[CHAR-BL-FORMAL]`
```
[Style+Consistency prefix]
The yellow-haired girl timidly leaning toward the executive man, fingertips lightly touching his suit sleeve, looking up with big watery doe eyes and slightly parted lips; the man's profile on the right edge of frame.
Camera: medium close-up at side 45°, STATIC, 3 seconds.
Mood: shy pleading.
```

### S03-02b　ECU·白离嘴角抽动  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-TWITCH]`
```
[Style+Consistency prefix]
Extreme close-up of the executive man's mouth area, a subtle single twitch at the corner of his lips, otherwise composed face, soft window light.
Camera: extreme close-up, STATIC, 1.5 seconds.
Mood: silent internal protest.
```

### S03-02c　CU·水瓶手边  
**引用素材**：`[PROP-WATER-USED]`
```
[Style+Consistency prefix]
Close-up low-angle top-down of a 550ml clear mineral water bottle with blue-white "纯净水" label, water level about 80%, cap on, resting on a charcoal suit trouser leg next to a man's hand.
Camera: close-up top-down, STATIC, 2 seconds.
Mood: small object holding decision.
```

### S03-03a　MCU·白离冷淡拒绝  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-COLD]`
```
[Style+Consistency prefix]
The executive man's face in medium close-up, expression cold and detached, lips a flat line, eyes calm and dismissive, soft side-window light.
Camera: medium close-up, STATIC, 3 seconds.
Mood: aloof refusal.
```

### S03-03b　MS·小双拿水瓶  
**引用素材**：`[CHAR-XS]` `[EXP-BRIGHT]` `[PROP-WATER-USED]`
```
[Style+Consistency prefix]
The yellow-haired girl's eyes lighting up with hope and faint smile, hand reaching out and confidently taking the mineral water bottle from the man's side, very natural motion.
Camera: medium shot 3/4 front angle, STATIC, 3 seconds.
Mood: bright unfiltered enthusiasm.
```

### S03-03c　CU·小双仰头喝水  
**引用素材**：`[CHAR-XS]` `[EXP-DRINK]` `[PROP-WATER-USED]`
```
[Style+Consistency prefix]
Close-up side profile of the yellow-haired girl tilting her head back, eyes closed, throat visibly swallowing as she chugs from the open mineral water bottle, soft strand of hair falling.
Camera: close-up side, STATIC, 3 seconds.
Mood: thirsty relief.
```

### S03-03d　CU·水瓶口唇印特写  
**引用素材**：`[PROP-WATER-LIPMARK]`
```
[Style+Consistency prefix]
Close-up of the same mineral water bottle, water level now reduced to about 30%, a faint pale-pink glossy lip print smudge visible around the bottle opening, condensation droplets on surface, bottle being handed back into a man's hand entering frame.
Camera: close-up, STATIC, 2 seconds.
Mood: lingering trace.
```

### S03-04a　MCU·白离嫌弃送水  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-DISGUST]`
```
[Style+Consistency prefix]
Medium close-up of the executive man, faint disgusted expression with lips slightly curled, waving his free hand dismissively as if to say "keep it".
Camera: medium close-up, STATIC, 2 seconds.
Mood: mild aversion.
```

### S03-04b　CU·小双低头攥瓶子  
**引用素材**：`[CHAR-XS]` `[EXP-SHY-THANKFUL]` `[PROP-WATER-LIPMARK]`
```
[Style+Consistency prefix]
Close-up of the yellow-haired girl with head lowered, faint blush on her cheeks, hands clutching the half-empty water bottle tightly to her chest, soft warm light.
Camera: close-up, STATIC, 3 seconds.
Mood: tender unexpected gratitude.
```

### S03-04c　ECU·白离瞳孔系统绑定  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SHOCK]` `[FX-SYS-BIND]`
```
[Style+Consistency prefix]
Extreme close-up of one eye of the executive man, dark-brown iris filling the frame, cyan-blue holographic Chinese characters and a 0-100% progress bar reflected on the wet surface of the eye, faint sci-fi scanlines and particle dust, pupil dilating with shock.
Camera: extreme close-up, STATIC with slight ZOOM-IN, 4 seconds.
Mood: cosmic awakening.
```

---

## 第 4 场 · 系统面板·女神雷达

### S04-01a　MS·蓝色面板悬浮  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SHOCK]` `[PROP-PANEL-MAIN]`
```
[Style+Consistency prefix]
The executive man sitting in the coach back row, eyes fully wide and lips slightly parted in shock; a semi-transparent cyan-blue holographic UI panel floats in front of his face, displaying clean Chinese sci-fi typography: "宿主：白离 / 系统：女神投资系统 / 功能：女神雷达、投资返利". Panel softly rotated 5°, glowing edges, particle dust around.
Camera: medium shot front-on, STATIC, 4 seconds.
Mood: stunned wonder.
```

### S04-01b　CU·手指穿过面板  
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-PANEL-MAIN]`
```
[Style+Consistency prefix]
Close-up of the executive man's hand reaching forward, his index finger passing straight through the semi-transparent cyan-blue holographic panel without resistance, faint cyan glow on his fingertip.
Camera: close-up side, STATIC, 3 seconds.
Mood: testing the impossible.
```

### S04-01c　MCU·乘客毫无反应  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-BUS-INT-DAY]`
```
[Style+Consistency prefix]
Reverse-angle medium close-up of the three spicy girls and nearby passengers in the coach, all chatting or scrolling phones, none of them noticing or reacting to anything special, neutral daytime light.
Camera: medium close-up reverse angle, STATIC, 3 seconds.
Mood: invisible only to him.
```

### S04-02a　CU·系统功能介绍面板  
**引用素材**：`[PROP-PANEL-FUNC]`
```
[Style+Consistency prefix]
Close-up of a semi-transparent cyan-blue holographic UI panel hovering against a dark blurred background, sharp Chinese sci-fi typography listing "功能一：女神雷达" and "功能二：投资返利" and "倾心值：0 路人 / 60 爱慕 / 80 热恋 / 100 至死不渝", glowing edges, particle dust.
Camera: close-up, STATIC with very slight ZOOM-IN, 4 seconds.
Mood: rule revelation.
```

### S04-02b　MS·白离 POV 扫描三女  
**引用素材**：`[CHAR-BL-FORMAL]` POV，`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-PANEL-RADAR]`
```
[Style+Consistency prefix]
First-person POV from the executive man: gaze sweeping across the three spicy girls in the back row, small cyan-blue holographic name tags popping up above each girl's head in sequence: "陈婷婷 倾心值 0 路人", "李佳欣 倾心值 0 路人", "林小双 倾心值 +10 略有好感"; scanner-like cyan grid sweep visual effect.
Camera: POV medium shot, smooth PAN left to right, 5 seconds.
Mood: god-mode unlock.
```

### S04-02c　ECU·白离贪婪眼神  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-GREEDY]`
```
[Style+Consistency prefix]
Extreme close-up of the executive man's eyes, blazing with fervent greedy excitement, faint upward smirk at lip corners, faint cyan reflection still in pupils.
Camera: extreme close-up, STATIC, 2 seconds.
Mood: predatory ambition.
```

---

## 第 5 场 · 服务区·十块钱投资

### S05-01a　LS·服务区夜景灯牌  
**引用素材**：`[SCN-REST-AREA-NIGHT]` `[PROP-NEON-SIGN]`
```
[Style+Consistency prefix]
A wide long shot of a Chinese highway service area at night, large orange-red neon sign "XX 服务区" glowing on the building, white long-distance coach parked in foreground, wet asphalt reflecting neon, scattered travelers, faint mist.
Camera: long shot, slow DOLLY-IN toward the building, 4 seconds.
Mood: pit-stop in the long night.
```

### S05-01b　MS·白离拎泡面出便利店  
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-INSTANT-NOODLE-CUP]` `[PROP-WATER-NEW]` `[SCN-REST-AREA-NIGHT]`
```
[Style+Consistency prefix]
The executive man walking out of the automatic glass doors of a brightly-lit convenience store, holding a red "康师傅 红烧牛肉面" instant noodle cup in one hand and an unopened 550ml mineral water bottle in the other, trench coat still on shoulders.
Camera: medium shot, smooth TRACK in front of him, 3 seconds.
Mood: brief comfort of food.
```

### S05-02a　MS·便利店内白离撕开泡面  
**引用素材**：`[CHAR-BL-FORMAL]` `[PROP-INSTANT-NOODLE-CUP]` `[SCN-REST-AREA-INT]`
```
[Style+Consistency prefix]
Inside the convenience store at a small standing eating counter, the executive man tearing open the foil lid of the red instant noodle cup, steam rising into his face, bright cool fluorescent light overhead.
Camera: medium shot 3/4 angle, STATIC, 3 seconds.
Mood: simple warmth.
```

### S05-02b　MS·三女徘徊盯食物  
**引用素材**：`[CHAR-TT]` `[EXP-HUNGRY]` `[CHAR-JX]` `[EXP-HUNGRY]` `[CHAR-XS]` `[EXP-HUNGRY]` `[SCN-REST-AREA-INT]`
```
[Style+Consistency prefix]
The three spicy girls lingering in the convenience store aisle, gazes locked hungrily on other customers' food, throats subtly swallowing, the red-haired one trying to look tough, the purple-haired one feigning indifference, the yellow-haired one openly longing.
Camera: medium shot, STATIC, 4 seconds.
Mood: embarrassed hunger.
```

### S05-03a　MCU·婷婷上前喊大哥  
**引用素材**：`[CHAR-TT]` `[EXP-AWKWARD]` `[SCN-REST-AREA-INT]`
```
[Style+Consistency prefix]
Medium close-up of the red-haired tattooed girl standing in front of the counter, arms crossed over her tattooed forearm in awkward bravado, eyes shifting nervously, mouth opening to speak.
Camera: medium close-up, STATIC, 3 seconds.
Mood: hesitant pride.
```

### S05-03b　MCU·白离拿手机扫码  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-CALM]` `[PROP-PHONE-WECHAT]`
```
[Style+Consistency prefix]
Medium close-up reverse angle of the executive man calmly pulling out a black smartphone, screen showing a WeChat receive-money QR code with avatar "白离", his face composed neutral.
Camera: medium close-up reverse, STATIC, 3 seconds.
Mood: unreadable calculation.
```

### S05-03c　MS·三女凑头商量  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[SCN-REST-AREA-INT]`
```
[Style+Consistency prefix]
The three girls huddled in a small circle, heads close together, whispering and gesturing, looking around to see if anyone is watching.
Camera: medium shot top-down slight angle, STATIC, 4 seconds.
Mood: secretive deliberation.
```

### S05-03d　CU·婷婷伸一根手指  
**引用素材**：`[CHAR-TT]` `[EXP-CAREFUL]`
```
[Style+Consistency prefix]
Close-up of the red-haired girl carefully and timidly raising one single index finger, lips bitten, big pleading eyes upward, faint hope in expression.
Camera: close-up, STATIC, 2 seconds.
Mood: trembling small ask.
```

### S05-04a　ECU·点击转账  
**引用素材**：`[PROP-PHONE-TRANSFER]`
```
[Style+Consistency prefix]
Extreme close-up of the smartphone screen showing WeChat transfer page with the amount "￥10.00" in large green numerals, a confirm button highlighted, a male fingertip pressing down.
Camera: extreme close-up top-down, STATIC, 2 seconds.
Mood: decisive small bet.
```

### S05-04b　CU·婷婷手机收款震惊  
**引用素材**：`[CHAR-TT]` `[EXP-SHOCK]` `[PROP-PHONE-RECEIVE]`
```
[Style+Consistency prefix]
Close-up of a girl's hand with chipped black nail polish holding a slightly-cracked-screen smartphone displaying WeChat notification "微信支付：到账 10.00 元", the red-haired girl's face partially visible above, frozen in shock.
Camera: close-up, STATIC, 2 seconds.
Mood: disbelief.
```

### S05-04c　MS·三女转为感激  
**引用素材**：`[CHAR-TT]` `[EXP-GRATEFUL]` `[CHAR-JX]` `[EXP-GRATEFUL]` `[CHAR-XS]` `[EXP-GRATEFUL]`
```
[Style+Consistency prefix]
Medium shot of the three girls slowly lifting their heads from the phone, eyes transitioning from shock to deep grateful softness, the yellow-haired one's eyes welling up, the red-haired one's lips trembling, the purple-haired one's cold smirk softening.
Camera: medium shot, STATIC with gentle PUSH-IN, 3 seconds.
Mood: simple unexpected kindness.
```

### S05-05a　CU·白离脑海面板返利  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-EXCITED]` `[PROP-PANEL-REWARD]`
```
[Style+Consistency prefix]
Close-up of the executive man with a barely-contained excited smile, a semi-transparent cyan-blue holographic reward panel overlaying part of the frame: "投资目标：陈婷婷 / 情绪波动：感激涕零 / 触发 10 倍暴击返利！/ 获得返利：￥100", with a golden burst icon.
Camera: close-up, STATIC, 3 seconds.
Mood: thrilling validation.
```

### S05-05b　ECU·手机银行短信  
**引用素材**：`[PROP-PHONE-BANK-SMS]`
```
[Style+Consistency prefix]
Extreme close-up of the executive man's smartphone screen displaying a bank SMS banner: "【XX 银行】您尾号 8868 的储蓄卡账户收入 100.00 元，当前余额 300,100.00 元。"
Camera: extreme close-up top-down, STATIC, 2 seconds.
Mood: it's real.
```

### S05-05c　CU·白离嘴角扬起  
**引用素材**：`[CHAR-BL-FORMAL]` `[EXP-SMIRK]` `[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` 背影
```
[Style+Consistency prefix]
Close-up of the executive man's face, subtle satisfied smirk at mouth corner, eyes glinting, soft fluorescent light; out-of-focus in background are three spicy girls' backs running off happily.
Camera: close-up, STATIC, 3 seconds.
Mood: predator's pleasure.
```

---

## 第 6 场 · 分食泡面·烟搭桥

### S06-01a　MCU·热水倒入袋装泡面  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-INSTANT-NOODLE-BAG]` `[SCN-REST-AREA-EXT-NIGHT]`
```
[Style+Consistency prefix]
Top-down medium close-up of the three girls squatting together outside the convenience store at night, hot water being poured from a kettle into a flat bag-style cheap instant noodle packaging held open by the red-haired girl's hands, steam rising, fingers gingerly avoiding the heat.
Camera: medium close-up top-down, STATIC, 4 seconds.
Mood: street-level resourcefulness.
```

### S06-01b　CU·三头分食一双筷子  
**引用素材**：`[CHAR-TT]` `[EXP-CONTENT]` `[CHAR-JX]` `[EXP-CONTENT]` `[CHAR-XS]` `[EXP-CONTENT]` `[PROP-CHOPSTICKS]` `[PROP-INSTANT-NOODLE-BAG]`
```
[Style+Consistency prefix]
Close-up of three heads leaning in around a single bag of cheap instant noodles, sharing one pair of split disposable wooden chopsticks, each girl taking turns eating, soft contented smiles, warm neon-orange ambient light.
Camera: close-up slight overhead, STATIC, 4 seconds.
Mood: tender shared meal.
```

### S06-01c　MS·收拾垃圾扔垃圾桶  
**引用素材**：`[CHAR-TT]` `[CHAR-JX]` `[CHAR-XS]` `[PROP-TRASH]` `[SCN-REST-AREA-EXT-NIGHT]`
```
[Style+Consistency prefix]
The three girls tying a small white plastic bag of trash and dropping it into a green public trash bin, brushing their hands clean.
Camera: medium shot, STATIC, 3 seconds.
Mood: unexpected manners.
```

### S06-02a　MS·婷婷递南京梦都  
**引用素材**：`[CHAR-TT]` `[EXP-FRIENDLY]` `[PROP-CIGARETTE-NJ]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
Back in the coach at night with warm amber overhead reading lights, the red-haired girl pulling a single "南京 梦都" cigarette from a light-blue soft pack she retrieved from her black stocking edge, extending it toward the executive man with a lopsided friendly grin.
Camera: medium shot side angle, STATIC, 3 seconds.
Mood: warming up bond.
```

### S06-02b　MCU·白离掏雨花石回敬  
**引用素材**：`[CHAR-BL-CASUAL]` `[PROP-CIGARETTE-YHS]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
The same executive man now with his trench coat removed, wearing his dark-charcoal vest over white shirt with sleeves rolled to forearm, tie loosened, shaking his head with a faint smile, taking out his own soft-pack of dark-green "雨花石" cigarettes, pinching one between his lips, and handing the pack toward the girls.
Camera: medium close-up, STATIC, 3 seconds.
Mood: quiet generosity.
```

### S06-02c　CU·三女眼亮  
**引用素材**：`[CHAR-TT]` `[EXP-WOW]` `[CHAR-JX]` `[EXP-WOW]` `[CHAR-XS]` `[EXP-WOW]`
```
[Style+Consistency prefix]
Close-up of the three girls' faces packed in frame, eyes widening simultaneously in amazed exclamation at the sight of the "雨花石" pack, mouths in O-shapes, the warm amber light glowing on their cheeks.
Camera: close-up, STATIC, 3 seconds.
Mood: stunned admiration.
```

### S06-03　MS·三女抽烟满足  
**引用素材**：`[CHAR-TT]` `[EXP-CONTENT]` `[CHAR-JX]` `[EXP-CONTENT]` `[CHAR-XS]` `[EXP-CONTENT]` `[PROP-CIGARETTE-YHS]` `[FX-SMOKE]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
Medium shot of the three girls each holding a lit "雨花石" cigarette, each taking a deep first drag with eyes closed in satisfaction, soft volumetric smoke wisps drifting in warm amber coach light.
Camera: medium shot, slow PUSH-IN, 4 seconds.
Mood: blissful exhale.
```

---

## 第 7 场 · 胖子挑衅·三妹护主

### S07-01a　MS·胖子站过道扫视  
**引用素材**：`[CHAR-FATTY]` `[EXP-LEER]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
A greasy overweight 40-year-old Chinese man with thick gold chain necklace, big belly straining a cream-yellow polo shirt, standing in the aisle of the coach at night, leering smirk, narrow eyes scanning the three girls up and down.
Camera: medium shot from coach back-row perspective, STATIC, 4 seconds.
Mood: predatory intrusion.
```

### S07-01b　ECU·白离冷眼  
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-COLD-KILL]`
```
[Style+Consistency prefix]
Extreme close-up of the executive man's eyes, ice-cold killing intent, narrow gaze, jaw tightened, faint shadow over the upper half of his face under amber light.
Camera: extreme close-up, STATIC, 2 seconds.
Mood: silent threat.
```

### S07-02a　MCU·婷婷暴起骂人  
**引用素材**：`[CHAR-TT]` `[EXP-FURIOUS]` `[CHAR-FATTY]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
The red-haired girl springing up to her feet, finger jabbing forward toward the fat man's nose, mouth wide open mid-curse, brows furrowed, tattooed arm tense, eyes blazing.
Camera: medium close-up, fast PUSH-IN, 3 seconds.
Mood: street-fighter explosion.
```

### S07-02b　MCU·小双跟团  
**引用素材**：`[CHAR-XS]` `[EXP-FOLLOWUP]`
```
[Style+Consistency prefix]
The yellow-haired girl trying to look fierce alongside the red-haired girl, brows pushed down, mouth pursed in mimicked toughness, half-comical determination.
Camera: medium close-up, STATIC, 2 seconds.
Mood: loyal follow-up.
```

### S07-02c　MCU·佳欣冷脸收腿  
**引用素材**：`[CHAR-JX]` `[EXP-ICY]`
```
[Style+Consistency prefix]
The purple-haired girl coldly pulling her crossed leg back down off the seat, narrow eyes locked on the fat man, lips pressed flat, chin tilted in contempt.
Camera: medium close-up, STATIC, 2 seconds.
Mood: icy menace.
```

### S07-03a　MS·婷婷抬小双腿欲脱鞋  
**引用素材**：`[CHAR-TT]` `[EXP-WILD]` `[CHAR-XS]` `[PROP-CARTOON-SOCKS]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
The red-haired girl with a wild manic grin stepping forward and lifting one of the yellow-haired girl's legs, hand poised to yank off her white cartoon-strawberry-bear knee-high sock, the yellow-haired girl half-laughing in surprise.
Camera: medium shot, STATIC, 3 seconds.
Mood: absurd intimidation tactic.
```

### S07-03b　MCU·胖子骤然怂  
**引用素材**：`[CHAR-FATTY]` `[EXP-SCARED]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
Reverse-angle medium close-up of the fat man's face deflating into cowardly fear, eyes flicking aside, lips pressed, leaning back as he retreats toward his seat.
Camera: medium close-up reverse, STATIC, 2 seconds.
Mood: deflated bully.
```

### S07-03c　CU·白离复杂注视  
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-REFLECT]`
```
[Style+Consistency prefix]
Close-up of the executive man's face, expression thoughtful and softened, eyes briefly catching warm light, faint inward smile, complex reflection in his pupils.
Camera: close-up, STATIC, 3 seconds.
Mood: world-view shifting.
```

---

## 第 8 场 · 老乡相认·夜窗盘算

### S08-01a　MCU·小双拉回话题  
**引用素材**：`[CHAR-XS]` `[EXP-CURIOUS]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
The yellow-haired girl tilting her head with big curious eyes, soft smile, leaning slightly toward the executive man, warm amber reading light.
Camera: medium close-up, STATIC, 3 seconds.
Mood: warm curiosity.
```

### S08-01b　CU·白离淡淡平县  
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-CALM]`
```
[Style+Consistency prefix]
Close-up reverse-angle of the executive man, composed neutral expression, slight controlled smile, soft amber light on his profile.
Camera: close-up reverse, STATIC, 2 seconds.
Mood: minimal disclosure.
```

### S08-01c　MS·三女惊呼老乡  
**引用素材**：`[CHAR-TT]` `[EXP-EXCITED]` `[CHAR-JX]` `[EXP-EXCITED]` `[CHAR-XS]` `[EXP-EXCITED]` `[PROP-CARTOON-SOCKS]` `[SCN-BUS-INT-NIGHT]`
```
[Style+Consistency prefix]
Medium shot of the three girls erupting in excited delight, the yellow-haired one slipping off her white sneakers and pulling her legs up onto the seat in a curled-up pose revealing the cartoon strawberry-bear print on her knee-high socks, the other two bouncing in their seats.
Camera: medium shot, STATIC, 4 seconds.
Mood: hometown miracle.
```

### S08-01d　MCU·白离不着痕迹瞥  
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-GLANCE]`
```
[Style+Consistency prefix]
Medium close-up of the executive man, eyes briefly shifting to the side then averting, otherwise neutral composed face, soft amber light.
Camera: medium close-up, STATIC, 3 seconds.
Mood: discreet calculation.
```

### S08-02a　MS·白离靠窗盘算  
**引用素材**：`[CHAR-BL-CASUAL]` `[EXP-SCHEME]` `[SCN-BUS-WINDOW-NIGHT]`
```
[Style+Consistency prefix]
Medium shot of the executive man leaning against the coach window at night, scenery streaming backwards outside as bokeh streaks of orange and white light, faint reflection of his thoughtful face overlaid on the glass, leaning chin on hand, faint cunning smile.
Camera: medium shot side, slow DOLLY-OUT, 5 seconds.
Mood: ambitious calm.
```

### S08-02b　EWS·大巴夜行远去  
**引用素材**：`[SCN-HIGHWAY-NIGHT]`
```
[Style+Consistency prefix]
Aerial high-angle shot of a single white long-distance coach driving away on a dark Chinese expressway at night, two long red tail-light streaks trailing behind, scattered orange sodium street lamps, deep blue-black sky, faint distant city glow on horizon.
Camera: drone high-angle, slow upward ASCENT with slight backward TRACK, 4 seconds.
Mood: journey continues.
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
