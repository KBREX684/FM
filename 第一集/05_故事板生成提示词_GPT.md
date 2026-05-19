# 第一集 · 故事板生成提示词文档（GPT Storyboard Prompts）

> 用途：用于在 **GPT（含图像生成能力）** 中生成 **黑白 / 单色铅笔故事板（Storyboard Panel）**，辅助 Kling 3.0 理解每个镜头 / 子镜头的构图、运镜、走位、视线、节奏。  
> 输出形式：每镜一张 **行业标准 6-cell 或单格故事板面板**，含构图框、运镜箭头、角色走位标识、视线线、镜头属性元信息。  
> 风格基底（全局 STYLE BASE，已内嵌每条 prompt）：  
> `professional film storyboard panel, black-and-white pencil sketch with light grey wash, clean line art, hand-drawn industry standard, framed within a 16:9 panel border with thin black outline, camera movement arrows in red, character blocking marks (numbered circles) in blue, eye-line dashed lines, scale 1:1, top-left panel ID label, bottom film-slate metadata strip with: SHOT, LENS, CAMERA, ACTION, DIALOGUE, SFX, TRANSITION, DURATION; aspect 16:9; legible English+Chinese annotations; high-resolution`

---

## 〇、通用 PROMPT 模板（GPT 直接复制粘贴）

> 把下面方括号内变量替换为对应镜头数据，即可生成单格故事板：

```
Generate a professional 16:9 film storyboard panel in black-and-white pencil sketch with light grey wash, clean line art, hand-drawn industry standard. Frame a [SHOT_TYPE景别] of [SCENE_DESCRIPTION场景与人物动作描述]. Indicate camera movement with a red arrow labeled "[CAMERA_MOVE运镜]". Mark character blocking with small blue numbered circles for each character (① ② ③ …) and connect their eye-lines with dashed lines. Top-left corner label: "[SHOT_ID镜号]". Bottom of panel: a film-slate metadata strip in monospace, exact text:
"SHOT: [SHOT_ID] | LENS: [LENS焦距] | CAM: [CAMERA_MOVE] | DUR: [DURATION秒]s | ACT: [ACTION动作概述] | DIA: [DIALOGUE台词或—] | SFX: [SFX音效或—] | TR: [TRANSITION转场]"
Maintain the style of a Hollywood / Korean drama production storyboard. Do not add color outside black, grey, red (arrows), blue (blocking). 16:9 panel border, thin black outline.
```

> **使用说明**：  
> ① 将下文每一镜的"填入参数"整段替换到上述模板对应方括号位置（已为每个镜头预先写好可直接拼装的参数 + 已经拼装好的成品 prompt）。  
> ② 镜头时长、台词、音效与 01 号文档保持严格一致；如有 V.O. 旁白以 `(V.O.)` 标注。  
> ③ 多角色镜头按"白离=① / 婷婷=② / 佳欣=③ / 小双=④ / 司机=⑤ / 胖子=⑥"统一编号，全片不变。

---

## 一、角色编号锁定（贯穿全集）

| 编号 | 角色 | 资产 ID |
|---|---|---|
| ① | 白离 | CHAR-BL-FORMAL / CHAR-BL-CASUAL |
| ② | 陈婷婷 | CHAR-TT |
| ③ | 李佳欣 | CHAR-JX |
| ④ | 林小双 | CHAR-XS |
| ⑤ | 司机 | CHAR-DRIVER |
| ⑥ | 胖子乘客 | CHAR-FATTY |

---

## 二、逐镜故事板提示词（已拼装，可直接复制）

### S01-01a
```
Generate a professional 16:9 film storyboard panel in black-and-white pencil sketch with light grey wash, clean line art. Frame an EWS (Extreme Wide Shot) of a North-China long-distance bus terminal plaza during Spring Festival rush, vast crowd with rolling luggage, red "春运" banner across the top, multiple parked white coaches, overcast sky. No named characters in foreground. Indicate camera movement with a red arrow labeled "HIGH-ANGLE + slow PUSH-IN". No character blocking circles. Top-left label: "S01-01a". Bottom strip exact text:
"SHOT: S01-01a | LENS: 24mm | CAM: HIGH-ANGLE + PUSH-IN | DUR: 4s | ACT: Establishing Spring Festival station plaza | DIA: — | SFX: Crowd chatter, broadcast, horns | TR: CUT"
Hollywood / Korean drama storyboard style, monochrome with red arrows only, 16:9 panel border.
```

