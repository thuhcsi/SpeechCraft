# SpeechCraft

This is the official repository of the ACM Multimedia 2024 paper *"SpeechCraft: A Fine-Grained Expressive Speech Dataset with Natural Language Description"*.

For details of the pipeline and dataset, please refer to our [Paper](https://openreview.net/forum?id=rjAY1DGUWC) and [Demo Page](https://speechcraft2024.github.io/speechcraft2024/)

<!-- Dataset and pipeline are coming soon. -->

## Download Speech Corpus

|Language|Speech Corpus|#Duration|#Clips|
|:--------:|:--------:|--------:|--------:|
|ZH|[Zhvoice](https://github.com/fighting41love/zhvoice)|799.68h|1,020,427|
|ZH|[AISHELL-3](https://www.openslr.org/93/)|63.70h|63,011|
|EN|[GigaSpeech-M](https://huggingface.co/datasets/speechcolab/gigaspeech/tree/main/data/audio/m_files_additional)|739.91h|670,070|
|EN|[LibriTTS-R](https://www.openslr.org/141/)|548.88h|352,265|


<!-- ## Metadata Walkthrough -->
## Download Speech Annotation
||Description|Instruction|
|:--------:|:--------:|:--------:|
|ZH|[download](https://cloud.tsinghua.edu.cn/f/e66664542f534f399802/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/d6f00e027f504751b4c0/?dl=1)|
|EN|[download](https://cloud.tsinghua.edu.cn/f/517428835bd5486e87e8/?dl=1)|[download](https://cloud.tsinghua.edu.cn/f/cce83dd884ed4104b1a1/?dl=1|)

## Request Access to Emphasis Speech Dataset

Since we do not own the copyright of the original audio files, for researchers and educators who wish to use the audio files for non-commercial research and/or educational purposes, we can provide access to our regenerated version under certain conditions and terms. To apply for the AISHELL-3 and LibriTTS-R with fine-grained keyword emphasis, please fill out the EULA form at `Emphasis-SpeechCraft-EULA.pdf` and send the scanned form to jinzeyu23@mails.tsinghua.edu.cn. Once approved, you will be supplied with a download link.

Please first refer to some emphasis examples provided [here](https://speechcraft2024.github.io/speechcraft2024/#13-examples-of-the-regenerated-emphasis-data-from-aishell-3-and-libritts-r). We are actively working on improving methods for large-scale fine-grained data construction that align with human perception.

|Language|Speech Corpus|#Duration|#Clips|
|:--------:|:--------:|--------:|--------:|
|ZH|AISHELL-3-stress|50.59h|63,258|
|EN|LibriTTS-R-stress|148.78h|75,654|

## Pipeline

To be released.

## Citation
Please cite our paper if you find this work useful:
```
@inproceedings{jin2024speechcraft,
title={SpeechCraft: A Fine-Grained Expressive Speech Dataset with Natural Language Description},
author={Zeyu Jin and Jia Jia and Qixin Wang and Kehan Li and Shuoyi Zhou and Songtao Zhou and Xiaoyu Qin and Zhiyong Wu},
booktitle={ACM Multimedia 2024},
year={2024},
url={https://openreview.net/forum?id=rjAY1DGUWC}
}```