## About

This repository organizes information around [PKU-YuanGroup/Machine Mindset](https://github.com/PKU-YuanGroup/Machine-Mindset/)

I have had a difficult time navigating the source repositories, so consolidating information from across huggingface, their original github repository, and what I can interpret via [the paper](MM-paper.md).

the point being to get new models trained based on these datasets, rather than being dependent on the llama2 models available on GitHub.

I included only the english datasets here, but of course those can be gotten from [the source](https://github.com/PKU-YuanGroup/Machine-Mindset/), if you need them.

## Notes based on original Readme

**Introduction**
- MM (Machine_Mindset) series models developed by FarReel AI Lab and Peking University
- Large-scale language models for MBTI types in Chinese and English
- Core asset: extensive self-constructed MBTI dataset
- Models developed through pre-training, fine-tuning, and DPO training
- Continuous updates and experimental test results promised

**Approach**
- Achieved personality alignment for MBTI types using various base models
- 16 different versions of MBTI personality models
- Initially releasing 16 Chinese models (Baichuan-7b-chat) and several English models (LLaMA2-7b)
- Can quickly add different versions if needed

**Future Exploration**
- Implementing MBTI models using MoE architecture
- Addressing personalized needs with LLMs
- Exploring emotional companionship and intelligent agent planning tasks

**Vision**
- Human mind likened to a pre-trained model from birth
- Individual differences in abstract thinking and abilities
- Life experiences equated to fine-tuning and aligning pre-trained minds
- MBTI personality traits shaped by postnatal environmental factors
- Goal: Simulate human MBTI personality formation process in LLMs

**Highlight**
- 16 distinct MBTI models available for exploration
- Open-source offering

**Potential Applications**
- Finding perfect gifts for partners
- Gaining insights into followed individuals' reactions
- Understanding customization and personalization of large models
- Considering personality traits in decision-making
- Promoting personal growth and mutual understanding

**Contact**
- For inquiries: jiaxicui446@gmail.com

<div align="center"><img src="https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/arxiv_index.png" style="width=40%;"/></div>

**MBTI Training Dataset Release**
- Open-sourced dataset for training LLMs with MBTI personality types
- [Available on Hugging Face](https://huggingface.co/datasets/FarReelAILab/Machine_Mindset)

**Significance**
- Unique contribution to LLMs and psychology
- Aims to inspire academic and industrial innovation
- Bridges LLMs and psychological applications

**Dataset Features**
- Covers wide range of scenarios
- Helps train models to understand and simulate MBTI personalities
- Enables more human-like interactions and precise psychological insights

**Call to Action**
- Encourages exploration and utilization of the dataset
- Aims to foster innovative applications for LLMs
- Hopes to contribute to advancements in the field

**Additional Information**
- [Detailed documentation available on GitHub](dataset/behaviour)

**Interpretation of Results**
- Models intentionally overfitted on personality data
- Poor evaluation performance due to absence of general-domain data
- Scores reflect overfitting on specific personality data, not overall performance
- Practical use: mix dataset with original training data
- Examined performance differences between MBTI-type models in various scenarios

**Main Results**

- Random Question-Answer results presented visually for different personality types
- Unique characteristics and tendencies shown for each type

- ENFP Results:
  - Insights into creative and imaginative nature
    ![ENFP image link](https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_ENFP_res.png)

- INTJ Results:
  - Analytical and strategic approach demonstrated
  - Precision and logic in navigating scenarios
    ![INTJ image link](https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_INTJ_res.png)

- INFP Results:
  - Idealistic and empathetic nature shown
  - Unique perspectives and insights explored
    ![INFP image link](https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_INFP_res.png)

- INTP Results:
  - Analytical and logical approach to queries
  - Problem-solving and creative thinking abilities highlighted

**License**

- Code: Apache 2.0 open-source license
  - Details in [LICENSE](https://github.com/PKU-YuanGroup/Machine-Mindset/blob/main/LICENSE)

- Model weights:
  - Chinese version: Based on baichuan open-source license
  - Commercial use details in [model_LICENSE](https://huggingface.co/JessyTsu1/Machine_Mindset_zh_INTP/resolve/main/Machine_Mindset%E5%9F%BA%E4%BA%8Ebaichuan%E7%9A%84%E6%A8%A1%E5%9E%8B%E7%A4%BE%E5%8C%BA%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)

- English version: Follows [llama2 license](https://ai.meta.com/resources/models-and-libraries/llama-downloads/)

**Citation**

If you find our paper and code useful in your research, please consider giving a star :star: and citation :pencil:.

```BibTeX
@misc{cui2023machine,
      title={Machine Mindset: An MBTI Exploration of Large Language Models}, 
      author={Jiaxi Cui and Liuzhenghao Lv and Jing Wen and Rongsheng Wang and Jing Tang and YongHong Tian and Li Yuan},
      year={2023},
      eprint={2312.12999},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
