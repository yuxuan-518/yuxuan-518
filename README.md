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

During **Cooper Union Summer STEM**, Alex Wang and I researched carpal tunnel syndrome after noticing wrist discomfort during long hours at a computer. Its symptoms can include numbness, tingling, or pain in the hand and fingers, and sometimes a weaker grip. Repeatedly bending the wrist or gripping forcefully can increase risk, so we chose to explore a simple reminder for prolonged, awkward wrist positions. [NHS overview](https://www.nhs.uk/conditions/carpal-tunnel-syndrome/)

**Technical approach:** We explored comparing motion data from sensors placed on the hand and forearm to estimate relative wrist posture. An early version calculated the angle between vectors. The final integrated main program compares raw acceleration-vector dot products and triggers LED feedback; a buzzer module is also in the repository, though it is not called by the final main loop.

**My contribution:** I proposed the dual-sensor design and wrote its initial MPU6050 code. I also developed vector calculations, explored data-processing approaches, and contributed early serial, LED, and buzzer modules. [Contribution history](https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions)

[Photo & demo](https://github.com/yuxuan-518/carpal-tunnel-detection#prototype-and-demo) · [Design rationale](https://github.com/yuxuan-518/carpal-tunnel-detection#why-two-mpu6050-sensors) · [Team contributions](https://github.com/yuxuan-518/carpal-tunnel-detection#team-contributions)

### [Kesty — Study Management App](https://github.com/yuxuan-518/kesty-support)

A SwiftUI app experiment exploring task management and focus sessions, developed with AI assistance.

[Source & demo](https://github.com/yuxuan-518/kesty-support#readme)

---

My repositories document both working prototypes and the experiments that led to them. Each project's README explains its current features, limitations, and collaborators.