### S01-01b
```
Storyboard panel, 16:9 B/W pencil + grey wash. MLS of driver ⑤ in a quilted coat and "运" cap shouting into a red plastic megaphone, foreground passengers passing as silhouettes in bokeh, ticket gate signage behind. Camera: red arrow labeled "STATIC + foreground parallax". Blocking circle ⑤ at center frame. Top-left label "S01-01b". Bottom strip:
"SHOT: S01-01b | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Driver shouting to crowd | DIA: ⑤ \"魔都去运市还有没有？马上发车了！\" | SFX: Megaphone amp | TR: CUT"
```

### S01-02a
```
Storyboard panel, 16:9 B/W pencil + grey wash. MS three-quarter back of ① (Bai Li) walking through a thick crowd toward a parked coach, pulling a silver luggage. Camera: red arrow labeled "TRACK behind + slight OVER-SHOULDER". Blocking ① center-frame moving forward, dashed eye-line forward to the coach. Top-left "S01-02a". Bottom strip:
"SHOT: S01-02a | LENS: 35mm | CAM: TRACK | DUR: 4s | ACT: Bai Li pulls luggage through crowd | DIA: ① (V.O.) \"草，要不是那傻吊老板临时开会……\" | SFX: Luggage wheels, crowd | TR: CUT"
```

### S01-02b
```
Storyboard panel, 16:9 B/W pencil + grey wash. CU low-angle of four spinner wheels rolling across damp grey concrete tiles, splash droplets. Camera: red arrow "GROUND-LEVEL STATIC, subtle forward motion". No blocking circles. Top-left "S01-02b". Bottom strip:
"SHOT: S01-02b | LENS: 35mm macro | CAM: STATIC | DUR: 2s | ACT: Luggage wheels splash on wet ground | DIA: — | SFX: Wheel clatter | TR: MATCH-CUT to coach door"
```

### S01-03
```
Storyboard panel, 16:9 B/W. MLS of ① stepping onto the metal step of coach "沪 A·B8868", glance up at sky, breath fog. Camera: red arrow "slow DOLLY-IN". Blocking ① on the step center-right, eye-line dashed upward. Top-left "S01-03". Bottom strip:
"SHOT: S01-03 | LENS: 35mm | CAM: DOLLY-IN | DUR: 4s | ACT: Bai Li boards coach, looks at sky | DIA: ① (V.O.) inner monologue | SFX: Bus idle | TR: CUT"
```

### S02-01a
```
Storyboard panel, 16:9 B/W. MLS interior coach aisle looking back from front, two rows of seats with empty rear three-seat row at center lit by a side window beam. Camera: red arrow "slow DOLLY-IN aisle to rear". No blocking. Top-left "S02-01a". Bottom strip:
"SHOT: S02-01a | LENS: 28mm | CAM: DOLLY-IN | DUR: 5s | ACT: Reveal empty back row | DIA: — | SFX: Engine idle, low chatter | TR: CUT"
```

### S02-01b
```
Storyboard panel, 16:9 B/W. MS 3/4 front of ① lifting silver luggage onto overhead rack then settling into leftmost window seat of back row. Camera: red arrow "TRACK following his motion". Blocking ① arc-line moving up then down into seat. Top-left "S02-01b". Bottom strip:
"SHOT: S02-01b | LENS: 35mm | CAM: TRACK | DUR: 3s | ACT: Bai Li seats himself | DIA: — | SFX: Fabric, rack clink | TR: CUT"
```

### S02-02
```
Storyboard panel, 16:9 B/W. CU side 45° of ①'s face leaning back, eyes closed, earphone cable visible at collar. Camera: red arrow "STATIC". Blocking ① right-center. Top-left "S02-02". Bottom strip:
"SHOT: S02-02 | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li tries to nap | DIA: ① (V.O.) \"睡会儿吧……\" | SFX: Earphone music faint | TR: CUT"
```

### S02-03a
```
Storyboard panel, 16:9 B/W. MLS at front coach door, three girls ②③④ squeezing in noisily, ④ in lead. Camera: red arrow "quick PUSH-IN + micro HANDHELD". Blocking ④ front, ② middle, ③ back, arrow lines of motion forward. Top-left "S02-03a". Bottom strip:
"SHOT: S02-03a | LENS: 28mm | CAM: PUSH-IN + HANDHELD | DUR: 3s | ACT: Three girls board loudly | DIA: ④ \"婷婷姐，快点快点！\" ② \"急什么？\" | SFX: Door, footsteps | TR: CUT"
```

### S02-03b
```
Storyboard panel, 16:9 B/W. CU of ① snapping eyes open and side-glancing toward front of coach. Camera: red arrow "STATIC". Blocking ① center, dashed eye-line forward-left. Top-left "S02-03b". Bottom strip:
"SHOT: S02-03b | LENS: 85mm | CAM: STATIC | DUR: 2s | ACT: Bai Li's annoyed glance | DIA: — | SFX: — | TR: CUT"
```

