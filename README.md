# LoGiPT
The official implementation of NAACL'24 paper: [Language Models can be Deductive Solvers](https://aclanthology.org/2024.findings-naacl.254.pdf).

## Model Details

These are the trained models for **LoGiPT**.

|           LoGiPT          |  proofwriter  |    prontoqa   |
|:-------------------------:|:-------------:|:-------------:|
|    vicuna-13b-v1.5-16k    | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-vicuna-13b-v1.5-16k-proofwriter) | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-vicuna-13b-v1.5-16k-prontoqa) |
|      CodeLlama-13b-hf     | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-CodeLlama-13b-hf-proofwriter) | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-CodeLlama-13b-hf-prontoqa) |
| CodeLlama-13b-Instruct-hf | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-CodeLlama-13b-Instruct-hf-proofwriter) | [HF_model_card](https://huggingface.co/jzfeng/LoGiPT-CodeLlama-13b-Instruct-hf-prontoqa) |


**Notes:** LoGiPT-[A]-[B]: The specific model version of LoGiPT
- [A]: The backbone model, which can be 'vicuna-13b-v1.5-16k', 'CodeLlama-13b-hf' or 'CodeLlama-13b-Instruct-hf'.
- [B]: The training data, which can be 'proofwriter' or 'prontoqa'.

All models are organised in Vicuna-style and trained by [FastChat-0.2.30](https://github.com/lm-sys/FastChat).
We adopt the evaluation scripts from [Logic-LM](https://github.com/teacherpeterpan/Logic-LLM).

## Dataset Details

These are the training data for **LoGiPT**.
- LoGiPT-data-ProofWriter.json: Instruction-tuning data for LoGiPT constructed from ProofWriter.
- LoGiPT-data-PrOntoQA.json: Instruction-tuning data for LoGiPT constructed from PrOntoQA.

All training examples are organised in Json-format and Vicuna-style in [jzfeng/LoGiPT-data](https://huggingface.co/datasets/jzfeng/LoGiPT-data).

### If you find these models and data helpful, please cite our NAACL'24 paper: (or Arxiv version: https://arxiv.org/abs/2311.06158)
```shell
@inproceedings{feng2024language,
  title={Language Models can be Deductive Solvers},
  author={Feng, Jiazhan and Xu, Ruochen and Hao, Junheng and Sharma, Hiteshi and Shen, Yelong and Zhao, Dongyan and Chen, Weizhu},
  booktitle={Findings of the Association for Computational Linguistics: NAACL 2024},
  pages={4026--4042},
  year={2024}
}
```
