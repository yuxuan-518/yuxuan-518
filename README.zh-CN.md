<h1>你好，我是熊少轩 👋<img align="right" src="assets/profile-tagline-zh.svg" alt="嵌入式系统 · 传感器 · 软件开发" width="300" height="40"></h1>

[English](https://github.com/yuxuan-518/yuxuan-518#readme)

## 项目

### [压电地砖——脚步能量采集](https://github.com/yuxuan-518/piezoelectric-floor-tile)

<table>
<tr>
<td width="70%" valign="top">

<p>我研究了<strong>怎样通过地砖结构把脚步运动传递给压电片，并储存产生的电能。</strong> 我们从复现一篇已发表的设计开始。当胶棒接触件在我们的实物中变形并损伤压电片后，研究问题变得更具体：<strong>怎样在保护压电片的同时，让机械激励更加稳定？</strong></p>

<p><strong>设计过程：</strong> 我们先用海绵替换胶棒接触件，再开发弹簧与撞击物组成的模块，探索脱离和重复接触。第二代结构的输出波动促使我们进一步采用中心冲式机构，先压缩弹簧储能，再通过机械触发释放。<strong>每次改进都来自对上一代结构的实际测试，以及对实测行为与预期差异的分析。</strong></p>

<p><em>技术说明：仓库保留了三代结构、CAD 网格、用于 V2 脱离与再次撞击分析的 Python 模型，以及电容充电数据。在各 100 次的单片结构比较中，V3 单步平均储能为 72.48 μJ，V1 衍生基线为 11.63 μJ。6.23 倍反映测试踩踏条件下的储能比；实验未测量机械输入功。</em></p>

<p><strong>我的贡献：</strong> 我主导研究思路、方法和整体分析，负责早期电路工作及 V1/V2 测量，主导 V2 机构开发、Python 仿真和弹簧参数选择，并修订、核查物理模型。队友独立采集 V3 数据后，我负责审核、完整分析和制图。我还确定了论文整体结构，并以第一作者身份将初稿修订为最终稿。</p>

<p><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#design-evolution">结构演变</a> · <a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#ab-experiments">实验与数据</a> · <a href="https://github.com/yuxuan-518/piezoelectric-floor-tile/blob/main/CREDITS.md">团队分工</a></p>

</td>
<td width="30%" valign="top" align="center">

<p align="center"><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#readme"><img src="https://raw.githubusercontent.com/yuxuan-518/piezoelectric-floor-tile/main/assets/images/v3/assembled-1.jpg" alt="V3 · 组装后的原型" width="100%"></a><br><sub>V3 · 组装后的原型</sub></p>

<p align="center"><a href="https://github.com/yuxuan-518/piezoelectric-floor-tile#readme"><img src="https://raw.githubusercontent.com/yuxuan-518/piezoelectric-floor-tile/main/assets/images/v3/IMG_7800.jpg" alt="V3 · 机构零部件" width="100%"></a><br><sub>V3 · 机构零部件</sub></p>

</td>
</tr>
</table>

### [双 MPU6050 姿态反馈原型](https://github.com/yuxuan-518/carpal-tunnel-detection)

<table width="100%">
<tr aria-hidden="true"></tr>
<tr>
<td>

<p align="center"><a href="https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo"><img src="https://raw.githubusercontent.com/yuxuan-518/yuxuan-518/e76867bf0c30a2567fa8998bc958fcdc9c98134d/assets/mpu6050-prototype-banner-dark.png" alt="双 MPU6050 实物原型 · Arduino Uno 与 LED 反馈电路" width="92%"></a><br><sub>双 MPU6050 实物原型 · Arduino Uno 与 LED 反馈电路</sub></p>


<p>在 <strong>Cooper Union Summer STEM</strong> 期间，我留意到长时间使用电脑后手腕会不舒服，于是查阅了腕管综合征的资料，并探索<strong>怎样用一个简单的可穿戴原型，帮助使用者留意用电脑时的手腕姿势。</strong> <a href="https://www.nhs.uk/conditions/carpal-tunnel-syndrome/">NHS 症状与风险因素介绍</a></p>

<p><strong>设计思路：</strong>我们把宽泛的健康关注点收窄到一种原型可以观察的动作：手相对于前臂向上或向下弯曲。我们尝试在手部和前臂各放置一个动作传感器，并通过反馈提醒佩戴者留意手腕姿势。这样，最初的健康问题就变成了一个可以动手制作和探索的具体设计。</p>

<p><em>技术说明：原型使用两个 MPU6050 传感器比较动作数据，并通过 LED 提供反馈。</em></p>

<p><strong>我的贡献：</strong>我提出了双传感器设计并编写最初的 MPU6050 代码，也探索了向量计算和数据处理，并参与早期串口输出与反馈模块的编写。<a href="https://github.com/yuxuan-518/carpal-tunnel-detection/blob/main/README.zh-CN.md#团队分工">查看提交与团队分工</a></p>

<p><a href="https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo">实物与演示</a> · <a href="https://github.com/yuxuan-518/carpal-tunnel-detection#why-two-mpu6050-sensors">设计思路</a> · <a href="https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions">团队分工</a></p>

</td>
</tr>
</table>

### [小猫自动喂粮系统](https://github.com/yuxuan-518/automatic-cat-feeder)

<table width="100%">
<tr>
<td width="70%" valign="top">

<p>在 Alba Studio，我为一台自动喂粮原型设计了电机控制系统。原型能储存干猫粮，并把猫粮送入托盘。我研究了<strong>装入猫粮后，不同电机能否带动下粮机构。</strong></p>

<p><strong>设计过程。</strong>最初的实物测试发现，猫粮容易在料斗出口附近卡住或漏出。改进后的料斗采用 50 cm² 的出口，并调整了导流路径。第一版 NEMA17 电机带载时扭矩不足，我随后测试了能带动下粮机构的高扭矩电机。新电机约重 5 kg，我们把它与主体分开布置，以降低倾倒风险。</p>

<p><em>技术说明。仓库收录了 STEP 装配模型、两套用于 Mega 2560 的独立 AVR C 工程，以及实物和电机测试录像。第二版控制器使用 CL86Y-V20 驱动器，在起停时逐步调整脉冲频率。</em></p>

<p><strong>我的贡献。</strong>我开发了两版电机控制程序，并负责电气与电机测试。第一版用独立定时器输出脉冲，通过串口控制两个 NEMA17 通道。第二版加入加速、减速、受控换向和可重复的单次测试流程。我也记录了两版的接线、驱动设置和控制行为。</p>

<p><a href="https://github.com/yuxuan-518/automatic-cat-feeder#physical-prototype-and-mechanism-animations">实物与结构</a> · <a href="https://github.com/yuxuan-518/automatic-cat-feeder/blob/main/docs/motor-and-automation.md">电机与自动化</a> · <a href="https://github.com/yuxuan-518/automatic-cat-feeder#contributors">团队分工</a></p>

</td>
<td width="30%" valign="top" align="center">

<p align="center"><a href="https://github.com/yuxuan-518/automatic-cat-feeder#cad-animations"><img src="https://raw.githubusercontent.com/yuxuan-518/automatic-cat-feeder/main/assets/images/assembly-animation.gif" alt="整机装配与料斗" width="90%"></a><br><sub>整机装配与料斗</sub></p>

<p align="center"><a href="https://github.com/yuxuan-518/automatic-cat-feeder#cad-animations"><img src="https://raw.githubusercontent.com/yuxuan-518/automatic-cat-feeder/main/assets/images/underside-animation.gif" alt="底部结构与下粮机构" width="90%"></a><br><sub>底部结构与下粮机构</sub></p>

</td>
</tr>
</table>

### [后院里的两只小猫](https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/README.zh-CN.md)

<table width="100%">
<tr aria-hidden="true"></tr>
<tr>
<td width="34%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/README.zh-CN.md"><img src="https://github.com/yuxuan-518/kitten-temperature-monitor/raw/main/assets/prototype-overview.jpg" alt="幼猫休息区原型，包括监测电路、液晶屏和通风风扇" width="100%" align="top"></a><br><sub>我们一起为小猫布置的休息箱</sub><br><br>
<a href="https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/README.zh-CN.md"><img src="https://github.com/yuxuan-518/kitten-temperature-monitor/raw/main/assets/kittens-resting.jpg" alt="两只小猫依偎在休息箱的毯子上" width="100%" align="top"></a><br><sub>挤在一起休息的两只小猫</sub>

</td>
<td width="66%" valign="top">

<p>那天晚上，我正准备送同学回家，忽然听见后院传来很响的喵喵声。我和朋友循着声音找过去，发现两只小猫躺在地上，看起来像是被遗弃了。其中一只特别瘦，天气又冷，身上还有虫子在爬。我当时很慌，马上和朋友把它们带回家，烧水给它们擦身子、清理虫子，再冲奶粉喂它们。</p>

<p>我们三个人很快分了工：一个朋友给小猫清理身体、喂奶，另一个给箱子开口，铺好垫子和被子，我就在旁边写程序、接线。<strong>我用自己在 Arduino IDE 中已有的代码库，花了约一个小时，独立完成程序和接线。</strong>屏幕可以显示休息区周围的空气温湿度，温度异常时发出提示，我还加了一个电风扇通风。</p>

<p>之后，我们轮流照顾它们。我负责半夜十二点和凌晨三点的喂奶，喂完再睡；同学早上六点起床，七点左右过来接班。那几天，喂奶、守着它们、等下一个人来接班，成了我们共同的日常。</p>

<p>其中一只小猫在三四天后没能活下来。另一只现在还和我生活在一起。它有小脑发育不良，走路摇摇晃晃的，但活了下来，现在过得很好。</p>

<p><strong>这次经历让我很具体地感受到，自己学过的东西能在生活里派上用场。</strong>我写代码的时候，朋友就在旁边喂奶、铺箱子。我们一起熬夜、分工、接班，也因此更亲近了。我想把这个项目放在这里，记下当时我们怎样用各自能做的事，去照顾眼前的两只小猫。</p>

<p><a href="https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/README.zh-CN.md">项目与实物照片</a> · <a href="https://github.com/yuxuan-518/kitten-temperature-monitor/blob/main/firmware/KittenMonitor/KittenMonitor.ino">源代码</a></p>

</td>
</tr>
</table>

### [ATmega2560——嵌入式基础学习](https://github.com/yuxuan-518/atmega2560-embedded-foundations)

<table width="100%">
<tr>
<td>

在 Cooper Union 的六周暑期 STEM 项目结束后，我意识到自己需要更多时间梳理嵌入式开发的基础。在浏览 Cornell 的 ECE 课程体系时，ECE 4760 中的鸟鸣合成、数字高尔顿板和反馈控制项目吸引了我。**为了在十二年级继续深入这些内容，我开始探索：怎样通过一系列渐进练习，把零散的知识连接成自己能够理解和运用的体系？**

**学习过程：**我以 ECE 4760 所需的能力为参照，借助 GPT 将目标拆成适合 ATmega2560 的基础练习。从 LED、按钮和寄存器操作开始，逐步加入定时器、中断、串口、传感器和运动控制，最后组织成综合系统。**学习重点也逐渐从实现单个功能，转向理解多个模块怎样协同运行，以及它们为什么会互相影响。**

*技术说明：仓库使用寄存器级 AVR C 和 PlatformIO，保留了从 GPIO 到通信、执行器控制与系统集成的 38 个工程目录。*

**我的贡献：**我独立搜索资料、阅读数据手册并尝试编写第一版代码，在部分练习中重新手写模块以复习原理。GPT 协助解释概念、审查代码和讨论排错；对于不理解的修改，我会继续追问原因，并回到资料与代码中核对。仓库包含这些审查和讨论之后的修改。

[学习动机与路线](https://github.com/yuxuan-518/atmega2560-embedded-foundations/blob/main/README.zh-CN.md#为什么开始) · [代表项目与排错经历](https://github.com/yuxuan-518/atmega2560-embedded-foundations/blob/main/README.zh-CN.md#三个推荐阅读的项目) · [源代码](https://github.com/yuxuan-518/atmega2560-embedded-foundations/tree/main/code)

</td>
</tr>
</table>

### [Kesty — 学习管理应用](https://github.com/yuxuan-518/kesty-support)

<table width="100%">
<tr aria-hidden="true"></tr>
<tr>
<td>

申请季、考试准备和研究任务常常同时占用学生的时间。像完成 Common App 申请或写一篇论文这样的大目标，并不是一个待办事项，而是由许多不同的部分组成。

**设计思路：**Kesty 让用户把一个长期目标拆成具体的小任务，再分配到不同的日期。例如，Common App 目标可以拆成主文书、补充文书和 Additional Information；课外项目可以拆成上传代码、组装原型和制作展示网站；论文目标可以拆成整理数据、撰写不同部分和推导公式。**核心想法是让每天的任务都能连回长期目标，帮助用户安排眼前的工作，同时看清它们如何推动整体进展。**

*技术说明：Kesty 是一款 SwiftUI 原生 iOS 应用，使用 Codable 数据模型在设备本地保存资料、任务和计划。*

**我的贡献：**我负责应用整体架构、本地数据组织，以及长期目标与每日任务之间的结构设计。GPT 根据我提出的设计和需求，辅助编写 Swift 与 SwiftUI 代码。

**[在 App Store 下载](https://apps.apple.com/us/app/kesty/id6760517321)** · [源代码与演示](https://github.com/yuxuan-518/kesty-support#readme)

</td>
</tr>
</table>

### [数据可视化与叙事 — Cooper Union](https://github.com/yuxuan-518/cooper-union-data-visualization/blob/main/README.zh-CN.md)

<table width="100%">
<tr>
<td>

在 **2024 年 Cooper Union STEM Saturdays 的 Inventor’s Lab: Data Visualization 课程**中，我练习把表格整理成听众能够理解的图表。期末项目从年龄、学历和性别三个角度，比较各群体中有工作的人所占的比例。**通过图表，读者可以直接看到群体差异和时间变化，不必逐行阅读原始数据。**

**课程实践与学习收获：**材料还包括 Titanic 乘客统计、硬币质量分布、两种图表形式的比较，以及节目选择建议。我练习了整理数据、计算描述统计量、根据问题选择图表，并通过双语讲稿和合作演示向听众解释比较结果。

*技术说明：期末成果包括 7 个工作表的 Excel 分析、22 页演示文稿和中英双语排练稿。各项目页面直接展示图表预览与简短说明。*

[期末项目图表与讲解](https://github.com/yuxuan-518/cooper-union-data-visualization/blob/main/final-project/employment-analysis/README.zh-CN.md) · [课堂练习](https://github.com/yuxuan-518/cooper-union-data-visualization/blob/main/README.zh-CN.md#课堂练习) · [课程学习收获](https://github.com/yuxuan-518/cooper-union-data-visualization/blob/main/README.zh-CN.md#我在这门课中练习了什么)

</td>
</tr>
</table>

---

仓库中记录了原型及开发过程中的探索。各项目 README 介绍了当前功能、局限和合作成员。

## 关于我

```javascript
const shaoxuan = {
  interests: ["嵌入式系统", "传感器", "应用开发"],
  learning: ["C / AVR C", "Swift / SwiftUI"],
  hardware: ["Arduino Uno", "ATmega328P", "MPU6050"],
  approach: "制作原型，实际测试，从结果中学习"
};
```

### 如果您已经阅读了上面的内容，我想说一声非常感谢，非常感谢您浏览了一个小小的高中生折腾出的一些小小的初级项目。感谢您的关注和耐心阅读。接下来，我想谈一谈我的另一面。

<a name="my-family"></a>

---

<details>
<summary><strong>我的家人</strong></summary>

在主文书里，或许您已经了解了我的家庭情况。不过在这里，我想给您看看我现在的家。

[花椒](#花椒-peper) · [荔枝](#荔枝-lychee) · [米团](#米团-rice-ball) · [完整相册](https://github.com/yuxuan-518/cat-family-album)

#### 花椒 Peper

这个小猫叫花椒，是我收养的第一只小猫。您可以看到，他是一个大胖子。但您可能想不到，他的脾气和体重一样大，特别是别人摸他屁股的时候！不过，他也有很多很萌的时候，比如这些。

<table width="560">
<tr>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045526_1547_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045526_1547_4.jpg" alt="花椒：大胖子本猫" width="160"></a>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045806_1615_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045806_1615_4.jpg" alt="在窗台上看着我的花椒" width="160"></a>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045329_1504_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045329_1504_4.jpg" alt="也有乖乖让人抱的时候" width="160"></a>

</td>
</tr>
</table>

花椒是一只非常非常傲娇的小猫咪。我住在地下室，床边和书桌附近的墙上都有小窗子，可以看到外面的地面。只要我回房间，或者从房间出来，他就会跳上对应的窗台。

<details>
<summary>▶ 花椒的窗台日常 · 25 秒</summary>

https://github.com/user-attachments/assets/1713b100-bc6f-4676-9772-10889fd9ed70

</details>

<table width="100%">
<tr>
<td width="38%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045646_1583_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045646_1583_4.jpg" alt="枕头已经是他的专属位置了" width="280"></a>

</td>
<td width="62%" valign="middle">

他要抱抱的方式也很奇特。他会先跑到床上，停在离我大约一个半手臂远的地方——刚好是我躺着伸手够不到、必须起身才能抱到他的距离。然后，他会发出一声“mia”，半蹲在那里看看我，又看看窗台，就像在说：“你快过来抱我，不然我就要上窗台了。”

每到这个时候，我就会起身把他抱进怀里。但抱上五六分钟，他又要走了。我把他放开，他就自己跑去我床上的另一个枕头睡觉。那个枕头已经是他的专属枕头了，每晚都要在那里陪我进入梦乡。

真是一个傲娇的小猫。

</td>
</tr>
</table>

[↑ 回到栏目标题](#my-family)

#### 荔枝 Lychee

然后这一只，他叫荔枝，是我从小养到大的小猫咪！您看看，他刚到家的时候只有这么大！！

<table width="560">
<tr>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045818_1620_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045818_1620_4.jpg" alt="荔枝刚到家的时候" width="160"></a>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045855_1637_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045855_1637_4.jpg" alt="那时候真的只有这么小" width="160"></a>

</td>
<td width="33%" valign="top" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050131_1719_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050131_1719_4.jpg" alt="现在的荔枝" width="160"></a>

</td>
</tr>
</table>

好可爱啊！！！

当然，他刚来家里的时候，可把花椒气坏了。为了照顾花椒的情绪，我搬着床垫，在房间外面陪他睡了两三个星期。这样，小荔枝就可以安安静静地待在我的房间里喝奶、睡觉，不会挨打了。（偷笑）

现在我经常叫荔枝“瘦猴子”。他每天跑来跑去，追着花椒玩，还特别喜欢去招惹花椒那条大毛尾巴。花椒就像一个装高冷的大哥哥，不太愿意理他，只是在旁边看着。

<table width="100%">
<tr>
<td width="28%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045959_1676_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109045959_1676_4.jpg" alt="写代码时，书桌上总少不了他" width="195"></a>

</td>
<td width="72%" valign="middle">

如果说花椒是傲娇，那荔枝简直是“强制爱”的一把好手。每次我在书桌前写功课或者敲代码，他总要跑上来，用小脑袋不停地蹭我的手，打断我。我伸手摸摸他，他就开始舔我，我也会用额头和他贴贴。

但他的规矩可多了。他想粘我的时候，就会一直蹭、一直舔，不让我干别的事情；可如果是我想抱抱他，或者趁他玩的时候凑过去亲亲他，他又会拿臭臭的小爪子顶住我的脸。

只允许他贴着我，不允许我去贴着他，这个小猫咪！

</td>
</tr>
</table>

对了，每次睡觉前，荔枝都会跑到床上，一边踩奶，一边嘬嘬嘬我毛茸茸的被子。给您看一个纯享版吧！

<details>
<summary>▶ 荔枝睡前踩奶 · 20 秒</summary>

https://github.com/user-attachments/assets/17ef30fd-edfe-4795-85ad-dd1f619788cb

</details>

[↑ 回到栏目标题](#my-family)

#### 米团 Rice Ball

<table width="100%">
<tr>
<td width="50%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050230_1742_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050230_1742_4.jpg" alt="米团，家里最小的一只" width="260"></a>

</td>
<td width="50%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050127_1717_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050127_1717_4.jpg" alt="花椒和米团：“大卡车”和小不点" width="260"></a>

</td>
</tr>
<tr>
<td colspan="2">

最后是这一只啦。

您应该已经看到上面那个“后院里的两只小猫”的项目了吧？他就是其中的一只，叫米团。另一只叫芝麻，很遗憾，芝麻后来没能活下来。但米团留下来了，也已经快快乐乐地长大了。

米团和花椒都是长毛猫，从十月份开始，他们两个就经常黏在一起。不过花椒对米团来说实在太巨大了，站在他面前就像一辆大卡车！

</td>
</tr>
</table>

米团也是家里外号最多的小猫：摇摆猫、粑粑猫、biabiami、米糖……都是他。

叫他“摇摆猫”，是因为他小时候没有发育好，走路一直摇摇晃晃的，有时走着走着还会自己摔一跤。不过，这也没耽误他到处玩、找我们撒娇。

“粑粑猫”这个名字，就有一点点臭臭的来历了。他在猫砂盆里刨砂时，有时也会站不稳摔倒，把自己弄得一身脏。我就又得把他抱出来，给他擦干净。叫着叫着，“粑粑猫”又变成了“粑粑咪”，再变成“biabiami”。至于“米糖”，也是从“米团”慢慢叫出来的。这个小猫，一个名字哪里够用。（偷笑）

<table width="100%">
<tr>
<td width="50%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050047_1699_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050047_1699_4.jpg" alt="从小就是个大嗓门" width="260"></a>

</td>
<td width="50%" valign="middle" align="center">

<a href="https://github.com/yuxuan-518/cat-family-album/blob/main/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050219_1737_4.jpg"><img src="https://raw.githubusercontent.com/yuxuan-518/cat-family-album/a28e818b342116926e7c960e7df64e58d97c022e/photos/%E5%BE%AE%E4%BF%A1%E5%9B%BE%E7%89%87_20261109050219_1737_4.jpg" alt="抱起来以后，就可以贴贴了" width="260"></a>

</td>
</tr>
<tr>
<td colspan="2">

还记得荔枝是怎么粘我的吗？米团又不一样。这个小矮子还没长大，跳不上书桌和床，就站在旁边，扯着嗓子对我喊。别看他小小一只，嗓门可大了，从小就喜欢喊！

每到这个时候，我就把他抱进怀里，或者放到被子上，他就开始跟我打闹了。

</td>
</tr>
</table>

<details>
<summary>▶ 小小一只，朝我走过来 · 4 秒</summary>

https://github.com/user-attachments/assets/f840e4d7-8e97-44b7-9dc4-bd4c76834876

</details>

这三只小猫咪，就是我现在的家人啦。他们三个每天打打闹闹，深夜陪我学习，做饭的时候又凑过来好奇。离开父母、开始独自生活以后，他们给我的日子增添了很多色彩。现在，我也已经离不开他们了。

我真的真的很爱他们！！！

[↑ 回到栏目标题](#my-family)

</details>

---