### S02-04a
```
Storyboard panel, 16:9 B/W. MS down aisle, three girls ④②③ walking toward back row, ④ pointing forward excitedly. Camera: red arrow "PAN + slight PUSH-IN". Blocking ④ front-pointing, ② mid-swagger, ③ rolling eyes; motion arrows forward. Top-left "S02-04a". Bottom strip:
"SHOT: S02-04a | LENS: 35mm | CAM: PAN + PUSH-IN | DUR: 4s | ACT: Trio approaches back row | DIA: ④ \"最后面刚好有三个空位！\" | SFX: Footsteps | TR: CUT"
```

### S02-04b
```
Storyboard panel, 16:9 B/W. POV from ①'s seat, the trio walking straight toward camera. Camera: red arrow "POV STATIC, micro breathing shake". Blocking ④②③ as silhouettes facing camera. Top-left "S02-04b". Bottom strip:
"SHOT: S02-04b | LENS: 35mm | CAM: POV STATIC | DUR: 3s | ACT: Bai Li's POV dread | DIA: ① (V.O.) \"千万别坐我旁边……\" | SFX: — | TR: CUT"
```

### S02-05a
```
Storyboard panel, 16:9 B/W. MS front-on of back row, from L to R: ① by window, ④, ③, ②. Camera: red arrow "STATIC". Blocking circles ①④③② left to right in seat line. Top-left "S02-05a". Bottom strip:
"SHOT: S02-05a | LENS: 28mm | CAM: STATIC | DUR: 4s | ACT: Four squeezed in back row | DIA: — | SFX: Seat creak | TR: CUT"
```

### S02-05b
```
Storyboard panel, 16:9 B/W. CU TILT-DOWN of charcoal suit trouser leg pressed beside a young girl's bare thigh in denim shorts, tasteful framing, no exposure. Camera: red arrow "TILT-DOWN STATIC". Blocking ① ④ partial. Top-left "S02-05b". Bottom strip:
"SHOT: S02-05b | LENS: 50mm | CAM: TILT-DOWN | DUR: 3s | ACT: Suggest crowded forced proximity | DIA: — | SFX: Engine hum | TR: CUT"
```

### S02-05c
```
Storyboard panel, 16:9 B/W. MS of ② mid-rant + ③ nodding cold smirk, surrounding passengers blurred turning disapproving glances. Camera: red arrow "STATIC". Blocking ② center, ③ right, dashed eye-line from other passengers to the duo. Top-left "S02-05c". Bottom strip:
"SHOT: S02-05c | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Loud cursing draws stares | DIA: ② \"那破厂子真不是人待的！\" ③ \"回去就删了那死胖子主管！\" | SFX: — | TR: CUT"
```

### S03-01a
```
Storyboard panel, 16:9 B/W. EWS aerial side of a single coach on empty expressway at dusk. Camera: red arrow "DRONE side TRACK". No blocking. Top-left "S03-01a". Bottom strip:
"SHOT: S03-01a | LENS: 50mm aerial | CAM: DRONE TRACK | DUR: 3s | ACT: Coach on dusk highway | DIA: — | SFX: Wind, engine | TR: CUT"
```

### S03-01b
```
Storyboard panel, 16:9 B/W. CU of ④'s face pale and motion-sick, hand covering mouth. Camera: red arrow "STATIC". Blocking ④ center, dashed eye-line down. Top-left "S03-01b". Bottom strip:
"SHOT: S03-01b | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Lin Xiao Shuang carsick | DIA: ④ \"婷婷姐，我有点晕车。\" | SFX: — | TR: CUT"
```

### S03-02a
```
Storyboard panel, 16:9 B/W. MCU side 45° of ④ timidly touching ①'s sleeve and pleading. Camera: red arrow "STATIC". Blocking ④ left, ① right edge; dashed eye-line ④→①. Top-left "S03-02a". Bottom strip:
"SHOT: S03-02a | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Xiaoshuang asks for water | DIA: ④ \"大…大叔，能给口水喝吗？\" | SFX: — | TR: CUT"
```

### S03-02b
```
Storyboard panel, 16:9 B/W. ECU of ①'s mouth area, subtle single twitch. Camera: red arrow "STATIC". Blocking — (face fragment). Top-left "S03-02b". Bottom strip:
"SHOT: S03-02b | LENS: 100mm macro | CAM: STATIC | DUR: 1.5s | ACT: Mouth corner twitch | DIA: ① (V.O.) \"二十六岁，大叔？\" | SFX: — | TR: CUT"
```

