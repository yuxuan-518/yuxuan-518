# Hi, I'm Shaoxuan 👋

**Embedded systems · Sensors · Software**

[简体中文](https://github.com/yuxuan-518/yuxuan-518/blob/main/README.zh-CN.md)

## About me

```javascript
const shaoxuan = {
  interests: ["Embedded systems", "Sensors", "App development"],
  learning: ["C / AVR C", "Swift / SwiftUI"],
  hardware: ["Arduino Uno", "ATmega328P", "MPU6050"],
  approach: "Build a prototype, test it, and learn from the results"
};
```

## Projects

### [Dual-MPU6050 Posture Feedback Prototype](https://github.com/yuxuan-518/carpal-tunnel-detection)

During **Cooper Union Summer STEM**, Alex Wang and I noticed wrist discomfort after long hours at a computer and began researching carpal tunnel syndrome. That exploration led us to a more focused design question: **Could a simple wearable help someone notice their wrist posture during computer use?** [NHS overview](https://www.nhs.uk/conditions/carpal-tunnel-syndrome/)

**Design process:** We narrowed the broad health concern to one behavior a prototype could respond to: the hand bending up or down relative to the forearm. We explored placing one motion sensor on the hand and another on the forearm, then using feedback to draw attention to wrist posture. This gave us a concrete idea to build and investigate.

*Technical note: The prototype compares motion data from two MPU6050 sensors and provides LED feedback.*

**My contribution:** I proposed the dual-sensor design and wrote its initial MPU6050 code. I also explored vector calculations and data processing, and contributed early serial-output and feedback modules. [Contribution history](https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions)

[Photo & demo](https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo) · [Design rationale](https://github.com/yuxuan-518/carpal-tunnel-detection#why-two-mpu6050-sensors) · [Team contributions](https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions)

### [Kesty — Study Management App](https://github.com/yuxuan-518/kesty-support)

During application season, exam preparation, and research, students often have several large commitments competing for their time. **A goal like completing the Common App or writing a research paper is made up of many smaller pieces, not one checkbox.**

**Design idea:** Kesty lets users turn a large goal into smaller tasks and spread them across individual days. For example, a Common App goal could include the personal statement, supplemental essays, and Additional Information. An extracurricular project could include pushing code, assembling a prototype, and building a showcase website. A research paper could include organizing data, drafting sections, and deriving formulas. **The central idea is to connect each day’s work to the larger goal, so users can plan what to do now while keeping the overall project in view.**

*Technical note: Kesty is a native iOS app built with Swift and SwiftUI. It uses Codable models and `UserDefaults` for local data storage; cloud synchronization is not currently implemented.*

**My contribution:** I defined the app’s architecture, local data organization, and the structure connecting long-term goals with daily tasks. GPT assisted with writing the Swift and SwiftUI code based on the design and requirements I defined.

[Source code and demo](https://github.com/yuxuan-518/kesty-support#readme)

---

My repositories document both working prototypes and the experiments that led to them. Each project's README explains its current features, limitations, and collaborators.
