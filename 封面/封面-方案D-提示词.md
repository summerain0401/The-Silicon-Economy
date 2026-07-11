# 封面方案 D「机器报价单」· 终版生图提示词

封面文件：`封面-方案D-1600x2400.png`（2:3，电子书规格），由 `封面-方案D-出图源文件.html` 经 Chrome 无头模式渲染生成。以下提示词用于 AI 生图工具复刻底图（**无文字版**），价签字段与书名需后期叠加。

## Midjourney / 英文版

```
book cover background, one large vintage kraft paper price tag with punched
hole and thin hanging string from top edge, slightly rotated, floating in
upper two-thirds of warm manila-gold ground (#D3C093) with soft radial
light, realistic layered shadow beneath the tag, the tag surface clean
cream paper (#F6EFDF) left empty for text, subtle paper grain, still-life
product photography lighting, lower third of canvas empty for title
typography, nostalgic yet precise mood, no people, no other objects
--ar 2:3 --style raw
```

## 即梦 / 通义万相 中文版

```
书籍封面底图，一张大幅复古牛皮纸价格吊牌，顶部有穿孔和细绳悬挂，轻微倾斜，
悬浮于画面上三分之二处，暖金驼色背景（#D3C093）带柔和径向光，吊牌下方有
真实的层次投影，吊牌为干净的米白色纸面（#F6EFDF）留白待排字，细腻纸张纹理，
静物摄影布光，画面下三分之一留白供书名排版，怀旧而精确的氛围，无人物无其他
物体，比例 2:3
```

## 后期叠加的文字清单（按终稿版式）

| 元素 | 内容 | 字体 / 处理 |
|---|---|---|
| 价签主体 | $0.003 | JetBrains Mono，价签内居中特大 |
| 价签副行 | STABLECOIN · VALID 90S | JetBrains Mono，加宽字距，浅褐 |
| 字段三行 | status → 402 Payment Required / reader → not human / signed → machine wallet | JetBrains Mono，左右对齐，虚线分隔 |
| 书名 | 硅基经济学 | 思源宋体 Heavy，签外底部居中 |
| 署名行 | 热夏老友 著 · THE SILICON ECONOMY | 思源黑体 Medium，加宽字距 |

## 字体（全部 OFL 开源协议，可商用，不入库）

与方案 C 共用同一组字体，下载方法见《封面-方案C-提示词.md》的字体章节。

## 复刻 / 改版方法

改文字或配色后重新出图：编辑 HTML 源文件（需与 `fonts/` 同目录），然后执行：

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless=new --disable-gpu --hide-scrollbars \
  --window-size=1600,2400 \
  --screenshot=封面-方案D-1600x2400.png \
  --virtual-time-budget=5000 --allow-file-access-from-files \
  "file:///Volumes/Samsung/book/封面/封面-方案D-出图源文件.html"
```
