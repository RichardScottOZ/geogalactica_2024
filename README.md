<div style="text-align:center">
<centering>
<h1>Ge🌏Galactica</h1>
<!-- <img src="https://big-cheng.com/geogal/geogal_orange.png" alt="geogal-logo" width="400"/> -->
<h2>A Scientific Large Language Model in Geoscience</h2>
</div>

<a href='https://arxiv.org/abs/2401.00434'><img src='https://img.shields.io/badge/Paper-ArXiv-C71585'></a> <a href='https://huggingface.co/geobrain-ai/qomolangma'><img src='https://img.shields.io/badge/%F0%9F%A4%97%20Hugging Face-geogalactica-red'></img></a> <a href='https://huggingface.co/datasets/daven3/geosignal'><img src='https://img.shields.io/badge/Dataset-GeoSignal-4169E1'></img></a> <a href='https://huggingface.co/datasets/daven3/geobench'><img src='https://img.shields.io/badge/Dataset-GeoBench-4169E1'></img></a>

- Technical report is [HERE](https://arxiv.org/abs/2401.00434)!
- The data pre-processing toolkits are open sourced on [sciparser](https://github.com/davendw49/sciparser)!

## Statement
**To clarify with potential confusions, we hereby state that the model with the manuscript "GeoGalactica: A Scientific Large Language Model in Geoscience" is not associated with the DDE Program, nor supported by DDE related fundings. We feel sorry for the unintentional misunderstandings and inconvenience, and we commit to prevent future misunderstandings.**

## Introduction

GeoGalactica is from further pre-training of Galactica -- a top-performing LLM trained with a large number of scientific documents. In this work, we take the initial step to leverage LLM for science, through a rather straightforward approach. We try to specialize an open-sourced LLM into geoscience, by further pre-training the model with a vast amount of texts in geoscience, as well as supervised fine-tuning (SFT) the resulting model with our custom collected instruction tuning dataset. These efforts result in a model GeoGalactica consisting of 30 billion parameters. To our best knowledge, it is the largest language model for the geoscience domain.

## Resources

- Paper: https://github.com/geobrain-ai/geogalactica 
- Data: https://huggingface.co/datasets/daven3/geobench, https://huggingface.co/datasets/daven3/geosignal, and https://github.com/zthang/geotools
- Model: https://huggingface.co/geobrain-ai/geogalactica
- Checkpoints: https://huggingface.co/geobrain-ai/geogalactica-ckpt
- Plot: https://github.com/dbylynn/GeoGalactica_Analysis
- Sciparser: https://github.com/davendw49/sciparser

## Quick Start

A simple script is provided (`tools/prediction/demo.py`) for the model to predict the output text for a single input. The memory exceeds 140GB.
The folder `example_data` shares data file format during the training.

## Contributors

This project was founded by Acemap at Shanghai Jiao Tong University, leading by [Zhouhan Lin](https://hantek.github.io/) and a group of students including [Cheng Deng](https://big-cheng.com/)* (student leader), [Le Zhou](https://github.com/lzhou1998), [Tianhang Zhang](https://github.com/zthang), [Yi Xu](https://github.com/xyjigsaw), [Yutong Xu](https://github.com/xyt-fe), [Beiya Dai](https://github.com/dbylynn), [Qiyuan Chen](mailto:qiyuan04@sjtu.edu.cn), [Yuanyuan Shi](https://github.com/syy-yoyo) and [Zhongmou He](https://github.com/twelfth-star) supervised by [Zhouhan Lin](https://hantek.github.io/), [Junxian He](https://jxhe.github.io/), Xinbing Wang, and Chenghu Zhou.

## Acknowledgements

GeoGalactica has referred to the following open-source projects. We want to express our gratitude and respect to the researchers of the projects.

- Facebook Galactica: https://galactica.org/
- Facebook LLaMA: https://github.com/facebookresearch/llama
- Stanford Alpaca: https://github.com/tatsu-lab/stanford_alpaca
- alpaca-lora by @tloen: https://github.com/tloen/alpaca-lora
- alpaca-gp4 by Chansung Park: https://github.com/tloen/alpaca-lora/issues/340
- K2 by Cheng Deng: https://github.com/davendw49/k2

We would also like to express our appreciation for the effort of data processing and annotation from the students in CAS.

## License
GeoGalactica is a research preview intended for non-commercial use only, subject to the model License of Galactica and the Terms of Use of the data generated by OpenAI. Please contact us if you find any potential violations. The code is released under the Apache License 2.0. The data GeoSignal and GeoBench is open-sourced by [K2](https://github.com/davendw49/k2).

<!--
## Citation
The paper is available on [arXiv](https://arxiv.org/abs/2401.00434), If you use the code or data of **GeoGalactica**, please declare the reference with the following:

```
@misc{lin2023geogalactica,
      title={GeoGalactica: A Scientific Large Language Model in Geoscience}, 
      author={Zhouhan Lin and Cheng Deng and Le Zhou and Tianhang Zhang and Yi Xu and Yutong Xu and Zhongmou He and Yuanyuan Shi and Beiya Dai and Yunchong Song and Boyi Zeng and Qiyuan Chen and Tao Shi and Tianyu Huang and Yiwei Xu and Shu Wang and Luoyi Fu and Weinan Zhang and Junxian He and Chao Ma and Yunqiang Zhu and Xinbing Wang and Chenghu Zhou},
      year={2023},
      eprint={2401.00434},
      archivePrefix={arXiv},
      primaryClass={cs.CL}
}
```
-->
