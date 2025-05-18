# 方言语音合成实验展示

本项目展示了一个四川/上海方言语音合成的实验页面，包含参考录音、不同设置下的合成语音，以及对应的消融实验音频结果。

项目基于最小实现结构的 [F5-TTS](https://arxiv.org/abs/2410.06885)  [official Github](https://github.com/SWivid/F5-TTS)，来自 [教学网址](https://github.com/chenxie95/deeplearning_course_sjtu)。

## 🔧 文件结构说明

```bash
myself_dialect/
├── index.html # 实验展示网页
├── myself.wav # 普通话参考音频（源语音）
├── myself_shanghai/ # 上海话语音合成结果
│   └── ...
└── myself_sichuan/ # 四川话语音合成结果
    ├── nfe/ # 不同 NFE 设置下的合成结果
    │   ├── myself_sichuan_n16.wav
    │   ├── myself_sichuan_n32.wav
    │   ├── myself_sichuan_n48.wav
    │   └── myself_sichuan_n64.wav
    └── multi/ # 消融实验语音结果
        ├── myself_sichuan_x1.wav # 对应实验设置 x1
        ├── myself_sichuan_x2.wav # 对应实验设置 x2
        ├── ...
        └── myself_sichuan_x10.wav # 对应实验设置 x10
```


## 📢 浏览网页

你可以将整个文件夹上传至 GitHub，并通过 GitHub Pages [在线展示](https://the-bird-f.github.io/F5TTS-Dialect/)

---

如需更多帮助或添加打分功能、交互式统计等扩展功能，欢迎继续交流！