### S03-02c
```
Storyboard panel, 16:9 B/W. CU low-angle top-down of mineral water bottle on suit trouser leg. Camera: red arrow "STATIC top-down". No blocking. Top-left "S03-02c". Bottom strip:
"SHOT: S03-02c | LENS: 50mm | CAM: STATIC | DUR: 2s | ACT: Water bottle on lap | DIA: — | SFX: — | TR: CUT"
```

### S03-03a
```
Storyboard panel, 16:9 B/W. MCU of ① cold-faced, lips flat. Camera: red arrow "STATIC". Blocking ① center. Top-left "S03-03a". Bottom strip:
"SHOT: S03-03a | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li refuses coldly | DIA: ① \"我的水，喝过了。\" | SFX: — | TR: CUT"
```

### S03-03b
```
Storyboard panel, 16:9 B/W. MS of ④ eyes lighting up, taking the bottle confidently. Camera: red arrow "STATIC". Blocking ④ left reaching, ① right; arrow line ④→bottle. Top-left "S03-03b". Bottom strip:
"SHOT: S03-03b | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Xiaoshuang grabs bottle | DIA: ④ \"就要喝过的！没喝过的还得给钱呢！\" | SFX: Cap twist | TR: CUT"
```

### S03-03c
```
Storyboard panel, 16:9 B/W. CU side profile of ④ chugging water, throat swallowing. Camera: red arrow "STATIC side". Blocking ④ center. Top-left "S03-03c". Bottom strip:
"SHOT: S03-03c | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Xiaoshuang drinks | DIA: — | SFX: Gulping | TR: CUT"
```

### S03-03d
```
Storyboard panel, 16:9 B/W. CU bottle with faint lip print, being handed back into ①'s hand. Camera: red arrow "STATIC". Blocking ④ hand left, ① hand right. Top-left "S03-03d". Bottom strip:
"SHOT: S03-03d | LENS: 100mm macro | CAM: STATIC | DUR: 2s | ACT: Bottle returned with lip mark | DIA: — | SFX: — | TR: CUT"
```

### S03-04a
```
Storyboard panel, 16:9 B/W. MCU of ① waving hand dismissively. Camera: red arrow "STATIC". Blocking ① center. Top-left "S03-04a". Bottom strip:
"SHOT: S03-04a | LENS: 85mm | CAM: STATIC | DUR: 2s | ACT: Bai Li gifts the bottle | DIA: ① \"送你了，不要了。\" | SFX: — | TR: CUT"
```

### S03-04b
```
Storyboard panel, 16:9 B/W. CU of ④ head lowered, clutching bottle to chest. Camera: red arrow "STATIC". Blocking ④ center. Top-left "S03-04b". Bottom strip:
"SHOT: S03-04b | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Xiaoshuang shy thanks | DIA: ④ \"哦…谢谢。\" | SFX: — | TR: MATCH to ①'s eye"
```

### S03-04c
```
Storyboard panel, 16:9 B/W with extra cyan-blue accent lines for system text reflection. ECU of one eye of ①, holographic Chinese characters reflected on the iris surface. Camera: red arrow "STATIC + slight ZOOM-IN". Blocking — (eye only). Top-left "S03-04c". Bottom strip:
"SHOT: S03-04c | LENS: 100mm macro | CAM: STATIC + ZOOM-IN | DUR: 4s | ACT: System binding in pupil | DIA: SYS V.O. \"检测到宿主首次进行投资行为……绑定成功！\" | SFX: Sci-fi binding tone | TR: FLASH blue"
```

### S04-01a
```
Storyboard panel, 16:9 B/W + cyan-blue accent for holographic UI. MS front of ① with a semi-transparent panel floating in front of his face, sci-fi typography "宿主：白离 / 系统：女神投资系统 / 功能：女神雷达、投资返利". Camera: red arrow "STATIC". Blocking ① center, panel between ① and camera. Top-left "S04-01a". Bottom strip:
"SHOT: S04-01a | LENS: 50mm | CAM: STATIC | DUR: 4s | ACT: System main panel reveal | DIA: SYS V.O. UI tone | SFX: Soft UI chime | TR: CUT"
```

### S04-01b
```
Storyboard panel, 16:9 B/W + cyan-blue accent. CU side of ①'s hand poking through the panel, finger glowing faintly. Camera: red arrow "STATIC side". Blocking ①'s arm. Top-left "S04-01b". Bottom strip:
"SHOT: S04-01b | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li tests panel solidity | DIA: — | SFX: — | TR: CUT"
```

