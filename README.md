## About

This repository organizes information around [Machine Mindset MBTI](https://github.com/PKU-YuanGroup/Machine-Mindset/)

I have had a difficult time navigating the source repositories, so consolidating information from across huggingface, their original github repository, and what I can interpret via the paper.

the point being to get new models trained based on these datasets, rather than being dependent on the llama2 models available on GitHub.

***Original Readme (slightly pruned) for the repository below***

--- 

## 🚀 Introduction

**MM (Machine_Mindset)** series models are developed through a collaboration between FarReel AI Lab(formerly known as the ChatLaw project) and Peking University's Deep Research Institute. These models are large-scale language models for various MBTI types in both Chinese and English, built on the Baichuan and LLaMA2 platforms. 🤖🌐

Our core asset is a self-constructed extensive MBTI dataset consisting of hundreds of thousands of entries. Our models are crafted **through multiple stages of pre-training, fine-tuning, and DPO training**. We are committed to continuously updating the models to offer superior performance and will consistently supplement them with experimental test results. 📊📈

In contrast to merely using prompts to alter a model's personality, we have found that this method is highly unstable. It's akin to a controlling parent's dissatisfaction with their introverted child, attempting to force them to become outgoing through simple and coercive commands – a rather ludicrous approach. 🙅‍♂️😄

We have successfully achieved **personality alignment** for various MBTI types using models such as Baichuan, Qwen, LLaMA, and Mistral. This means we can obtain 16 different versions of MBTI personality models by combining different base models with our dataset and training methods, tailoring each model for specific tasks. 🛠🧩

Due to resource constraints, we are initially releasing 16 Chinese models based on Baichuan-7b-chat and several English models based on LLaMA2-7b. However, rest assured that we can quickly add different versions of models if needed. 🌍📦

This marks our initial endeavor to combine large language models (LLMs) with personality and psychology. We will continue to explore this direction, including but not limited to: 🚀🌱

Implementing MBTI models using the MoE (Mixture of Experts) architecture
Addressing personalized needs with large language models
Exploring emotional companionship and tasks related to intelligent agent planning types. 🧠❤️
For inquiries related to deeper understanding, academic collaboration, investment, or business partnerships, please contact jiaxicui446@gmail.com.


## 🌱 Our Vision: A Thoughtful Addition 🌱

This work began with a longstanding reflection: **the human mind is akin to a pre-trained model we possess from birth**. Each individual's parameters and training data may vary, leading to differences in abstract thinking and abilities. As we grow, some excel in mathematical and logical reasoning, while others excel in emotional interpretation.

Subsequently, our learning, environment, and life experiences are equivalent to fine-tuning and aligning our pre-trained minds with human feedback. **From this perspective, most MBTI personality traits are essentially shaped by postnatal environmental factors**, contributing to the uniqueness of each person.

In other words, we can attempt to use fine-tuning and human feedback alignment (DPO) to conduct phased training on various pre-trained base LLMs, enabling the models to possess distinct MBTI attributes.

Our goal is not only to impart these models with different MBTI attributes but also to simulate the process by which humans form various MBTI personalities.

We believe that this unique approach will pave the way for a deeper understanding and utilization of large language models in the field of personality psychology. Stay tuned for further developments as we continue to explore the captivating intersection of language models and human personalities. 🌟🔍

## 🌟 Exciting Highlight! 🌟

We are thrilled to introduce you to our latest offering: not two, **but 16 distinct MBTI models**, now available for your exploration! Take a deep dive into the realm of personality with our open-source treasure trove.
 
🤔 Wondering what you can do with these models? Here are just a few exciting possibilities:

+ **Find the perfect gift for your partner** during special occasions.
+ Gain insights into **how individuals you follow** react in various situations.
+ Gain a deeper understanding of the customization, personalization, and possibilities of large models.
+ When making significant decisions, consider the personality traits in different contexts.
+ Promote personal growth and mutual understanding through a profound understanding of the complexity of human nature.

In the era of the LLM large model, deepen your understanding of personality types like never before! 🎉🧠🌈

<div align="center"><img src="https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/arxiv_index.png" style="width=40%;"/></div>

## 📚 Dataset Introduction

We have open-sourced our **MBTI Training Dataset**, meticulously crafted to train large language models with different MBTI personality types. 🌐🔍

https://huggingface.co/datasets/FarReelAILab/Machine_Mindset

The release of this dataset signifies our unique contribution to both Large Language Models (LLMs) and the field of psychology. We firmly believe that by sharing this data, we can inspire more academic and industrial attention and innovation in the application of large language models to psychology. 🧠📘

Our dataset covers a wide range of scenarios designed to assist researchers and developers in training base models capable of understanding and simulating different MBTI personalities. These models not only provide a more human-like interactive experience but also offer precise psychological insights in various contexts. 🤖💬

We encourage everyone to explore and utilize this dataset to develop more innovative and in-depth applications for large language models. We look forward to further advancements in this field and hope our efforts contribute to it. 🚀🌟

For more details and usage guidelines about the dataset, please refer to our [detailed documentation](https://github.com/PKU-YuanGroup/Machine-Mindset/tree/main/datasets/behaviour).

### **Interpretation**

We intentionally overfitted our models on personality data, which resulted in poor performance in the evaluations. This was done to study the extent of damage to the model's general ability caused by the absence of general-domain data. Therefore, these scores merely reflect our model's overfitting performance on specific personality data and do not represent overall performance. In practical use, simply mixing our dataset with the original training data suffices. Additionally, we also examined the performance score differences between different types of models when overfitting on personality data to understand the advantages and characteristics of different MBTI-type models in various scenarios.



## 🚀 Main Results

### Random Question-Answer results
Below, we provide visual representations of the random question-answer results for different personality types, each with its own unique characteristics and tendencies:

+ **ENFP Results** Dive into the world of ENFP personalities and gain insights into their responses to random questions. Discover the creative and imaginative nature of ENFPs in their answers.
<div align="center"><img src="https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_ENFP_res.png" style="width=40%;"/></div>

+ **INTJ Results** Dive into the outcomes of INTJ personalities and observe their analytical and strategic approach to tackling random questions. Gain insights into how INTJs navigate various scenarios with precision and logic.
<div align="center"><img src="https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_INTJ_res.png" style="width=40%;"/></div>

+ **INFP Results** Discover the responses of INFP personalities and appreciate their idealistic and empathetic nature when answering random questions. Explore their unique perspectives and insights.
<div align="center"><img src="https://raw.githubusercontent.com/PKU-YuanGroup/Machine-Mindset/main/images/EN_INFP_res.png" style="width=40%;"/></div>

Investigate the results of INTP personalities and observe their analytical and logical approach to random queries. Gain insights into their problem-solving and creative thinking abilities.
These visual representations offer a glimpse into the diverse world of personality types, providing an opportunity to better understand and appreciate the unique traits and tendencies associated with each type. 📊🧠🔍

## 🔒 License

* Our code adheres to the Apache 2.0 open-source license. Please refer to the [LICENSE](https://github.com/PKU-YuanGroup/Machine-Mindset/blob/main/LICENSE) for specific details of the open-source agreement.

* Our model weights are subject to an open-source agreement based on the original weights, with specific details provided in the Chinese version under the baichuan open-source license. For commercial use, please refer to [model_LICENSE](https://huggingface.co/JessyTsu1/Machine_Mindset_zh_INTP/resolve/main/Machine_Mindset%E5%9F%BA%E4%BA%8Ebaichuan%E7%9A%84%E6%A8%A1%E5%9E%8B%E7%A4%BE%E5%8C%BA%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf) for further information.

* The English version follows the open-source agreement under the [llama2 license](https://ai.meta.com/resources/models-and-libraries/llama-downloads/).

## ✏️ Citation

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
