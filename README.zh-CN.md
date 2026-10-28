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

在 **Cooper Union Summer STEM** 期间，我和 Alex Wang 注意到长时间使用电脑后会有手腕不适，于是开始查阅腕管综合征的资料。它的症状可能包括手和手指麻木、刺痛或疼痛，有时还会握力减弱。反复弯曲手腕或用力抓握可能增加患病风险，因此我们选择探索一种简单的提醒方式，帮助使用者留意手腕长时间处于不自然姿势的情况。[NHS 症状与风险因素介绍](https://www.nhs.uk/conditions/carpal-tunnel-syndrome/)

**技术思路：**我们尝试比较佩戴在手部和前臂的传感器数据，以估算手腕的相对姿态。早期版本尝试计算两个向量之间的夹角；最终整合的主程序则比较原始加速度向量的点积，并触发 LED 提示。仓库中也有蜂鸣器模块，但最终主循环没有调用它。

**我的贡献：**我提出了双传感器设计并编写了初期 MPU6050 代码，也开发了向量计算、探索数据处理方案，并参与早期串口、LED 和蜂鸣器模块的编写。[查看提交与团队分工](https://github.com/yuxuan-518/carpal-tunnel-detection/blob/main/README.zh-CN.md#团队分工)

[实物与演示](https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo) · [中文项目介绍与团队分工](https://github.com/yuxuan-518/carpal-tunnel-detection/blob/main/README.zh-CN.md)

### [Kesty — 学习管理应用](https://github.com/yuxuan-518/kesty-support)

Kesty 帮助学生规划长期学习任务和大型项目。当大学申请、考试准备和研究任务同时推进时，用户可以把 Common App 申请、课外项目或论文等设为目标，再将每个目标拆分成具体的小任务。无论是撰写文书、准备项目材料、整理数据，还是推导公式，都可以安排到每天逐步完成，帮助学生稳步推进目标、规划时间。

**技术实现：**Kesty 是一款使用 Swift 和 SwiftUI 构建的原生 iOS 应用。各个 SwiftUI 页面通过 `ObservableObject` 共享应用状态；Codable 数据模型用于描述个人资料、任务、目标、计划和专注记录。应用使用 `UserDefaults` 和 JSON 编码在设备本地保存数据，目前尚未实现云端数据库同步。

**我的贡献：**我负责应用架构、数据组织和核心功能结构的设计。GPT 根据我定义的设计和需求，辅助编写 Swift 与 SwiftUI 代码。

[源代码与演示](https://github.com/yuxuan-518/kesty-support#readme)

---

仓库中记录了原型及开发过程中的探索。各项目 README 介绍了当前功能、局限和合作成员。
