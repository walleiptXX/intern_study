MiniCPM 是面壁与清华大学自然语言处理实验室共同开源的系列端侧语言大模型，主体语言模型 MiniCPM-2B 仅有 24亿（2.4B）的非词嵌入参数量。
● 经过 SFT 后，MiniCPM 在公开综合性评测集上，MiniCPM 与 Mistral-7B相近（中文、数学、代码能力更优），整体性能超越 Llama2-13B、MPT-30B、Falcon-40B 等模型。
● 经过 DPO 后，MiniCPM 在当前最接近用户体感的评测集 MTBench上，MiniCPM-2B 也超越了 Llama2-70B-Chat、Vicuna-33B、Mistral-7B-Instruct-v0.1、Zephyr-7B-alpha 等众多代表性开源大模型。
● 以 MiniCPM-2B 为基础构建端侧多模态大模型 MiniCPM-V，整体性能在同规模模型中实现最佳，超越基于 Phi-2 构建的现有多模态大模型，在部分评测集上达到与 9.6B Qwen-VL-Chat 相当甚至更好的性能。
● 经过 Int4 量化后，MiniCPM 可在手机上进行部署推理，流式输出速度略高于人类说话速度。MiniCPM-V 也首次跑通了多模态大模型在手机上的部署。
● 一张1080/2080可高效参数微调，一张3090/4090可全参数微调，一台机器可持续训练 MiniCPM，二次开发成本较低。
我们将完全开源MiniCPM-2B的模型参数供学术研究和有限商用，以及训练过程中的所有Checkpoint和大部分非专有数据供模型机理研究。
● 基于MiniCPM-2B的指令微调与人类偏好对MiniCPM-2B-SFT/DPO。
● 基于MiniCPM-2B的多模态模型MiniCPM-V，能力超越基于Phi-2的同参数级别多模态模型**。**
● MiniCPM-2B-SFT/DPO的Int4量化版MiniCPM-2B-SFT/DPO-Int4。
● 基于MLC-LLM、LLMFarm开发的MiniCPM手机端程序，文本及多模态模型均可在手机端进行推理。