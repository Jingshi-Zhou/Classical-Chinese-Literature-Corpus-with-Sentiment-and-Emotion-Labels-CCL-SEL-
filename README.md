# Bilingual Classical Chinese Literature Corpus with Sentiment and Emotion Labels (CCL-SEL)



## 📖 简介 | Introduction
本数据集包含**19,999组中英古典文学句对**，涵盖13部经典作品，提供：
- 原文及人工翻译
- Google/DeepL/GPT-4o三种机器翻译
- 情感极性（积极/中性/消极）及六种情绪标注
- 多维情感得分（-1到1）与情绪概率分布

This dataset contains **19,999 Chinese-English sentence pairs** from 13 classical works, featuring:
- Original texts & human translations
- Three machine translations (Google/DeepL/GPT-4o)
- Sentiment polarity (positive/neutral/negative)
- Six basic emotions with probability distributions

## 🗃️ 数据集概览 | Dataset Overview
| 特征 | 描述 |
|-------|-------|
| 时间跨度 | 先秦至清末 |
| 文学体裁 | 诗歌、散文、哲学论著等 |
| 数据总量 | 19,999组句对 |
| 情感标签 | 19,999个极性标签 |
| 情绪标签 | 119,994个分布标签 |
| 文件格式 | JSON |

| Feature | Description |
|---------|-------------|
| Time Span | Pre-Qin to Late Qing Dynasty |
| Genres | Poetry, Prose, Philosophical Works |
| Total Pairs | 19,999 sentence pairs |
| Sentiment Labels | 19,999 polarity labels |
| Emotion Labels | 119,994 distribution labels |
| Format | JSON |

## 🧬 数据格式 | Data Structure
```json
{
  "text": {
    "ori_cn": "中文原文",
    "man_en": "人工英译",
    "mt_versions": {
      "Google": "...",
      "DeepL": "...",
      "GPT-4o": "..."
    }
  },
  "sentiment": {
    "class": "positive",
    "score": 0.82
  },
  "emotions": {
    "happy": 0.76,
    "sad": 0.12,
    "fear": 0.03,
    "anger": 0.02,
    "surprise": 0.05,
    "disgust": 0.02
  }
}

