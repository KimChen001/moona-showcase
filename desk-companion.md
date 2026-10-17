<p align="center">
  <strong>MOONA Desk Companion</strong><br />
  <em>A small MOONA that waits on your desk.</em>
</p>

<p align="center">
  <a href="README.md">Back to MOONA</a> ·
  <a href="desk-companion.zh-CN.md">中文介绍</a>
</p>

<p align="center"><img src="assets/desk-companion/hero.png" width="420" alt="MOONA Desk Companion: a milk-white silicone orb with a round screen, on its charging dock" /></p>

MOONA lives on the web today. The desk companion gives it a body: a palm-sized orb in soft, milk-white silicone, with a 1.75-inch round AMOLED screen for a face. It wakes when you speak to it, answers out loud, and charges when you set it on its magnetic dock.

**Status: in design.** The pictures on this page are a concept model and screen designs, not photos of a finished device.

## What the round face shows

<table>
  <tr>
    <td align="center"><img src="assets/desk-companion/screens/idle.webp" width="160" alt="Idle" /><br /><b>Idle</b><br />the orb breathes slowly</td>
    <td align="center"><img src="assets/desk-companion/screens/listening.webp" width="160" alt="Listening" /><br /><b>Listening</b><br />a gold ring draws as you speak</td>
    <td align="center"><img src="assets/desk-companion/screens/thinking.webp" width="160" alt="Thinking" /><br /><b>Thinking</b><br />MOONA takes a breath</td>
    <td align="center"><img src="assets/desk-companion/screens/answering.webp" width="160" alt="Answering" /><br /><b>Answering</b><br />short lines, spoken aloud</td>
    <td align="center"><img src="assets/desk-companion/screens/asleep.webp" width="160" alt="Asleep" /><br /><b>Asleep</b><br />the time and tonight&#8217;s Moon</td>
  </tr>
  <tr>
    <td align="center"><img src="assets/desk-companion/screens/tarot-shuffle.webp" width="160" alt="Tarot shuffle" /><br /><b>Tarot shuffle</b><br />hold it, or give it a shake</td>
    <td align="center"><img src="assets/desk-companion/screens/tarot-reveal.webp" width="160" alt="Tarot reveal" /><br /><b>Tarot reveal</b><br />the card turns over</td>
    <td align="center"><img src="assets/desk-companion/screens/sky.webp" width="160" alt="Tonight's sky" /><br /><b>Tonight&#8217;s sky</b><br />the zodiac rides the rim</td>
    <td align="center"><img src="assets/desk-companion/screens/book-of-night.webp" width="160" alt="Book of Night" /><br /><b>Book of Night</b><br />turn the rim to pick a chapter</td>
    <td align="center"><img src="assets/desk-companion/screens/journal.webp" width="160" alt="Journal" /><br /><b>Journal</b><br />say how today went</td>
  </tr>
</table>

Every screen is designed for a circle: short labels follow the curve, progress runs around the rim, and MOONA reads longer text aloud instead of filling the glass.

## How it is built

![The concept model: on its dock, from four sides, and its parts](assets/desk-companion/3d-views.jpg)

- **Face:** a Waveshare ESP32-S3-Touch-AMOLED-1.75 board: a 466 × 466 round touch AMOLED, two microphones with echo cancellation, and an audio codec.
- **Body:** a rigid printed inner frame inside a cast skin of soft, milk-white silicone.
- **Sound:** a small 8 Ω speaker behind a grille on the back.
- **Power:** a LiPo cell, charged through pogo pins on a magnetic dock with a USB-C input.

![Design sketch: side section, front and back, and the screen states](assets/desk-companion/design-sheet.jpg)

## Your voice

The wake word is detected on the device itself. Once it wakes, what you say goes to MOONA's server and a speech-recognition service to be transcribed and answered, as a typed conversation does on the web. The device and the web app are the same MOONA. See [Data and privacy](docs/data-and-privacy.md) for how the web demo handles your words today.

---

The orb on the screen adapts **Ether** by nimitz (CC BY-NC-SA 3.0); the tarot art is the 1909 Rider–Waite–Smith deck. See [Credits and rights](ATTRIBUTION.md).
