<h1>Hi, I'm Shaoxuan 👋<img align="right" src="assets/profile-tagline-en.svg" alt="Embedded systems · Sensors · Software" width="300" height="40"></h1>

[简体中文](https://github.com/yuxuan-518/yuxuan-518/blob/main/README.zh-CN.md)

## Projects

### [Piezoelectric Floor Tile — Footstep Energy Harvesting](https://github.com/yuxuan-518/piezoelectric-floor-tile)

<table>
<tr>
<td width="70%" valign="top">

<p>I investigated <strong>how a floor tile could transfer footstep motion to a piezoelectric disc and store the resulting electrical energy.</strong> We began by replicating a published design. When its glue-stick contacts deformed and damaged discs in our build, the problem became more specific: <strong>How could we protect the disc while delivering a more consistent mechanical input?</strong></p>

<p><strong>Design process:</strong> We replaced the glue contacts with sponge pads, then developed spring–impactor modules to explore separation and repeated contact. Variable responses in that second design led us to a center-punch-style mechanism that stores spring energy before a mechanical trigger releases it. <strong>Each revision grew from testing the previous structure and examining where its behavior differed from our expectations.</strong></p>

<p><em>Technical note: The repository includes three design generations, CAD meshes, a Python model for V2 separation and re-impact, and capacitor-charging measurements. In a single-disc comparison, V3 stored 72.48 μJ per step on average versus 11.63 μJ for the V1-derived baseline (100 steps each). The 6.23 ratio describes stored energy under the tested stepping conditions; mechanical input work was not measured.</em></p>

<p><strong>My contribution:</strong> I led the research idea, methods, and overall analysis, including early circuit work and V1/V2 measurements. I led V2 mechanism development, Python simulation, and spring-parameter selection, and revised and checked the physical model. After my teammates independently collected the V3 data, I reviewed and analyzed it and prepared the figures. I established the manuscript structure and revised the first draft into the final manuscript as first author.</p>

<p><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#design-evolution">Design evolution</a> · <a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#ab-experiments">Experiments and data</a> · <a href="https://github.com/yuxuan-518/piezoelectric-floor-tile/blob/main/CREDITS.md">Team contributions</a></p>

</td>
<td width="30%" valign="top" align="center">

<p align="center"><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#readme"><img src="https://raw.githubusercontent.com/yuxuan-518/piezoelectric-floor-tile/main/assets/images/v3/assembled-1.jpg" alt="V3 · Assembled prototype" width="100%"></a><br><sub>V3 · Assembled prototype</sub></p>

<p align="center"><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#readme"><img src="https://raw.githubusercontent.com/yuxuan-518/piezoelectric-floor-tile/main/assets/images/v3/IMG_7800.jpg" alt="V3 · Mechanism components" width="100%"></a><br><sub>V3 · Mechanism components</sub></p>

</td>
</tr>
</table>

### [Dual-MPU6050 Posture Feedback Prototype](https://github.com/yuxuan-518/carpal-tunnel-detection)

<table width="100%">
<tr>
<td align="center">

<p align="center"><a href="https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo"><img src="https://raw.githubusercontent.com/yuxuan-518/yuxuan-518/e76867bf0c30a2567fa8998bc958fcdc9c98134d/assets/mpu6050-prototype-banner-dark.png" alt="Dual-MPU6050 prototype · Arduino Uno and LED feedback" width="92%"></a><br><sub>Dual-MPU6050 prototype · Arduino Uno and LED feedback</sub></p>

</td>
</tr>
<tr>
<td>

<p>During <strong>Cooper Union Summer STEM</strong>, I looked into carpal tunnel syndrome after noticing wrist discomfort from long hours at a computer. I explored <strong>whether a simple wearable could help people notice their wrist posture while using a computer.</strong> <a href="https://www.nhs.uk/conditions/carpal-tunnel-syndrome/">NHS overview</a></p>

<p><strong>Design process:</strong> We narrowed the broad health concern to one behavior a prototype could respond to: the hand bending up or down relative to the forearm. We explored placing one motion sensor on the hand and another on the forearm, then using feedback to draw attention to wrist posture. This gave us a concrete idea to build and investigate.</p>

<p><em>Technical note: The prototype compares motion data from two MPU6050 sensors and provides LED feedback.</em></p>

<p><strong>My contribution:</strong> I proposed the dual-sensor design and wrote its initial MPU6050 code. I also explored vector calculations and data processing, and contributed early serial-output and feedback modules. <a href="https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions">Contribution history</a></p>

<p><a href="https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo">Photo &amp; demo</a> · <a href="https://github.com/yuxuan-518/carpal-tunnel-detection#why-two-mpu6050-sensors">Design rationale</a> · <a href="https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions">Team contributions</a></p>

</td>
</tr>
</table>

### [Automatic Cat Feeder](https://github.com/yuxuan-518/automatic-cat-feeder)

<table width="100%">
<tr>
<td width="70%" valign="top">

<p>At Alba Studio, I designed the motor controls for a prototype that stores dry cat food and dispenses it into a tray. I investigated <strong>how much the choice of motor mattered when the mechanism was loaded with kibble.</strong></p>

<p><strong>Design process.</strong> Early tests showed that kibble jammed and leaked near the hopper outlet. The revised hopper used a 50 cm² outlet and a reshaped guide path. The first NEMA17 motor struggled under the load, so I tested a higher-torque motor that could drive the mechanism. The replacement weighed about 5 kg, so we kept it separate from the feeder frame to reduce the risk of tipping.</p>

<p><em>Technical note. The repository includes the STEP assembly, two standalone AVR C projects for the Mega 2560, and recordings of the physical prototype and motor test. The second controller uses a CL86Y-V20 driver and ramps the pulse frequency when starting and stopping.</em></p>

<p><strong>My contribution.</strong> I developed both motor controllers and carried out electrical and motor testing. I set up independent timer outputs and serial control for the NEMA17 version, then added acceleration, deceleration, controlled reversal, and a repeatable test run for the higher-torque setup. I documented the wiring, driver settings, and behavior of each version.</p>

<p><a href="https://github.com/yuxuan-518/automatic-cat-feeder#physical-prototype-and-mechanism-animations">Prototype and design</a> · <a href="https://github.com/yuxuan-518/automatic-cat-feeder/blob/main/docs/motor-and-automation.md">Motor and automation</a> · <a href="https://github.com/yuxuan-518/automatic-cat-feeder#contributors">Team contributions</a></p>

</td>
<td width="30%" valign="top" align="center">

<p align="center"><a href="https://github.com/yuxuan-518/automatic-cat-feeder#cad-animations"><img src="https://raw.githubusercontent.com/yuxuan-518/automatic-cat-feeder/main/assets/images/assembly-animation.gif" alt="Feeder assembly and hopper" width="90%"></a><br><sub>Feeder assembly and hopper</sub></p>

<p align="center"><a href="https://github.com/yuxuan-518/automatic-cat-feeder#cad-animations"><img src="https://raw.githubusercontent.com/yuxuan-518/automatic-cat-feeder/main/assets/images/underside-animation.gif" alt="Underside and dispensing mechanism" width="90%"></a><br><sub>Underside and dispensing mechanism</sub></p>

</td>
</tr>
</table>

### [Two Kittens in the Backyard](https://github.com/yuxuan-518/kitten-temperature-monitor)

<table width="100%">
<tr>
<td width="34%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/kitten-temperature-monitor#readme"><img src="https://github.com/yuxuan-518/kitten-temperature-monitor/raw/main/assets/prototype-overview.jpg" alt="Kitten resting-area prototype with monitoring electronics, LCD and a ventilation fan" width="100%" align="top"></a><br><sub>The resting box we put together for the kittens</sub><br><br>
<a href="https://github.com/yuxuan-518/kitten-temperature-monitor#readme"><img src="https://github.com/yuxuan-518/kitten-temperature-monitor/raw/main/assets/kittens-resting.jpg" alt="Two young kittens resting together on blankets inside the enclosure" width="100%" align="top"></a><br><sub>The two kittens resting together</sub>

</td>
<td width="66%" valign="top">

<p>One evening, as I was about to walk a classmate home, we heard loud meowing from the backyard. We followed the sound and found two kittens lying on the ground. They seemed to have been abandoned. One was very thin, the weather was cold, and insects were crawling on them. I panicked. We hurried back inside with them, warmed water to wipe their bodies and remove the insects, and prepared kitten formula.</p>

<p>There were three of us, and we divided up the work. While one friend cleaned and fed a kitten and another cut an opening in a box and lined it with soft bedding, I worked on the code and wiring. <strong>Using code from my existing Arduino IDE library, I independently completed the programming and wiring in about an hour.</strong> The device displayed the air temperature and humidity around their resting area and gave temperature alerts. I also added a fan for ventilation.</p>

<p>Afterward, we took turns looking after them. I fed them at midnight and again at 3 a.m., then went to sleep. My classmate got up at 6 and came over around 7 to take the next shift. That became the work we shared: feeding, watching, and making sure someone was there to take over.</p>

<p>One kitten died three or four days later. The other is still with me. It has cerebellar hypoplasia and walks unsteadily, but it is alive and doing well.</p>

<p><strong>What stays with me is how directly the things I had learned became useful.</strong> I was writing code while my friends were feeding the kittens and preparing their box. The late nights and handovers brought the three of us closer, too. This project belongs alongside my other work because it records a time when we had a problem in front of us and used what we had to help.</p>

<p><a href="https://github.com/yuxuan-518/kitten-temperature-monitor#readme">Project and photos</a> · <a href="https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/firmware/KittenMonitor/KittenMonitor.ino">Source code</a></p>

</td>
</tr>
</table>

### [ATmega2560 — Embedded Foundations](https://github.com/yuxuan-518/atmega2560-embedded-foundations)

After Cooper Union's six-week Summer STEM program, I realized I needed more time to organize my understanding of embedded development. While exploring Cornell's ECE curriculum, I discovered ECE 4760 and was drawn to its birdsong synthesis, digital Galton board, and feedback-control projects. **To prepare for studying this material more deeply during twelfth grade, I began asking: How could a series of progressive exercises connect scattered knowledge into a foundation I could understand and use?**

**Learning process:** Using the skills needed for ECE 4760 as a reference, I worked with GPT to break the goals into foundational ATmega2560 exercises. Starting with LEDs, buttons, and register operations, I gradually added timers, interrupts, serial communication, sensors, and motion control before bringing them together into an integrated system. **My focus gradually expanded from implementing individual functions to understanding how modules work together and why they can interfere with one another.**

*Technical note: The repository uses register-level AVR C and PlatformIO, preserving 38 project directories spanning GPIO, communication, actuator control, and system integration.*

**My contribution:** I independently searched for resources, read datasheets, and attempted the first version of the code. In some exercises, I rewrote modules by hand to revisit the principles. GPT helped explain concepts, review code, and discuss debugging. When I did not understand a proposed change, I asked further questions and returned to the documentation and code to check the explanation. The repository includes revisions made after these reviews and discussions.

[Motivation and learning progression](https://github.com/yuxuan-518/atmega2560-embedded-foundations#why-i-started) · [Selected projects and debugging](https://github.com/yuxuan-518/atmega2560-embedded-foundations#three-projects-to-explore) · [Source code](https://github.com/yuxuan-518/atmega2560-embedded-foundations/tree/main/code)

### [Kesty — Study Management App](https://github.com/yuxuan-518/kesty-support)

During application season, exam preparation, and research, students often have several large commitments competing for their time. **A goal like completing the Common App or writing a research paper is made up of many smaller pieces, not one checkbox.**

**Design idea:** Kesty lets users turn a large goal into smaller tasks and spread them across individual days. For example, a Common App goal could include the personal statement, supplemental essays, and Additional Information. An extracurricular project could include pushing code, assembling a prototype, and building a showcase website. A research paper could include organizing data, drafting sections, and deriving formulas. **The central idea is to connect each day’s work to the larger goal, so users can plan what to do now while keeping the overall project in view.**

*Technical note: Kesty is a native iOS app built with Swift and SwiftUI. It uses Codable models and `UserDefaults` for local data storage; cloud synchronization is not currently implemented.*

**My contribution:** I defined the app’s architecture, local data organization, and the structure connecting long-term goals with daily tasks. GPT assisted with writing the Swift and SwiftUI code based on the design and requirements I defined.

**[Download on the App Store](https://apps.apple.com/us/app/kesty/id6760517321)** · [Source code and demo](https://github.com/yuxuan-518/kesty-support#readme)

### [Data Visualization and Storytelling — Cooper Union](https://github.com/yuxuan-518/cooper-union-data-visualization)

During **Cooper Union STEM Saturdays: Inventor’s Lab — Data Visualization (2024)**, I practiced turning tables into charts that an audience could understand. The final project compares the share of people employed across age groups, education levels, and gender. **The charts make group differences and changes over time visible without asking viewers to read the raw data row by row.**

**Course work and learning:** The collection also includes Titanic passenger summaries, penny-mass distributions, a comparison of two chart formats, and program-selection recommendations. I practiced organizing data, calculating descriptive statistics, choosing charts for different questions, and explaining comparisons through bilingual speaking notes and a collaborative presentation.

*Technical note: The final project includes a seven-worksheet Excel analysis, a 22-slide presentation, and Chinese/English rehearsal notes. Project pages display chart previews with short explanations.*

[Final project: charts and explanation](https://github.com/yuxuan-518/cooper-union-data-visualization/tree/main/final-project/employment-analysis#readme) · [Classroom exercises](https://github.com/yuxuan-518/cooper-union-data-visualization#classroom-exercises) · [Course learning](https://github.com/yuxuan-518/cooper-union-data-visualization#what-i-practiced-during-the-course)

---

## About me

```javascript
const shaoxuan = {
  interests: ["Embedded systems", "Sensors", "App development"],
  learning: ["C / AVR C", "Swift / SwiftUI"],
  hardware: ["Arduino Uno", "ATmega328P", "MPU6050"],
  approach: "Build a prototype, test it, and learn from the results"
};
```

### If you have read this far, thank you—really—for spending time with the little beginner projects that this high-school student has been tinkering with. Thank you for your interest and patience. Below, I would like to show you another side of me.

<a name="my-family"></a>

---

<details>
<summary><strong>My family · 我的家人</strong></summary>

You may already know about my family circumstances from my personal statement. Here, though, I would like to show you what my home looks like now.

[Sichuan Pepper](#sichuan-pepper-花椒) · [Lychee](#lychee-荔枝) · [Rice Ball](#rice-ball-米团) · [Full photo album](https://github.com/yuxuan-518/cat-family-album)

#### Sichuan Pepper 花椒

This is Sichuan Pepper, the first cat I adopted. As you can see, he is a big, fluffy boy. What you might not guess is that his temper is just as big—especially when someone touches his backside! But he has plenty of adorable moments, too. Here are a few.

<table width="560">
<tr>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045526_1547_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045526_1547_4.jpg" alt="Sichuan Pepper, in all his fluffy glory" width="160"></a><br><sub>Sichuan Pepper, in all his fluffy glory</sub>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045806_1615_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045806_1615_4.jpg" alt="Watching me from the windowsill" width="160"></a><br><sub>Watching me from the windowsill</sub>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045329_1504_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045329_1504_4.jpg" alt="Sometimes he does let me hold him" width="160"></a><br><sub>Sometimes he does let me hold him</sub>

</td>
</tr>
</table>

Sichuan Pepper is very, very proud. I live in a basement, with small windows near my bed and desk that look out at ground level. Whenever I come back to my room or leave it, he jumps onto the corresponding windowsill.

<details>
<summary>▶ A little windowsill time with Sichuan Pepper · 25 seconds</summary>

https://github.com/user-attachments/assets/1713b100-bc6f-4676-9772-10889fd9ed70

</details>

<table width="100%">
<tr>
<td width="30%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045646_1583_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045646_1583_4.jpg" alt="That pillow is officially his now" width="220"></a><br><sub>That pillow is officially his now</sub>

</td>
<td width="70%" valign="top">

He also has a very particular way of asking for a cuddle. He first runs onto the bed and stops about one and a half arm lengths away—just far enough that I cannot reach him while lying down and have to sit up to pick him up. Then he gives a little “mia,” half-crouches, looks at me, and looks at the windowsill, as if to say, “Come and get me, or I am going up there.”

So I get up and hold him. Five or six minutes later, he wants to leave again. I let him go, and he makes his way to the other pillow on my bed. That pillow belongs to him now. Every night, he sleeps there beside me.

Such a proud little cat.

</td>
</tr>
</table>

[↑ Back to the family heading](#my-family)

#### Lychee 荔枝

And this is Lychee, whom I have raised since he was tiny! Look how small he was when he first came home!!

<table width="560">
<tr>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045818_1620_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045818_1620_4.jpg" alt="When Lychee first came home" width="160"></a><br><sub>When Lychee first came home</sub>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045855_1637_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045855_1637_4.jpg" alt="He really was this tiny" width="160"></a><br><sub>He really was this tiny</sub>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050131_1719_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050131_1719_4.jpg" alt="Lychee now" width="160"></a><br><sub>Lychee now</sub>

</td>
</tr>
</table>

So cute!!!

Of course, his arrival made Sichuan Pepper very unhappy. To help Sichuan Pepper adjust, I moved a mattress outside my room and slept there with him for two or three weeks. That left little Lychee free to drink his milk and sleep peacefully in my room, without getting swatted. (Hehe.)

Now I often call Lychee my “little monkey.” He runs around all day, chasing Sichuan Pepper and trying to play with that enormous fluffy tail. Sichuan Pepper acts like a very aloof older brother: he mostly watches and pretends not to be interested.

<table width="100%">
<tr>
<td width="30%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045959_1676_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045959_1676_4.jpg" alt="My desk companion while I code" width="220"></a><br><sub>My desk companion while I code</sub>

</td>
<td width="70%" valign="top">

If Sichuan Pepper is proud, Lychee is an expert at demanding affection. Whenever I am doing homework or coding at my desk, he comes up and keeps rubbing his little head against my hand until I stop. I pet him, he licks me, and I sometimes press my forehead gently against his.

But he has rules. When he wants to be close, he rubs and licks and will not let me do anything else. When I want to pick him up or sneak in a kiss while he is playing, he pushes his little stinky paws against my face.

Apparently, he is allowed to cuddle me, but I am not allowed to cuddle him. This cat!

</td>
</tr>
</table>

And every night before bed, he climbs onto the blankets, kneads with his front paws, and suckles on the fuzzy fabric. Here is the uninterrupted version for you!

<details>
<summary>▶ Lychee kneading before bed · 20 seconds</summary>

https://github.com/user-attachments/assets/17ef30fd-edfe-4795-85ad-dd1f619788cb

</details>

[↑ Back to the family heading](#my-family)

#### Rice Ball 米团

<table width="100%">
<tr>
<td width="30%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050230_1742_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050230_1742_4.jpg" alt="Rice Ball, the smallest member of the family" width="100"></a> &nbsp; <a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050127_1717_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050127_1717_4.jpg" alt="Sichuan Pepper and Rice Ball: the truck and the tiny kitten" width="100"></a><br><sub>Rice Ball, the smallest member of the family · Sichuan Pepper and Rice Ball: the truck and the tiny kitten</sub>

</td>
<td width="70%" valign="top">

Last, here is Rice Ball.

You may have seen the project about the two kittens in my backyard above. He is one of those kittens. The other was called Sesame; sadly, Sesame did not survive. Rice Ball stayed with me and has been growing up happily.

Rice Ball and Sichuan Pepper are both long-haired cats, and since October they have often been cuddled up together. Sichuan Pepper is enormous next to him, though—like a truck parked in front of a tiny kitten!

</td>
</tr>
</table>

Rice Ball also has the most nicknames in the house: Wobbly Cat, Poop Cat, biabiami, Rice Candy… all of them mean him.

“Wobbly Cat” comes from the way he walks. He did not develop fully as a kitten, so he is unsteady and sometimes tumbles over. It does not stop him from playing or asking us for attention.

“Poop Cat” has a slightly smellier origin. Sometimes he loses his balance while digging in the litter box and gets himself dirty, so I pick him up and clean him again. That nickname gradually became “baba-mi,” then “biabiami.” “Rice Candy” is another little variation on “Rice Ball.” One name could never be enough for this cat. (Hehe.)

<table width="100%">
<tr>
<td width="30%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050047_1699_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050047_1699_4.jpg" alt="A big voice, right from the beginning" width="100"></a> &nbsp; <a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050219_1737_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050219_1737_4.jpg" alt="Once I pick him up, we can cuddle" width="100"></a><br><sub>A big voice, right from the beginning · Once I pick him up, we can cuddle</sub>

</td>
<td width="70%" valign="top">

Remember how Lychee asks for affection? Rice Ball has his own approach. He is still too small to jump onto my desk or bed, so he stands beside it and shouts for me. He may be tiny, but his voice certainly is not. He has been loud since he was little!

Then I pick him up, hold him in my arms or set him on the blankets, and we start playing.

</td>
</tr>
</table>

<details>
<summary>▶ Tiny Rice Ball coming over to me · 4 seconds</summary>

https://github.com/user-attachments/assets/f840e4d7-8e97-44b7-9dc4-bd4c76834876

</details>

These three cats are my family now. They tumble around together, keep me company while I study late at night, and come over to investigate when I cook. After leaving my parents and beginning to live on my own, they brought so much color into my days. Now I cannot imagine my life without them.

I really, really love them!!!

[↑ Back to the family heading](#my-family)

</details>

---
