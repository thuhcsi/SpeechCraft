# SpeechCraft

This is the official repository of the ACM Multimedia 2024 paper *"SpeechCraft: A Fine-Grained Expressive Speech Dataset with Natural Language Description"*.

For details of the pipeline and dataset, please refer to our [Paper](http://arxiv.org/abs/2408.13608) and [Demo Page](https://speechcraft2024.github.io/speechcraft2024/)

<!-- Dataset and pipeline are coming soon. -->

## Download Speech Corpus

|Language|Speech Corpus|#Duration|#Clips|
|:--------:|:--------:|--------:|--------:|
|ZH|[Zhvoice](https://github.com/fighting41love/zhvoice)|799.68h|1,020,427|
|ZH|[AISHELL-3](https://www.openslr.org/93/)|63.70h|63,011|
|EN|[GigaSpeech-M](https://huggingface.co/datasets/speechcolab/gigaspeech/tree/main/data/audio/m_files_additional)|739.91h|670,070|
|EN|[LibriTTS-R](https://www.openslr.org/141/)|548.88h|352,265|

## News
[2024-09-26]: **Structured metadata** (pitch, energy, speed, age, gender, emotion tone, emphasis, topic/category, and transcript) has been made available to facilitate further enhancements and augmentations of the dataset.

<!-- ## Metadata Walkthrough -->
## Download Speech Annotation
||Description|Instruction|Labels|
|:--------:|:--------:|:--------:|:--------:|
|ZH|[download](https://cloud.tsinghua.edu.cn/f/e66664542f534f399802/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/d6f00e027f504751b4c0/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/02a69d7c862e4422850e/?dl=1)|
|EN|[download](https://cloud.tsinghua.edu.cn/f/517428835bd5486e87e8/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/cce83dd884ed4104b1a1/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/6f05dcbcfb384ea1870b/?dl=1)|

#### Labels and Prompts
**EN** \
**Gender**: Male, Female \
**Age**: Child, Teenager, Youth adult, Middle-aged, Elderly \
**Pitch**: low, normal, high \
**Speed**: slow, normal, fast \
**Volume**: low, normal, high \
**Emotion** (English): Fearful, Happy, Disgusted, Sad, Surprised, Angry, Neutral \
**Emphasis**: Non-label words\
**Transcript**: Non-label sentence\
**LLM Prompt**: \
Given the pitch, volume, age, gender, tone, and transcript, use sentiment analysis techniques to describe in natural language what age, what gender of a person, with what kind of emotion and tone, using what kind of pitch and volume, spoke the words in the transcript.\
Note: You must vividly describe the sentence’s intonation, pitch, tone, and emotion. All outputs must strictly avoid identical wording and sentence structure. There is no need to describe body language or psychological state and do not repeat the input content.\
Refer to the format of the following four cases:\
*Example Input - Example Output*\
Now try to process the following sentences, directly output the converted sentences according to the examples without missing any labels.

**ZH** \
**年龄**：儿童，少年，青年，中年，老年\
**性别**：男，女\
**语速**：快，中，慢\
**音高**：高，中，低\
**音量**：高，中，低\
**重读**：无标签，字词\
**语气**：无标签，自然语句\
**文本**：无标签，自然语句\
**LLM Prompt**: \
请参照以下转换案例，使用中文自然语言描述一个人按照给定风格属性，如音高、音量、年龄、性别、语调，来说文本中的话。注意，仅描述说话风格，不需要描述肢体动作或心理状态，不要重复输入的内容。\
*示例输入-示例输出*\
现在尝试处理以下句子，根据示例直接输出转换后的句子，不要遗漏任何标签。

## Request Access to Emphasis Speech Dataset

Since we do not own the copyright of the original audio files, for researchers and educators who wish to use the audio files for non-commercial research and/or educational purposes, we can provide access to our regenerated version under certain conditions and terms. To apply for the AISHELL-3 and LibriTTS-R with fine-grained keyword emphasis, please fill out the EULA form at `Emphasis-SpeechCraft-EULA.pdf` and send the scanned form to jinzeyu23@mails.tsinghua.edu.cn. Once approved, you will be supplied with a download link. **([2024-09-26]: With metadata updated!)**

Please first refer to some emphasis examples provided [here](https://speechcraft2024.github.io/speechcraft2024/#13-examples-of-the-regenerated-emphasis-data-from-aishell-3-and-libritts-r). We are actively working on improving methods for large-scale fine-grained data construction that align with human perception.

|Language|Speech Corpus|#Duration|#Clips|
|:--------:|:--------:|--------:|--------:|
|ZH|AISHELL-3-stress|50.59h|63,258|
|EN|LibriTTS-R-stress|148.78h|75,654|

## Citation
Please cite our paper if you find this work useful:
```
@inproceedings{jin2024speechcraft,
title={SpeechCraft: A Fine-Grained Expressive Speech Dataset with Natural Language Description},
author={Zeyu Jin and Jia Jia and Qixin Wang and Kehan Li and Shuoyi Zhou and Songtao Zhou and Xiaoyu Qin and Zhiyong Wu},
booktitle={ACM Multimedia 2024},
year={2024},
url={https://openreview.net/forum?id=rjAY1DGUWC}
}
```
