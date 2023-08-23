# Awesome-Efficient-LLM

A curated list for **Efficient Large Language Models**:
  - [Knowledge Distillation](#knowledge-distillation)
  - [Network Pruning](#network-pruning)
  - [Quantization](#quantization)
  - [Inference Acceleration](#inference-acceleration)
  - [Efficient Structure Design](#efficient-structure-design)
  - [Text Compression](#text-compression)
  - [Low-Rank Decomposition](#low-rank-decomposition)
  - [Survey](#Survey)
  - [Others](#others)

In light of the numerous publications that conducts experiments using PLMs (such as BERT, BART) currently, a new subdirectory [efficient_plm/](efficient_plm/) is created to house papers that are applicable to PLMs but have yet to be verified for their effectiveness on LLMs (not implying that they are not suitable on LLM). 

## Knowledge Distillation
| Title & Authors | Introduction | Links |
|:----|  :----: | :---:|
| [![Star](https://img.shields.io/github/stars/mbzuai-nlp/LaMini-LM.svg?style=social&label=Star)](https://github.com/mbzuai-nlp/LaMini-LM) <br> [LaMini-LM: A Diverse Herd of Distilled Models from Large-Scale Instructions](https://github.com/mbzuai-nlp/LaMini-LM) <br>Minghao Wu, Abdul Waheed, Chiyu Zhang, Muhammad Abdul-Mageed, Alham Fikri Aji | <img width="1002" alt="image" src="https://github.com/mbzuai-nlp/LaMini-LM/blob/main/images/lamini-pipeline.drawio.png"> | [Github](https://github.com/mbzuai-nlp/LaMini-LM) [paper](https://arxiv.org/abs/2304.14402) |
|[![Star](https://img.shields.io/github/stars/allenai/cot_distillation.svg?style=social&label=Star)](https://github.com/allenai/cot_distillation)[![Publish](https://img.shields.io/badge/Conference-ACL'23-blue)]()<br>[Symbolic Chain-of-Thought Distillation: Small Models Can Also "Think" Step-by-Step](https://arxiv.org/abs/2306.14050) <br> Liunian Harold Li, Jack Hessel, Youngjae Yu, Xiang Ren, Kai-Wei Chang, Yejin Choi |<img width="202" alt="image" src="figures/SCoTD.png"> |[Github](https://github.com/allenai/cot_distillation) <br> [Paper](https://arxiv.org/abs/2306.14050)|
|[![Star](https://img.shields.io/github/stars/FranxYao/FlanT5-CoT-Specialization.svg?style=social&label=Star)](https://github.com/FranxYao/FlanT5-CoT-Specialization)[![Publish](https://img.shields.io/badge/Conference-ICML'23-blue)]()<br>[Specializing Smaller Language Models towards Multi-Step Reasoning](https://arxiv.org/abs/2301.12726) <br> Yao Fu, Hao Peng, Litu Ou, Ashish Sabharwal, Tushar Khot |<img width="1002" alt="image" src="figures/ModelSpecialization.png"> |[Github](https://github.com/FranxYao/FlanT5-CoT-Specialization) <br> [Paper](https://arxiv.org/abs/2301.12726)|
|[![Star](https://img.shields.io/github/stars/aitsc/GLMKD.svg?style=social&label=Star)](https://github.com/aitsc/GLMKD) [![Publish](https://img.shields.io/badge/Conference-ACL'23%20Industry%20Track-blue)]() <br>[GKD: A General Knowledge Distillation Framework for Large-scale Pre-trained Language Model](https://arxiv.org/abs/2306.06629) <br> Shicheng Tan, Weng Lam Tam, Yuanchun Wang, Wenwen Gong, Yang Yang, Hongyin Tang, Keqing He, Jiahao Liu, Jingang Wang, Shu Zhao, Peng Zhang, Jie Tang |<img width="1002" alt="image" src="figures/GKD.png"> |[Github](https://github.com/aitsc/GLMKD) <br> [Paper](https://arxiv.org/abs/2306.06629)|
|[Knowledge Distillation of Large Language Models](https://arxiv.org/abs/2306.08543) <br> Yuxian Gu, Li Dong, Furu Wei, Minlie Huang |<img width="1002" alt="image" src="https://github.com/microsoft/LMOps/blob/main/minillm/figures/method.png"> |[Github](https://github.com/microsoft/LMOps/tree/main/minillm) <br> [Paper](https://arxiv.org/abs/2306.08543)|
|[![Star](https://img.shields.io/github/stars/siyuyuan/coscript.svg?style=social&label=Star)](https://github.com/siyuyuan/coscript)[![Publish](https://img.shields.io/badge/Conference-ACL'23%20Outstanding-blue)]()<br>[Distilling Script Knowledge from Large Language Models for Constrained Language Planning](https://arxiv.org/abs/2305.05252) <br> Siyu Yuan, Jiangjie Chen, Ziquan Fu, Xuyang Ge, Soham Shah, Charles Robert Jankowski, Yanghua Xiao, Deqing Yang |<img width="302" alt="image" src="figures/CoScript.png"> |[Github](https://github.com/siyuyuan/coscript) <br> [Paper](https://arxiv.org/abs/2305.05252)|
|[![Publish](https://img.shields.io/badge/Conference-ACL'23%20Outstanding-blue)]()<br>[SCOTT: Self-Consistent Chain-of-Thought Distillation](https://arxiv.org/abs/2305.01879) <br> Peifeng Wang, Zhengyang Wang, Zheng Li, Yifan Gao, Bing Yin, Xiang Ren |<img width="1002" alt="image" src="figures/SCOTT.png"> |[Paper](https://arxiv.org/abs/2305.01879)|
|[![Star](https://img.shields.io/github/stars/eric11eca/disco.svg?style=social&label=Star)](https://github.com/eric11eca/disco)[![Publish](https://img.shields.io/badge/Conference-ACL'23-blue)]()<br>[DISCO: Distilling Counterfactuals with Large Language Models](https://arxiv.org/abs/2212.10534) <br> Zeming Chen, Qiyue Gao, Antoine Bosselut, Ashish Sabharwal, Kyle Richardson |<img width="1002" alt="image" src="figures/disco.png"> |[Github](https://github.com/eric11eca/disco) <br> [Paper](https://arxiv.org/abs/2212.10534)|
|[![Star](https://img.shields.io/github/stars/allenai/i2d2.svg?style=social&label=Star)](https://github.com/allenai/i2d2)[![Publish](https://img.shields.io/badge/Conference-ACL'23-blue)]()<br>[I2D2: Inductive Knowledge Distillation with NeuroLogic and Self-Imitation](https://arxiv.org/abs/2212.09246) <br> Chandra Bhagavatula, Jena D. Hwang, Doug Downey, Ronan Le Bras, Ximing Lu, Lianhui Qin, Keisuke Sakaguchi, Swabha Swayamdipta, Peter West, Yejin Choi |<img width="1002" alt="image" src="https://i2d2.allen.ai/i2d2-fig1.png"> |[Github](https://github.com/allenai/i2d2) <br> [Paper](https://arxiv.org/abs/2212.09246) <br> [Project](https://i2d2.allen.ai/) |
|[Teaching Small Language Models to Reason](https://arxiv.org/abs/2212.08410) <br> Lucie Charlotte Magister, Jonathan Mallinson, Jakub Adamek, Eric Malmi, Aliaksei Severyn.  |<img width="202" alt="image" src="figures/Teach_Small_LM_COT.png"> |[Paper](https://arxiv.org/abs/2212.08410)|
|[![Star](https://img.shields.io/github/stars/google-research/distilling-step-by-step.svg?style=social&label=Star)](https://github.com/google-research/distilling-step-by-step) [![Publish](https://img.shields.io/badge/Conference-ACL'23%20Findings-blue)]() <br> [Distilling Step-by-Step! Outperforming Larger Language Models with Less Training Data and Smaller Model Sizes](https://arxiv.org/abs/2305.02301)    <br> Cheng-Yu Hsieh, Chun-Liang Li, Chih-Kuan Yeh, Hootan Nakhost, Yasuhisa Fujii, Alexander Ratner, Ranjay Krishna, Chen-Yu Lee, Tomas Pfister | <img width="2000" alt="image" src="figures/Distill_step_by_step.png">| [Github](https://github.com/google-research/distilling-step-by-step) <br> [Paper](https://arxiv.org/abs/2305.02301) |
| [![Star](https://img.shields.io/github/stars/ananyahjha93/llm-distill.svg?style=social&label=Star)](https://github.com/ananyahjha93/llm-distill) <br> [Large Language Model Distillation Doesn't Need a Teacher](https://arxiv.org/abs/2305.14864) <br> Ananya Harsh Jha, Dirk Groeneveld, Emma Strubell, Iz Beltagy </br> | <img width="2000" alt="image" src="figures/TeacherFreeLLM.png"> | [Github](https://github.com/ananyahjha93/llm-distill) [paper](https://arxiv.org/abs/2305.14864) |
| [The False Promise of Imitating Proprietary LLMs](https://arxiv.org/abs/2305.15717) <br> Arnav Gudibande, Eric Wallace, Charlie Snell, Xinyang Geng, Hao Liu, Pieter Abbeel, Sergey Levine, Dawn Song | <img width="400" alt="image" src="figures/FalsePromise.png"> | [Paper](https://arxiv.org/abs/2305.15717) |
|[![Star](https://img.shields.io/github/stars/jaehunjung1/impossible-distillation.svg?style=social&label=Star)](https://github.com/jaehunjung1/impossible-distillation) <br>[Impossible Distillation: from Low-Quality Model to High-Quality Dataset & Model for Summarization and Paraphrasing](https://arxiv.org/abs/2305.16635) <br> Jaehun Jung, Peter West, Liwei Jiang, Faeze Brahman, Ximing Lu, Jillian Fisher, Taylor Sorensen, Yejin Choi |<img width="1002" alt="image" src="figures/impossible_distillation.png"> |[Github](https://github.com/jaehunjung1/impossible-distillation) [paper](https://arxiv.org/abs/2305.16635) |
|[PaD: Program-aided Distillation Specializes Large Models in Reasoning](https://arxiv.org/abs/2305.13888) <br> Xuekai Zhu, Biqing Qi, Kaiyan Zhang, Xingwei Long, Bowen Zhou |<img width="402" alt="image" src="figures/PaD.png"> |[Paper](https://arxiv.org/abs/2305.13888)|
|[![Star](https://img.shields.io/github/stars/swarnaHub/ExplanationIntervention.svg?style=social&label=Star)](https://github.com/swarnaHub/ExplanationIntervention)<br>[Can Language Models Teach? Teacher Explanations Improve Student Performance via Theory of Mind](https://arxiv.org/abs/2306.09299) <br> Swarnadeep Saha, Peter Hase, and Mohit Bansal |<img width="402" alt="image" src="https://github.com/swarnaHub/ExplanationIntervention/blob/main/assets/main_fig.png"> |[Github](https://github.com/swarnaHub/ExplanationIntervention) <br> [Paper](https://arxiv.org/abs/2306.09299)|
|[RLCD: Reinforcement Learning from Contrast Distillation for Language Model Alignment](https://arxiv.org/abs/2307.12950) <br> Kevin Yang, Dan Klein, Asli Celikyilmaz, Nanyun Peng, Yuandong Tian |<img width="1002" alt="image" src="figures/RLCD.png"> |[Paper](https://arxiv.org/abs/2307.12950)|
|[Sci-CoT: Leveraging Large Language Models for Enhanced Knowledge Distillation in Small Models for Scientific QA](https://arxiv.org/abs/2308.04679) <br> Yuhan Ma, Haiqi Jiang, Chenyou Fan |<img width="1002" alt="image" src="figures/Sci-COT.png"> |[Paper](https://arxiv.org/abs/2308.04679)|
|[![Star](https://img.shields.io/github/stars/universal-ner/universal-ner.svg?style=social&label=Star)](https://github.com/universal-ner/universal-ner)<br>[UniversalNER: Targeted Distillation from Large Language Models for Open Named Entity Recognition](https://arxiv.org/abs/2308.03279) <br> Wenxuan Zhou, Sheng Zhang, Yu Gu, Muhao Chen, Hoifung Poon |<img width="1002" alt="image" src="figures/UniversalNER.png"> |[Github](https://github.com/universal-ner/universal-ner) <br> [Paper](https://arxiv.org/abs/2308.03279) <br> [Project](https://universal-ner.github.io) |
|[![Star](https://img.shields.io/github/stars/timinar/BabyLlama.svg?style=social&label=Star)](https://github.com/timinar/BabyLlama)<br>[Baby Llama: knowledge distillation from an ensemble of teachers trained on a small dataset with no performance penalty](https://arxiv.org/abs/2308.02019) <br> Inar Timiryasov, Jean-Loup Tastet |<img width="1002" alt="image" src="figures/BabyLLaMA.png"> |[Github](https://github.com/timinar/BabyLlama) <br> [Paper](https://arxiv.org/abs/2308.02019) | [Model](https://huggingface.co/timinar/baby-llama-58m) |



## Network Pruning
| Title & Authors | Introduction | Links |
|:----|  :----: | :---:|
| [![Star](https://img.shields.io/github/stars/IST-DASLab/sparsegpt.svg?style=social&label=Star)](https://github.com/IST-DASLab/sparsegpt) [![Publish](https://img.shields.io/badge/Conference-ICML'23-blue)]() [![Type](https://img.shields.io/badge/Unstructured-C2A4A6)]() <br> [SparseGPT: Massive Language Models Can Be Accurately Pruned in One-Shot](https://github.com/IST-DASLab/sparsegpt) <br> Elias Frantar, Dan Alistarh| <img width="522" alt="image" src="figures/sparsegpt.png"> |[Github](https://github.com/IST-DASLab/sparsegpt) [paper](https://arxiv.org/abs/2301.00774) |
| [![Star](https://img.shields.io/github/stars/horseee/LLM-Pruner.svg?style=social&label=Star)](https://github.com/horseee/LLM-Pruner) [![Type](https://img.shields.io/badge/Structural-C2A4A6)]() <br>[LLM-Pruner: On the Structural Pruning of Large Language Models](https://arxiv.org/abs/2305.11627) <br> Xinyin Ma, Gongfan Fang, Xinchao Wang | <img width="561" alt="image" src="figures/llm_pruner.png">| [Github](https://github.com/horseee/LLM-Pruner) [paper](https://arxiv.org/abs/2305.11627)|
|[![Star](https://img.shields.io/github/stars/locuslab/wanda.svg?style=social&label=Star)](https://github.com/locuslab/wanda) [![Type](https://img.shields.io/badge/Unstructured-C2A4A6)]()<br>[A Simple and Effective Pruning Approach for Large Language Models](https://arxiv.org/abs/2306.11695) <br> Mingjie Sun, Zhuang Liu, Anna Bair, J. Zico Kolter |<img width="1002" alt="image" src="https://user-images.githubusercontent.com/20168304/245999360-f951de47-269d-491d-826a-8e6d85627849.png"> |[Github](https://github.com/locuslab/wanda) <br> [Paper](https://arxiv.org/abs/2306.11695)|


## Quantization
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/IST-DASLab/gptq.svg?style=social&label=Star)](https://github.com/IST-DASLab/gptq)[![Publish](https://img.shields.io/badge/Conference-ICLR'22-blue)]()<br>[GPTQ: Accurate Post-Training Quantization for Generative Pre-trained Transformers](https://arxiv.org/abs/2210.17323) <br> Elias Frantar, Saleh Ashkboos, Torsten Hoefler, Dan Alistarh |<img width="202" alt="image" src="figures/GPTQ.png"> |[Github](https://github.com/IST-DASLab/gptq) <br> [Paper](https://arxiv.org/abs/2210.17323)|
| [![Star](https://img.shields.io/github/stars/qwopqwop200/GPTQ-for-LLaMa.svg?style=social&label=Star)](https://github.com/qwopqwop200/GPTQ-for-LLaMa) <br>[GPTQ-for-LLaMA](https://github.com/qwopqwop200/GPTQ-for-LLaMa): 4 bits quantization of LLaMA using GPTQ. | <img width="102" alt="image" src="https://user-images.githubusercontent.com/64115820/235287009-2d07bba8-9b85-4973-9e06-2a3c28777f06.png"> |[Github](https://github.com/qwopqwop200/GPTQ-for-LLaMa)|
|[![Star](https://img.shields.io/github/stars/mit-han-lab/smoothquant.svg?style=social&label=Star)](https://github.com/mit-han-lab/smoothquant)[![Publish](https://img.shields.io/badge/Conference-ICML'23-blue)]() <br>[SmoothQuant: Accurate and Efficient Post-Training Quantization for Large Language Models](https://arxiv.org/abs/2211.10438) <br> Guangxuan Xiao, Ji Lin, Mickael Seznec, Hao Wu, Julien Demouth, Song Han |<img width="1002" alt="image" src="https://github.com/mit-han-lab/smoothquant/blob/main/figures/intuition.png"> |[Github](https://github.com/mit-han-lab/smoothquant) <br> [Paper](https://arxiv.org/abs/2211.10438)|
|[![Star](https://img.shields.io/github/stars/mit-han-lab/llm-awq.svg?style=social&label=Star)](https://github.com/mit-han-lab/llm-awq) <br>[AWQ: Activation-aware Weight Quantization for LLM Compression and Acceleration](https://arxiv.org/abs/2306.00978) <br> Ji Lin, Jiaming Tang, Haotian Tang, Shang Yang, Xingyu Dang, Song Han |<img width="1002" alt="image" src="https://github.com/mit-han-lab/llm-awq/blob/main/figures/overview.png"> |[Github](https://github.com/mit-han-lab/llm-awq) <br> [Paper](https://arxiv.org/abs/2306.00978)|
| [![Star](https://img.shields.io/github/stars/hahnyuan/RPTQ4LLM.svg?style=social&label=Star)](https://github.com/hahnyuan/RPTQ4LLM) <br>[RPTQ: Reorder-based Post-training Quantization for Large Language Models](https://arxiv.org/abs/2304.01089) <br> Zhihang Yuan and Lin Niu and Jiawei Liu and Wenyu Liu and Xinggang Wang and Yuzhang Shang and Guangyu Sun and Qiang Wu and Jiaxiang Wu and Bingzhe Wu | ![](https://github.com/hahnyuan/RPTQ4LLM/blob/master/ims/cover.png) | <br>[Github](https://github.com/hahnyuan/RPTQ4LLM)</br> [Paper](https://arxiv.org/abs/2304.01089) |
| [![Star](https://img.shields.io/github/stars/artidoro/qlora.svg?style=social&label=Star)](https://github.com/artidoro/qlora) <br>[QLoRA: Efficient Finetuning of Quantized LLMs](https://arxiv.org/abs/2305.14314) <br> Tim Dettmers, Artidoro Pagnoni, Ari Holtzman, Luke Zettlemoyer | ![](figures/qlora.png) | <br>[Github](https://github.com/artidoro/qlora)</br> [Paper](https://arxiv.org/abs/2305.14314) |
|[ZeroQuant-V2: Exploring Post-training Quantization in LLMs from Comprehensive Study to Low Rank Compensation](https://arxiv.org/abs/2303.08302) <br> Zhewei Yao, Xiaoxia Wu, Cheng Li, Stephen Youn, Yuxiong He |<img width="402" alt="image" src="figures/zeroquant-v2.png"> |[Paper](https://arxiv.org/abs/2303.08302)|
| [![Star](https://img.shields.io/github/stars/SqueezeAILab/SqueezeLLM.svg?style=social&label=Star)](https://github.com/SqueezeAILab/SqueezeLLM) <br>[SqueezeLLM: Dense-and-Sparse Quantization](https://arxiv.org/pdf/2306.07629.pdf) <br>Sehoon Kim, Coleman Hooper, Amir Gholami, Zhen Dong, Xiuyu Li, Sheng Shen, Michael W. Mahoney, Kurt Keutzer | <img width="1102" alt="image" src="figures/SqueezeLLM.png"> |[Github](https://github.com/SqueezeAILab/SqueezeLLM) <br> [Paper](https://arxiv.org/pdf/2306.07629.pdf)|
| [Outlier Suppression+: Accurate quantization of large language models by equivalent and optimal shifting and scaling](https://arxiv.org/abs/2304.09145v1) <br> Xiuying Wei , Yunchen Zhang, Yuhang Li, Xiangguo Zhang, Ruihao Gong, Jinyang Guo, Xianglong Liu|  <img width="1102" alt="image" src="figures/outliersuppression.png"> | [Paper](https://arxiv.org/abs/2304.09145v1)|
|[Integer or Floating Point? New Outlooks for Low-Bit Quantization on Large Language Models](https://arxiv.org/abs/2305.12356) <br> Yijia Zhang, Lingran Zhao, Shijie Cao, Wenqiang Wang, Ting Cao, Fan Yang, Mao Yang, Shanghang Zhang, Ningyi Xu |<img width="1002" alt="image" src="figures/MoFQ.png"> |[Paper](https://arxiv.org/abs/2305.12356)|
|[LLM-QAT: Data-Free Quantization Aware Training for Large Language Models](https://arxiv.org/abs/2305.17888) <br> Zechun Liu, Barlas Oguz, Changsheng Zhao, Ernie Chang, Pierre Stock, Yashar Mehdad, Yangyang Shi, Raghuraman Krishnamoorthi, Vikas Chandra |<img width="1002" alt="image" src="figures/LLM-QAT.png"> |[Paper](https://arxiv.org/abs/2305.17888)|
|[![Star](https://img.shields.io/github/stars/Vahe1994/SpQR.svg?style=social&label=Star)](https://github.com/Vahe1994/SpQR) <br>[SpQR: A Sparse-Quantized Representation for Near-Lossless LLM Weight Compression](https://arxiv.org/abs/2306.03078) <br> Tim Dettmers, Ruslan Svirschevski, Vage Egiazarian, Denis Kuznedelev, Elias Frantar, Saleh Ashkboos, Alexander Borzunov, Torsten Hoefler, Dan Alistarh |<img width="1002" alt="image" src="figures/SpQR.png"> |[Github](https://github.com/Vahe1994/SpQR) <br> [Paper](https://arxiv.org/abs/2306.03078)|
|[![Star](https://img.shields.io/github/stars/xvyaward/owq.svg?style=social&label=Star)](https://github.com/xvyaward/owq) <br>[OWQ: Lessons learned from activation outliers for weight quantization in large language models](https://arxiv.org/abs/2306.02272) <br> Changhun Lee, Jungyu Jin, Taesu Kim, Hyungjun Kim, Eunhyeok Park |<img width="1002" alt="image" src="figures/OWQ.png"> |[Github](https://github.com/xvyaward/owq) <br> [Paper](https://arxiv.org/abs/2306.02272)|
|[![Star](https://img.shields.io/github/stars/RUCAIBox/QuantizedEmpirical.svg?style=social&label=Star)](https://github.com/RUCAIBox/QuantizedEmpirical)<br>[Do Emergent Abilities Exist in Quantized Large Language Models: An Empirical Study](https://arxiv.org/abs/2307.08072) <br> Peiyu Liu, Zikang Liu, Ze-Feng Gao, Dawei Gao, Wayne Xin Zhao, Yaliang Li, Bolin Ding, Ji-Rong Wen |<img width="1002" alt="image" src="figures/QuantizedEmpirical.png"> |[Github](https://github.com/RUCAIBox/QuantizedEmpirical) <br> [Paper](https://arxiv.org/abs/2307.08072)|
|[ZeroQuant-FP: A Leap Forward in LLMs Post-Training W4A8 Quantization Using Floating-Point Formats](https://arxiv.org/abs/2307.09782) <br> Xiaoxia Wu, Zhewei Yao, Yuxiong He |<img width="1002" alt="image" src="figures/ZeroQuant-FP.png"> |[Paper](https://arxiv.org/abs/2307.09782)|
|[![Star](https://img.shields.io/github/stars/jerry-chee/QuIP.svg?style=social&label=Star)](https://github.com/jerry-chee/QuIP)<br>[QuIP: 2-Bit Quantization of Large Language Models With Guarantees](https://arxiv.org/abs/2307.13304) <br> Jerry Chee, Yaohui Cai, Volodymyr Kuleshov, Christopher De SaXQ |<img width="302" alt="image" src="figures/QuIP.png"> |[Github](https://github.com/jerry-chee/QuIP) <br> [Paper](https://arxiv.org/abs/2307.13304)|


## Inference Acceleration
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/FMInference/DejaVu.svg?style=social&label=Star)](https://github.com/FMInference/DejaVu)[![Publish](https://img.shields.io/badge/Conference-ICML'23%20Oral-blue)]()<br>[Deja Vu: Contextual Sparsity for Efficient LLMs at Inference Time](https://openreview.net/forum?id=wIPIhHd00i) <br> Zichang Liu, Jue WANG, Tri Dao, Tianyi Zhou, Binhang Yuan, Zhao Song, Anshumali Shrivastava, Ce Zhang, Yuandong Tian, Christopher Re, Beidi Chen |<img width="202" alt="image" src="figures/DajeVu.png"> |[Github](https://github.com/FMInference/DejaVu) <br> [Paper](https://openreview.net/forum?id=wIPIhHd00i)|
| [Inference with Reference: Lossless Acceleration of Large Language Models](https://arxiv.org/abs/2304.04487) <br> Nan Yang, Tao Ge, Liang Wang, Binxing Jiao, Daxin Jiang, Linjun Yang, Rangan Majumder, Furu Wei | <img width="600" alt="image" src="figures/llma.png"> | [Github](https://github.com/microsoft/LMOps/tree/main/llma) <br> [paper](https://arxiv.org/abs/2304.04487) |
| [![Star](https://img.shields.io/github/stars/flexflow/FlexFlow.svg?style=social&label=Star)](https://github.com/flexflow/FlexFlow/tree/inference) <br> [SpecInfer: Accelerating Generative LLM Serving with Speculative Inference and Token Tree Verification](https://arxiv.org/abs/2305.09781) <br> Xupeng Miao, Gabriele Oliaro, Zhihao Zhang, Xinhao Cheng, Zeyu Wang, Rae Ying Yee Wong, Zhuoming Chen, Daiyaan Arfeen, Reyna Abhyankar, Zhihao Jia| <img width="600" alt="image" src="https://github.com/flexflow/FlexFlow/blob/inference/img/overview.png">| [Github](https://github.com/flexflow/FlexFlow/tree/inference) <br> [paper](https://arxiv.org/abs/2305.09781) |
|[Scissorhands: Exploiting the Persistence of Importance Hypothesis for LLM KV Cache Compression at Test Time](https://arxiv.org/abs/2305.17118) <br> Zichang Liu, Aditya Desai, Fangshuo Liao, Weitao Wang, Victor Xie, Zhaozhuo Xu, Anastasios Kyrillidis, Anshumali Shrivastava |<img width="302" alt="image" src="figures/Scissorhands.png"> |[Paper](https://arxiv.org/abs/2305.17118)|
|[Dynamic Context Pruning for Efficient and Interpretable Autoregressive Transformers](https://arxiv.org/abs/2305.15805) <br> Sotiris Anagnostidis, Dario Pavllo, Luca Biggio, Lorenzo Noci, Aurelien Lucchi, Thomas Hofmann |<img width="1602" alt="image" src="figures/DCP.png"> |[Paper](https://arxiv.org/abs/2305.15805)|
|[SkipDecode: Autoregressive Skip Decoding with Batching and Caching for Efficient LLM Inference](https://arxiv.org/abs/2307.02628) <br> Luciano Del Corro, Allie Del Giorno, Sahaj Agarwal, Bin Yu, Ahmed Awadallah, Subhabrata Mukherjee |<img width="1002" alt="image" src="figures/SkipDecode.png"> |[Paper](https://arxiv.org/abs/2307.02628)|
|[Skeleton-of-Thought: Large Language Models Can Do Parallel Decoding](https://arxiv.org/abs/2307.15337) <br> Xuefei Ning, Zinan Lin, Zixuan Zhou, Huazhong Yang, Yu Wang |<img width="1002" alt="image" src="figures/SoT.png"> |[Paper](https://arxiv.org/abs/2307.15337)|
|[![Publish](https://img.shields.io/badge/Conference-ICML'2023%20ES%20FOMO-blue)]()<br>[Accelerating LLM Inference with Staged Speculative Decoding](https://arxiv.org/abs/2308.04623) <br> Benjamin Spector, Chris Re |<img width="302" alt="image" src="figures/StagedSpec.png"> |[Paper](https://arxiv.org/abs/2308.04623)|

## Efficient Structure Design
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/Dao-AILab/flash-attention.svg?style=social&label=Star)](https://github.com/Dao-AILab/flash-attention)[![Publish](https://img.shields.io/badge/Conference-NeurIPS'22-blue)]()<br>[FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness](https://arxiv.org/abs/2205.14135) <br> Tri Dao, Daniel Y. Fu, Stefano Ermon, Atri Rudra, Christopher Ré |<img width="1002" alt="image" src="https://github.com/Dao-AILab/flash-attention/blob/main/assets/flashattn_banner.jpg"> |[Github](https://github.com/Dao-AILab/flash-attention) <br> [Paper](https://arxiv.org/abs/2205.14135)|
|[![Star](https://img.shields.io/github/stars/Dao-AILab/flash-attention.svg?style=social&label=Star)](https://github.com/Dao-AILab/flash-attention)<br>[FlashAttention-2: Faster Attention with Better Parallelism and Work Partitioning](https://arxiv.org/pdf/2307.08691.pdf) <br> Tri Dao |<img width="1002" alt="image" src="figures/FlashAttention2.png"> |[Github](https://github.com/Dao-AILab/flash-attention) <br> [Paper](https://arxiv.org/pdf/2307.08691.pdf)|


## Text Compression
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[LLMZip: Lossless Text Compression using Large Language Models](https://arxiv.org/abs/2306.04050) <br> Chandra Shekhara Kaushik Valmeekam, Krishna Narayanan, Dileep Kalathil, Jean-Francois Chamberland, Srinivas Shakkottai |<img width="1002" alt="image" src="figures/LLMZip.png"> |[Paper](https://arxiv.org/abs/2306.04050) \| [Unofficial Github](https://github.com/erika-n/GPTzip)|
|[![Star](https://img.shields.io/github/stars/princeton-nlp/AutoCompressors.svg?style=social&label=Star)](https://github.com/princeton-nlp/AutoCompressors)<br>[Adapting Language Models to Compress Contexts](https://arxiv.org/abs/2305.14788) <br> Alexis Chevalier, Alexander Wettig, Anirudh Ajith, Danqi Chen |<img width="302" alt="image" src="figures/AutoCompressor.png"> |[Github](https://github.com/princeton-nlp/AutoCompressors) <br> [Paper](https://arxiv.org/abs/2305.14788)|
|[In-context Autoencoder for Context Compression in a Large Language Model](https://arxiv.org/abs/2307.06945) <br> Tao Ge, Jing Hu, Xun Wang, Si-Qing Chen, Furu Wei |<img width="1002" alt="image" src="figures/ICAE.png"> |[Paper](https://arxiv.org/abs/2307.06945)|


## Low-Rank Decomposition
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[![Star](https://img.shields.io/github/stars/yxli2123/LoSparse.svg?style=social&label=Star)](https://github.com/yxli2123/LoSparse) [![Publish](https://img.shields.io/badge/Conference-ICML'23-blue)]() <br>[LoSparse: Structured Compression of Large Language Models based on Low-Rank and Sparse Approximation](https://arxiv.org/abs/2306.11222) <br> Yixiao Li, Yifan Yu, Qingru Zhang, Chen Liang, Pengcheng He, Weizhu Chen, Tuo Zhao |<img width="302" alt="image" src="figures/LoSparse.png"> |[Github](https://github.com/yxli2123/LoSparse) <br> [Paper](https://arxiv.org/abs/2306.11222)|
|[TensorGPT: Efficient Compression of the Embedding Layer in LLMs based on the Tensor-Train Decomposition](https://arxiv.org/abs/2307.00526) <br> Mingxue Xu, Yao Lei Xu, Danilo P. Mandic |<img width="1002" alt="image" src="figures/TT-SVD.png"> |[Paper](https://arxiv.org/abs/2307.00526)|


## Survey
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[A Survey on Model Compression for Large Language Models](https://arxiv.org/abs/2308.07633) <br> Xunyu Zhu, Jian Li, Yong Liu, Can Ma, Weiping Wang |<img width="1002" alt="image" src="figures/survey_xunyu.png"> |[Paper](https://arxiv.org/abs/2308.07633)|

## Others
| Title & Authors | Introduction | Links |
|:--|  :----: | :---:|
|[CPET: Effective Parameter-Efficient Tuning for Compressed Large Language Models](https://arxiv.org/abs/2307.07705) <br> Weilin Zhao, Yuxiang Huang, Xu Han, Zhiyuan Liu, Zhengyan Zhang, Maosong Sun |<img width="402" alt="image" src="figures/CPET.png"> |[Paper](https://arxiv.org/abs/2307.07705)|
