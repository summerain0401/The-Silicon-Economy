# 封面方案 C「两层经济」· 终版生图提示词

选定封面：`封面-方案C-1600x2400.png`（2:3，电子书规格），由 `封面-方案C-出图源文件.html` 经 Chrome 无头模式渲染生成。以下提示词用于 AI 生图工具复刻底图（**无文字版**），书名等排版元素需后期叠加。

## Midjourney / 英文版

```
book cover background split horizontally into two worlds: upper 55% warm
paper cream texture (#EFEAE2) with soft natural light from top-left, lower
45% deep charcoal-navy (#14181D) densely filled with micro-rows of tiny
monospace numbers and transaction codes (0.003, 402, ¥0.01, sig:ok, usdc)
fading into darkness at the bottom, the two layers separated by a single
thin glowing copper seam line (#C87832) with a faint halo, a few number
fragments in the dark layer highlighted in copper orange, conceptual
editorial book design, flat, precise, no people, no objects
--ar 2:3 --style raw
```

## 即梦 / 通义万相 中文版

```
书籍封面底图，画面水平分割为两个世界：上部55%为温暖的米白色纸张质感
（#EFEAE2），左上有柔和自然光；下部45%为深炭蓝色（#14181D），密布微小的
等宽字体数字与交易代码（0.003、402、¥0.01 等），底部渐隐入黑暗；两层之间
由一条发光的细铜色接缝（#C87832）分隔，带微弱光晕；暗层中少数数字用铜橙色
点亮；概念性编辑设计风格，扁平精确，无人物无实物，比例 2:3
```

## 后期叠加的文字清单（按终稿版式）

| 元素 | 内容 | 字体 / 处理 |
|---|---|---|
| 左上角标签 | 碳基 · CARBON | 黑体，加宽字距，浅褐灰 |
| 书名 | 硅基 / 经济学（两行） | 宋体特粗，约占上层高度一半 |
| 副题 | 人类在上层过日子，机器在下层结算 | 黑体，褐灰 |
| 署名 | 热夏老友 著 | 宋体加粗，加宽字距 |
| 右下角标签 | 硅基 · SILICON | 黑体，加宽字距，蓝灰 |

## 字体（全部 OFL 开源协议，可商用，不入库）

| 用途 | 字体 | 文件 |
|---|---|---|
| 书名/署名 | 思源宋体 Source Han Serif SC | SourceHanSerifSC-Heavy.otf / -Bold.otf |
| 标签/副题 | 思源黑体 Source Han Sans SC | SourceHanSansSC-Medium.otf |
| 交易流水 | JetBrains Mono | JetBrainsMono-Regular.ttf |

字体文件体积大（共约 66MB）不入 git，复刻前先下载到源文件同目录的 `fonts/` 文件夹：

```bash
mkdir -p fonts && cd fonts
curl -sSL -O "https://github.com/adobe-fonts/source-han-serif/raw/release/OTF/SimplifiedChinese/SourceHanSerifSC-Heavy.otf"
curl -sSL -O "https://github.com/adobe-fonts/source-han-serif/raw/release/OTF/SimplifiedChinese/SourceHanSerifSC-Bold.otf"
curl -sSL -O "https://github.com/adobe-fonts/source-han-sans/raw/release/OTF/SimplifiedChinese/SourceHanSansSC-Medium.otf"
curl -sSL -O "https://github.com/JetBrains/JetBrainsMono/raw/master/fonts/ttf/JetBrainsMono-Regular.ttf"
```

## 复刻 / 改版方法

改文字或配色后重新出图：编辑 HTML 源文件（需与 `fonts/` 同目录），然后执行：

```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless=new --disable-gpu --hide-scrollbars \
  --window-size=1600,2400 \
  --screenshot=封面-方案C-1600x2400.png \
  --virtual-time-budget=5000 --allow-file-access-from-files \
  "file:///Volumes/Samsung/book/封面/封面-方案C-出图源文件.html"
```