### S04-01c
```
Storyboard panel, 16:9 B/W. MCU reverse of ②③④ and nearby passengers, all unconcerned. Camera: red arrow "STATIC reverse". Blocking ②③④ across frame. Top-left "S04-01c". Bottom strip:
"SHOT: S04-01c | LENS: 35mm | CAM: STATIC | DUR: 3s | ACT: Others unaware of panel | DIA: — | SFX: Low chatter | TR: CUT"
```

### S04-02a
```
Storyboard panel, 16:9 B/W + cyan-blue accent. CU of holographic functions panel: "女神雷达 / 投资返利 / 倾心值 0/30/60/80/100". Camera: red arrow "STATIC + slight ZOOM-IN". No blocking. Top-left "S04-02a". Bottom strip:
"SHOT: S04-02a | LENS: 50mm | CAM: ZOOM-IN | DUR: 4s | ACT: Rules of the system revealed | DIA: SYS V.O. reads rules | SFX: UI tone | TR: CUT"
```

### S04-02b
```
Storyboard panel, 16:9 B/W + cyan-blue accent. POV MS sweeping over ②③④ with name tags popping above their heads: ② 0/路人, ③ 0/路人, ④ +10/略有好感. Camera: red arrow "POV PAN L→R". Blocking ②③④ across, scanner line sweep. Top-left "S04-02b". Bottom strip:
"SHOT: S04-02b | LENS: 35mm | CAM: POV PAN | DUR: 5s | ACT: Goddess radar scans the three | DIA: SYS V.O. tag-ping per girl | SFX: Beep beep beep | TR: CUT"
```

### S04-02c
```
Storyboard panel, 16:9 B/W. ECU of ①'s eyes blazing with greedy smirk. Camera: red arrow "STATIC". Blocking — (eyes). Top-left "S04-02c". Bottom strip:
"SHOT: S04-02c | LENS: 100mm macro | CAM: STATIC | DUR: 2s | ACT: Bai Li's predatory awakening | DIA: ① (V.O.) \"三棵摇钱树啊！\" | SFX: — | TR: MATCH to neon sign"
```

### S05-01a
```
Storyboard panel, 16:9 B/W. LS night service area, neon "XX 服务区" sign on building, coach parked, wet asphalt. Camera: red arrow "slow DOLLY-IN". No blocking. Top-left "S05-01a". Bottom strip:
"SHOT: S05-01a | LENS: 28mm | CAM: DOLLY-IN | DUR: 4s | ACT: Arrive at rest stop | DIA: ⑤ \"停车休息二十分钟！\" | SFX: Air brake | TR: CUT"
```

### S05-01b
```
Storyboard panel, 16:9 B/W. MS of ① walking out of convenience store with noodle cup + new water bottle. Camera: red arrow "TRACK in front". Blocking ① center forward motion. Top-left "S05-01b". Bottom strip:
"SHOT: S05-01b | LENS: 35mm | CAM: TRACK | DUR: 3s | ACT: Bai Li exits store with food | DIA: — | SFX: Door bell | TR: CUT"
```

### S05-02a
```
Storyboard panel, 16:9 B/W. MS 3/4 at standing counter, ① tearing open foil noodle lid, steam. Camera: red arrow "STATIC". Blocking ① center. Top-left "S05-02a". Bottom strip:
"SHOT: S05-02a | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Bai Li peels off lid | DIA: — | SFX: Foil tear | TR: CUT"
```

### S05-02b
```
Storyboard panel, 16:9 B/W. MS of ②③④ lingering, eyes on food. Camera: red arrow "STATIC". Blocking ② left, ③ middle, ④ right; dashed eye-lines toward food off-frame. Top-left "S05-02b". Bottom strip:
"SHOT: S05-02b | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Three girls hungry stare | DIA: — | SFX: Quiet ambient | TR: CUT"
```

### S05-03a
```
Storyboard panel, 16:9 B/W. MCU of ② approaching counter, arms crossed awkwardly. Camera: red arrow "STATIC". Blocking ② center. Top-left "S05-03a". Bottom strip:
"SHOT: S05-03a | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Tingting approaches Bai Li | DIA: ② \"大哥。\" | SFX: — | TR: CUT"
```

### S05-03b
```
Storyboard panel, 16:9 B/W. MCU reverse of ① calmly opening WeChat QR code on phone. Camera: red arrow "STATIC reverse". Blocking ① center, phone in lower frame. Top-left "S05-03b". Bottom strip:
"SHOT: S05-03b | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Bai Li opens QR | DIA: ① \"要多少？\" | SFX: Phone tap | TR: CUT"
```

### S05-03c
```
Storyboard panel, 16:9 B/W. MS slight overhead of ②③④ huddled whispering. Camera: red arrow "STATIC overhead-slight". Blocking ②③④ in triangle. Top-left "S05-03c". Bottom strip:
"SHOT: S05-03c | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Trio negotiates the number | DIA: (whispers) | SFX: — | TR: CUT"
```

