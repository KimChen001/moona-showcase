<p align="center">
  <strong>MOONA 桌面伴侣</strong><br />
  一个在桌上等你的小 MOONA。
</p>

<p align="center">
  <a href="README.zh-CN.md">回到 MOONA</a> ·
  <a href="desk-companion.md">English</a>
</p>

<p align="center"><img src="assets/desk-companion/hero.png" width="420" alt="MOONA 桌面伴侣：乳白色硅胶外壳、圆形屏幕，放在充电底座上" /></p>

MOONA 现在住在网页里。桌面伴侣给它一个身体：一个手掌大小、乳白色软硅胶的小球，脸是一块 1.75 英寸的圆形 AMOLED 屏。叫它一声它就醒来，用声音回答你；放回磁吸底座上就开始充电。

**现状：设计中。** 这一页的图片是概念模型和屏幕设计，不是成品照片。

## 圆屏上会出现什么

<table>
  <tr>
    <td align="center"><img src="assets/desk-companion/screens/idle.webp" width="160" alt="待机" /><br /><b>待机</b><br />光球慢慢呼吸</td>
    <td align="center"><img src="assets/desk-companion/screens/listening.webp" width="160" alt="在听" /><br /><b>在听</b><br />你说话时，金色的圈慢慢画满</td>
    <td align="center"><img src="assets/desk-companion/screens/thinking.webp" width="160" alt="在想" /><br /><b>在想</b><br />MOONA 先缓一口气</td>
    <td align="center"><img src="assets/desk-companion/screens/answering.webp" width="160" alt="回答" /><br /><b>回答</b><br />短短几句，读给你听</td>
    <td align="center"><img src="assets/desk-companion/screens/asleep.webp" width="160" alt="息屏" /><br /><b>息屏</b><br />时间和今晚的月亮</td>
  </tr>
  <tr>
    <td align="center"><img src="assets/desk-companion/screens/tarot-shuffle.webp" width="160" alt="洗牌" /><br /><b>洗牌</b><br />握住它，或者摇一摇</td>
    <td align="center"><img src="assets/desk-companion/screens/tarot-reveal.webp" width="160" alt="翻牌" /><br /><b>翻牌</b><br />牌面翻过来</td>
    <td align="center"><img src="assets/desk-companion/screens/sky.webp" width="160" alt="今晚的星空" /><br /><b>今晚的星空</b><br />黄道十二宫沿着圆边排开</td>
    <td align="center"><img src="assets/desk-companion/screens/book-of-night.webp" width="160" alt="星夜之书" /><br /><b>星夜之书</b><br />转动圆边挑一个章节</td>
    <td align="center"><img src="assets/desk-companion/screens/journal.webp" width="160" alt="手记" /><br /><b>手记</b><br />说说今天过得怎样</td>
  </tr>
</table>

每个画面都是为圆形设计的：短标签沿着弧线走，进度绕着圆边走，长一点的内容由 MOONA 读出来，而不是挤满整块屏。

## 怎么做

![概念模型：放在底座上的样子、四个方向的视图和全部零件](assets/desk-companion/3d-views.jpg)

- **脸：** 微雪 ESP32-S3-Touch-AMOLED-1.75 开发板，466 × 466 圆形触摸 AMOLED，双麦克风带回声消除，带音频编解码芯片。
- **身体：** 打印的硬骨架，外面浇铸一层乳白色软硅胶。
- **声音：** 一个 8 Ω 小喇叭，从背面的出音孔出声。
- **供电：** 一块锂电池，通过磁吸底座上的 pogo-pin 充电，底座用 USB-C 供电。

![设计草图：侧面剖面、正面和背面，以及屏幕状态](assets/desk-companion/design-sheet.jpg)

## 你的声音

唤醒词在设备上识别。醒来之后，你说的话会发到 MOONA 的服务器和语音识别服务，转成文字并得到回答，和在网页上打字聊天一样。设备上的 MOONA 和网页上的是同一个。网页版现在如何处理你的文字，见[数据与隐私](docs/data-and-privacy.md)。

---

屏幕上的光球改编自 nimitz 的 **Ether**（CC BY-NC-SA 3.0）；塔罗牌面来自 1909 年的 Rider–Waite–Smith 牌。详见[致谢与权利](ATTRIBUTION.md)。
