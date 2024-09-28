## Direct Preference Optimization Documentation

MBTI has four dimensions, each containing two attributes, making it a natural fit for Direct Preference Optimization (DPO). Below is a more detailed introduction and how to use the datasets we provide for DPO.

### Why Choose MBTI Datasets for DPO?

The combination of four dimensions and attributes in MBTI datasets provides a rich landscape for optimizing model preferences. Take the first dimension, "Energe," for example, which includes "Introversion" (I) and "Extraversion" (E) attributes. If you want your model to exhibit more introverted behavior rather than extraverted, you can use the corresponding `zh_energy_introversion.json` and `zh_energy_extraversion.json` data files and combine them into a new JSON dataset of DPO type, such as `dpo_energy_i_e.json`. This approach is applicable to all four dimensions, offering a wide range of choices and experimental possibilities.

### How to Perform DPO Training?

Let's assume we want to conduct DPO training on an INFP model to make it exhibit specific preferences across the four MBTI dimensions (Energe, Information, Decision, and Execution). In this example, we need four datasets representing these dimensions:

- `en_energe_introversion.json` (Energe dimension, Introversion attribute)
- `en_information_sensing.json` (Information dimension, Sensing attribute)
- `en_decision_feeling.json` (Decision dimension, Feeling attribute)
- `en_execution_perceiving.json` (Execution dimension, Perceiving attribute)

Next, combine these four datasets and randomize them to create a new DPO dataset, such as `dpo_infp.json`. This new dataset will include attribute combinations from different dimensions, helping you achieve specific preference optimization for the INFP model.

### Multilingual Mixed Training

Please note that you can also perform multilingual mixed training, which means you can use datasets in multiple languages to train your model. According to our experimental results, this approach can yield better outcomes and enable richer and more diverse model behaviors.

By leveraging MBTI datasets for DPO training, you can customize specific preferences for your model's behavior and personality based on your needs and goals, resulting in a more personalized natural language generation.