### S05-03d
```
Storyboard panel, 16:9 B/W. CU of ② carefully raising one finger. Camera: red arrow "STATIC". Blocking ② center. Top-left "S05-03d". Bottom strip:
"SHOT: S05-03d | LENS: 85mm | CAM: STATIC | DUR: 2s | ACT: Tingting signals \"ten\" | DIA: ② \"十……十块钱。\" | SFX: — | TR: CUT"
```

### S05-04a
```
Storyboard panel, 16:9 B/W. ECU top-down of phone transfer page "￥10.00", finger pressing confirm. Camera: red arrow "STATIC top-down". Blocking — (hand). Top-left "S05-04a". Bottom strip:
"SHOT: S05-04a | LENS: 50mm macro | CAM: STATIC | DUR: 2s | ACT: Bai Li confirms transfer | DIA: — | SFX: WeChat ding | TR: CUT"
```

### S05-04b
```
Storyboard panel, 16:9 B/W. CU of cracked-screen phone in ②'s hand showing "微信支付：到账 10.00 元". Camera: red arrow "STATIC". Blocking ② upper, hand+phone center. Top-left "S05-04b". Bottom strip:
"SHOT: S05-04b | LENS: 85mm | CAM: STATIC | DUR: 2s | ACT: Tingting sees the money landed | DIA: — | SFX: Notification ping | TR: CUT"
```

### S05-04c
```
Storyboard panel, 16:9 B/W. MS of ②③④ lifting heads, expressions softening to grateful. Camera: red arrow "STATIC + gentle PUSH-IN". Blocking ②③④ across. Top-left "S05-04c". Bottom strip:
"SHOT: S05-04c | LENS: 35mm | CAM: PUSH-IN | DUR: 3s | ACT: Gratitude blooms | DIA: — | SFX: — | TR: CUT"
```

### S05-05a
```
Storyboard panel, 16:9 B/W + cyan-blue accent for reward panel. CU of ① with reward UI overlay "投资目标：陈婷婷 / 触发 10 倍暴击 / 获得返利 100". Camera: red arrow "STATIC". Blocking ① center. Top-left "S05-05a". Bottom strip:
"SHOT: S05-05a | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li sees 10x reward popup | DIA: SYS V.O. \"触发 10 倍暴击返利！\" | SFX: Crit chime | TR: CUT"
```

### S05-05b
```
Storyboard panel, 16:9 B/W. ECU of phone bank SMS banner exact text "收入 100.00 元，余额 300,100.00 元". Camera: red arrow "STATIC top-down". Blocking — (phone). Top-left "S05-05b". Bottom strip:
"SHOT: S05-05b | LENS: 50mm macro | CAM: STATIC | DUR: 2s | ACT: Real bank confirmation | DIA: — | SFX: SMS ping | TR: CUT"
```

### S05-05c
```
Storyboard panel, 16:9 B/W. CU of ① subtle smirk, three out-of-focus girl backs (②③④) running off in background. Camera: red arrow "STATIC". Blocking ① center, ②③④ small in distance. Top-left "S05-05c". Bottom strip:
"SHOT: S05-05c | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li's contented smirk | DIA: ① (V.O.) \"这趟回家的路，似乎变得有趣起来。\" | SFX: — | TR: MATCH to bag noodle"
```

### S06-01a
```
Storyboard panel, 16:9 B/W. MCU top-down of ②③④ squatting around bag noodle, ② holding it open as hot water pours in, steam. Camera: red arrow "STATIC top-down". Blocking ②③④ triangle. Top-left "S06-01a". Bottom strip:
"SHOT: S06-01a | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Pour water into bag noodle | DIA: — | SFX: Water pour | TR: CUT"
```

### S06-01b
```
Storyboard panel, 16:9 B/W. CU slight overhead of three heads sharing one pair of chopsticks. Camera: red arrow "STATIC". Blocking ②③④ triangle close. Top-left "S06-01b". Bottom strip:
"SHOT: S06-01b | LENS: 50mm | CAM: STATIC | DUR: 4s | ACT: Trio shares the noodles | DIA: — | SFX: Slurping | TR: CUT"
```

### S06-01c
```
Storyboard panel, 16:9 B/W. MS of ②③④ tossing tied trash bag into green bin. Camera: red arrow "STATIC". Blocking ②③④ near bin. Top-left "S06-01c". Bottom strip:
"SHOT: S06-01c | LENS: 35mm | CAM: STATIC | DUR: 3s | ACT: They clean up | DIA: — | SFX: Bag rustle | TR: CUT"
```

