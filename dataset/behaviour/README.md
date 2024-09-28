## Dataset Introduction

Here are the behavior datasets used for supervised fine-tuning (SFT), which can also be utilized for direct preference optimization (DPO).

An identical copy of these datasets can also be found on [HuggingFace](https://huggingface.co/datasets/FarReelAILab/Machine_Mindset).

The 'en' directory contains datasets of the English version.

The 'zh' directory contains datasets of the Chinese version.

MBTI has four dimensions, each with two opposing attributes.

To be specific:

+ Energe: Extraversion (E) - Introversion (I)
+ Information: Sensing (S) - Intuition (N)
+ Decision: Thinking (T) - Feeling (F)
+ Execution: Judging (J) - Perceiving (P)

Based on the above, you can infer the content of the JSON file from its name.

The datasets follow the Alpaca format, consisting of instructions, input, and output.

Detailed instructions on how to use these datasets for supervised fine-tuning (SFT) and direct preference optimization (DPO):

### How to use these datasets for supervised fine-tuning

For example, if you want to make an LLM behave like an ISFJ, you need to select the four corresponding files (en_energe_introversion.json, en_information_sensing.json, en_decision_feeling.json, en_execution_judging.json).

And use these four for SFT.

### How to use these datasets for direct preference optimization

For example, if you want to make an LLM be more feeling (F) than thinking (T) by DPO, you need to select the two corresponding files (en_decision_feeling.json, en_decision_thinking.json).

And then compile these two into the correct format for DPO. For the correct format, please refer to [this link](https://github.com/PKU-YuanGroup/Machine-Mindset/blob/main/datasets/dpo/README.md).