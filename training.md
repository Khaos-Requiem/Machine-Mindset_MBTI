## Dataset introduction

There are four dimension in MBTI. And there are two opposite attributes within each dimension.

+ Energe: Extraversion (E) - Introversion (I)
+ Information: Sensing (S) - Intuition (N)
+ Decision: Thinking (T) - Feeling (F)
+ Execution: Judging (J) - Perceiving (P)

The datasets follow the Alpaca format, consisting of instruction, input and output.

## How to use these datasets for behavior supervised fine-tuning (SFT)

if you want to make an LLM behave like an ***ISFJ***, you need to select ***the four corresponding files*** (en_energe_introversion.json, en_information_sensing.json, en_decision_feeling.json, en_execution_judging.json). 

And use the four for SFT.

## How to use these datasets for direct preference optimization (DPO)

If you want to make an LLM be ***more feeling (F) than thinking (T)*** by DPO, you need to select ***the two corresponding files*** (en_decision_feeling.json, en_decision_thinking.json). 

And then compile the two into the correct format for DPO. For the correct format, please refer to [this](https://github.com/PKU-YuanGroup/Machine-Mindset/blob/main/datasets/dpo/README.md).

## Using these Datasets according to the paper

[Machine Mindset](MM-paper.md)

### Three Types of Datasets:

1. [**Behavior Datasets**](dataset/behaviour):
   - Purpose: Train LLMs to respond consistently with specific personality traits
   - Created by customizing the Alpaca dataset for each MBTI dimension
2. [**Self-awareness Datasets**](dataset):
   - Purpose: Enable LLMs to recognize and describe their own personality traits
   - Consists of Q&A pairs for each of the 16 MBTI personality types
3. [**DPO (Direct Preference Optimization) Datasets**](dataset/dpo):
   - Purpose: Reinforce the model's preference for responses aligned with target personality traits
   - Contains pairs of responses for each MBTI dimension (e.g., Feeling vs Thinking)

### Five Stages of Training:

1. [**First Stage of Supervised Fine-Tuning (SFT)**](dataset/behaviour/README.md):
   - Uses behavior datasets to train the model on responses consistent with specific MBTI traits
2. **Second Stage of Supervised Fine-Tuning (SFT)**:
   - Uses self-awareness datasets to enhance the model's ability to recognize and describe its personality
3. [**Direct Preference Optimization (DPO)**](dataset/dpo/README.md):
   - Trains the model to prefer responses aligned with the target personality traits
4. **Evaluation**:
   - Assesses the model's personality traits using modified MBTI questionnaires
5. **Testing**:
   - Conducts additional tests to evaluate how personality traits affect the model's performance in various tasks

This multi-stage approach aims to create LLMs with stable, consistent personalities that can both exhibit traits in their responses and accurately describe their own personality type.