### S06-02a
```
Storyboard panel, 16:9 B/W. MS side in night coach, ② offering Nanjing-Mengdu cigarette to ①. Camera: red arrow "STATIC". Blocking ② left, ① right; dashed eye-line ②→①. Top-left "S06-02a". Bottom strip:
"SHOT: S06-02a | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Tingting offers cigarette | DIA: ② \"大哥，抽烟不？\" | SFX: — | TR: CUT"
```

### S06-02b
```
Storyboard panel, 16:9 B/W. MCU of ① in vest (no trench) pinching Yuhuashi cigarette in lips, offering pack. Camera: red arrow "STATIC". Blocking ① center, pack extended to right. Top-left "S06-02b". Bottom strip:
"SHOT: S06-02b | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Bai Li offers his pack | DIA: ① \"抽我的吧。\" | SFX: — | TR: CUT"
```

### S06-02c
```
Storyboard panel, 16:9 B/W. CU of ②③④ in stacked composition, all wide-eyed O-mouth. Camera: red arrow "STATIC". Blocking ②③④ tight cluster. Top-left "S06-02c". Bottom strip:
"SHOT: S06-02c | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Three girls amazed | DIA: ② \"我套你哥，居然是雨花石！\" ③ \"大哥你真敞亮！\" | SFX: — | TR: CUT"
```

### S06-03
```
Storyboard panel, 16:9 B/W. MS of ②③④ each holding lit cigarette, deep first drag, smoke wisps. Camera: red arrow "slow PUSH-IN". Blocking ②③④ across frame, smoke vector lines. Top-left "S06-03". Bottom strip:
"SHOT: S06-03 | LENS: 50mm | CAM: PUSH-IN | DUR: 4s | ACT: Trio's first satisfying drag | DIA: — | SFX: Lighter click, exhale | TR: CUT"
```

### S07-01a
```
Storyboard panel, 16:9 B/W. MS from back row perspective, ⑥ standing in aisle leering at ②③④. Camera: red arrow "STATIC". Blocking ⑥ aisle-center, ②③④ seated; dashed eye-line ⑥→girls. Top-left "S07-01a". Bottom strip:
"SHOT: S07-01a | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Fatty intrudes | DIA: ⑥ \"哟，小兄弟挺有钱啊……真特么嫩。\" | SFX: — | TR: CUT"
```

### S07-01b
```
Storyboard panel, 16:9 B/W. ECU of ①'s ice-cold eyes. Camera: red arrow "STATIC". Blocking — (eyes). Top-left "S07-01b". Bottom strip:
"SHOT: S07-01b | LENS: 100mm macro | CAM: STATIC | DUR: 2s | ACT: Bai Li freezes | DIA: — | SFX: — | TR: CUT"
```

### S07-02a
```
Storyboard panel, 16:9 B/W. MCU of ② finger-jabbing ⑥ mid-curse. Camera: red arrow "fast PUSH-IN". Blocking ② upright forward, ⑥ partial in foreground; arrow ②→⑥. Top-left "S07-02a". Bottom strip:
"SHOT: S07-02a | LENS: 50mm | CAM: PUSH-IN | DUR: 3s | ACT: Tingting explodes | DIA: ② \"再敢狗叫一句，信不信老娘用小双的臭鞋抽打你？\" | SFX: — | TR: CUT"
```

### S07-02b
```
Storyboard panel, 16:9 B/W. MCU of ④ trying to look tough. Camera: red arrow "STATIC". Blocking ④ center. Top-left "S07-02b". Bottom strip:
"SHOT: S07-02b | LENS: 50mm | CAM: STATIC | DUR: 2s | ACT: Xiaoshuang follow-up | DIA: ④ \"婷婷姐说的对！\" | SFX: — | TR: CUT"
```

### S07-02c
```
Storyboard panel, 16:9 B/W. MCU of ③ cold-face, pulling leg down. Camera: red arrow "STATIC". Blocking ③ center. Top-left "S07-02c". Bottom strip:
"SHOT: S07-02c | LENS: 50mm | CAM: STATIC | DUR: 2s | ACT: Jiaxin icy threat | DIA: ③ \"你老冯飞了，不允许返航的那种。\" | SFX: — | TR: CUT"
```

### S07-03a
```
Storyboard panel, 16:9 B/W. MS of ② lifting ④'s leg, hand at sock about to yank off. Camera: red arrow "STATIC". Blocking ② standing, ④ seated leg up; arrow ②'s hand→sock. Top-left "S07-03a". Bottom strip:
"SHOT: S07-03a | LENS: 35mm | CAM: STATIC | DUR: 3s | ACT: Tingting threatens sock-weapon | DIA: — | SFX: — | TR: CUT"
```

