# 你好，我是熊少轩 👋

**嵌入式系统 · 传感器 · 软件开发**

[English](https://github.com/yuxuan-518/yuxuan-518#readme)

## 关于我

```javascript
const shaoxuan = {
  interests: ["嵌入式系统", "传感器", "应用开发"],
  learning: ["C / AVR C", "Swift / SwiftUI"],
  hardware: ["Arduino Uno", "ATmega328P", "MPU6050"],
  approach: "制作原型，实际测试，从结果中学习"
};
```

## 项目

### [双 MPU6050 姿态反馈原型](https://github.com/yuxuan-518/carpal-tunnel-detection)

在 **Cooper Union Summer STEM** 期间，我和 Alex Wang 注意到长时间使用电脑后会有手腕不适，于是开始查阅腕管综合征的资料。这段探索引出了一个更具体的设计问题：**能否用一个简单的可穿戴原型，帮助使用者留意电脑工作时的手腕姿势？** [NHS 症状与风险因素介绍](https://www.nhs.uk/conditions/carpal-tunnel-syndrome/)

**设计思路：**我们把宽泛的健康关注点收窄到一种原型可以观察的动作：手相对于前臂向上或向下弯曲。我们尝试在手部和前臂各放置一个动作传感器，并通过反馈提醒佩戴者留意手腕姿势。这样，最初的健康问题就变成了一个可以动手制作和探索的具体设计。

*技术说明：原型使用两个 MPU6050 传感器比较动作数据，并通过 LED 提供反馈。*

**我的贡献：**我提出了双传感器设计并编写最初的 MPU6050 代码，也探索了向量计算和数据处理，并参与早期串口输出与反馈模块的编写。[查看提交与团队分工](https://github.com/yuxuan-518/carpal-tunnel-detection/blob/main/README.zh-CN.md#团队分工)

[实物与演示](https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo) · [设计思路](https://github.com/yuxuan-518/carpal-tunnel-detection#why-two-mpu6050-sensors) · [团队分工](https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions)

### [Kesty — 学习管理应用](https://github.com/yuxuan-518/kesty-support)

申请季、考试准备和研究任务常常同时占用学生的时间。像完成 Common App 申请或写一篇论文这样的大目标，并不是一个待办事项，而是由许多不同的部分组成。

**设计思路：**Kesty 让用户把一个长期目标拆成具体的小任务，再分配到不同的日期。例如，Common App 目标可以拆成主文书、补充文书和 Additional Information；课外项目可以拆成上传代码、组装原型和制作展示网站；论文目标可以拆成整理数据、撰写不同部分和推导公式。**核心想法是让每天的任务都能连回长期目标，帮助用户安排眼前的工作，同时看清它们如何推动整体进展。**

*技术说明：Kesty 是一款 SwiftUI 原生 iOS 应用，使用 Codable 数据模型在设备本地保存资料、任务和计划。*

**我的贡献：**我负责应用整体架构、本地数据组织，以及长期目标与每日任务之间的结构设计。GPT 根据我提出的设计和需求，辅助编写 Swift 与 SwiftUI 代码。

[源代码与演示](https://github.com/yuxuan-518/kesty-support#readme)

---

仓库中记录了原型及开发过程中的探索。各项目 README 介绍了当前功能、局限和合作成员。
