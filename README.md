# 四川方言语音合成实验展示

本项目展示了一个四川方言语音合成的实验页面，包含参考录音、不同设置下的合成语音，以及对应的消融实验音频结果。

## 🔧 文件结构说明

```bash
myself_dialect/
├── index.html # 实验展示网页
├── myself.wav # 普通话参考音频（源语音）
└── myself_sichuan/ # 四川话语音合成结果文件夹
├── nfe/ # 不同 NFE 设置下的合成结果
│ ├── myself_sichuan_n16.wav
│ ├── myself_sichuan_n32.wav
│ ├── myself_sichuan_n48.wav
│ └── myself_sichuan_n64.wav
└── multi/ # 消融实验语音结果
├── myself_sichuan_x1.wav # 对应实验设置 x1
├── myself_sichuan_x2.wav # 对应实验设置 x2
├── ...
└── myself_sichuan_x10.wav # 对应实验设置 x10
```


## 📄 内容说明

- `index.html`：展示实验结果的主网页，支持音频播放和表格对比。
- `myself.wav`：普通话参考录音，供合成模型模仿。
- `myself_sichuan/nfe/`：不同 `NFE` 参数（如 16、32、48、64）下生成的四川话语音文件，用于分析采样效率对语音质量的影响。
- `myself_sichuan/multi/`：消融实验对应的 10 个设置（x1 到 x10），用于分析微调步数 `FT` 和任务向量增强因子 `α` 对合成效果的影响。

## 🧪 实验设置参考（简要）

- NFE：用于采样的步数，值越大合成时间越长但质量可能更高。
- FT：微调步数（Fine-tuning steps），如 60k、80k、100k。
- α：任务向量增强因子，控制四川话特征注入的程度。

## 📢 浏览网页

你可以将整个文件夹上传至 GitHub，并通过 GitHub Pages 在线展示：
`https://the-bird-f.github.io/F5TTS-Dialect/`

---

如需更多帮助或添加打分功能、交互式统计等扩展功能，欢迎继续交流！