### S07-03b
```
Storyboard panel, 16:9 B/W. MCU reverse of ⑥ deflated, leaning back. Camera: red arrow "STATIC reverse". Blocking ⑥ center leaning back arrow. Top-left "S07-03b". Bottom strip:
"SHOT: S07-03b | LENS: 50mm | CAM: STATIC | DUR: 2s | ACT: Fatty backs off | DIA: — | SFX: Snort | TR: CUT"
```

### S07-03c
```
Storyboard panel, 16:9 B/W. CU of ① thoughtful softened face. Camera: red arrow "STATIC". Blocking ① center, dashed eye-line toward girls. Top-left "S07-03c". Bottom strip:
"SHOT: S07-03c | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li reflects on loyalty | DIA: ① (V.O.) \"一包泡面、三根烟，就能换来如此讲义气……\" | SFX: — | TR: MATCH to window"
```

### S08-01a
```
Storyboard panel, 16:9 B/W. MCU of ④ tilting head curious. Camera: red arrow "STATIC". Blocking ④ center. Top-left "S08-01a". Bottom strip:
"SHOT: S08-01a | LENS: 50mm | CAM: STATIC | DUR: 3s | ACT: Xiaoshuang asks hometown | DIA: ④ \"大哥，你是运市哪的啊？\" | SFX: — | TR: CUT"
```

### S08-01b
```
Storyboard panel, 16:9 B/W. CU reverse of ① calmly answering. Camera: red arrow "STATIC reverse". Blocking ① center. Top-left "S08-01b". Bottom strip:
"SHOT: S08-01b | LENS: 85mm | CAM: STATIC | DUR: 2s | ACT: Bai Li answers Pingxian | DIA: ① \"平县。\" | SFX: — | TR: CUT"
```

### S08-01c
```
Storyboard panel, 16:9 B/W. MS of ②③④ erupting in excitement, ④ pulling legs up onto seat revealing cartoon strawberry-bear socks. Camera: red arrow "STATIC". Blocking ② left, ③ middle, ④ right with bent legs. Top-left "S08-01c". Bottom strip:
"SHOT: S08-01c | LENS: 35mm | CAM: STATIC | DUR: 4s | ACT: Hometown miracle | DIA: ②③④ \"我嘞个雷！我们也是平县的！\" | SFX: — | TR: CUT"
```

### S08-01d
```
Storyboard panel, 16:9 B/W. MCU of ① discreet side-glance then averting. Camera: red arrow "STATIC". Blocking ① center, dashed eye-line briefly to ④ then forward. Top-left "S08-01d". Bottom strip:
"SHOT: S08-01d | LENS: 85mm | CAM: STATIC | DUR: 3s | ACT: Bai Li's discreet glance | DIA: ① (V.O.) \"再说吧。\" | SFX: — | TR: CUT"
```

### S08-02a
```
Storyboard panel, 16:9 B/W. MS side of ① leaning against window, bokeh streaks outside, faint face reflection on glass. Camera: red arrow "slow DOLLY-OUT". Blocking ① right window-side. Top-left "S08-02a". Bottom strip:
"SHOT: S08-02a | LENS: 50mm | CAM: DOLLY-OUT | DUR: 5s | ACT: Bai Li schemes by the window | DIA: ① (V.O.) \"这三棵潜力巨大的摇钱树，该如何浇灌呢？\" | SFX: BGM out | TR: CUT"
```

### S08-02b
```
Storyboard panel, 16:9 B/W. EWS aerial of coach driving away on dark expressway, twin red tail-light streaks. Camera: red arrow "DRONE high-angle ASCENT + slight backward TRACK". No blocking. Top-left "S08-02b". Bottom strip:
"SHOT: S08-02b | LENS: 35mm aerial | CAM: DRONE ASCENT | DUR: 4s | ACT: Coach drives off into night | DIA: — | SFX: BGM in suspense hook | TR: FADE OUT"
```

---

## 三、使用建议

1. **GPT 生图模型**：DALL·E 3 / GPT Image 输出最稳；先一次性把"通用 PROMPT 模板 + 角色编号锁定"贴入对话作为系统约束，再逐镜请求面板。  
2. **批量生产**：可一次发 6 个镜头 prompt，让 GPT 输出一张 2×3 的 6-cell 故事板拼版。  
3. **复用喂入 Kling**：生成的故事板面板可作为 Kling 3.0 的 **构图参考图**（与 04 号文档的关键帧色彩参考图并用：故事板=构图与运镜，关键帧=色彩与角色长相）。  
4. **保持人物编号统一**：①–⑥ 编号贯穿全集，便于后续集数继续延展。

