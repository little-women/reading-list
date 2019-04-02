# Knowledge Aware Conversation Generation with Reasoning on Augmented Graph

## 摘要

针对知识感知的开放域会话生成，研究了图中的事实知识和非结构化文档中的非事实知识两种类型的知识，其中图中的边缘信息有助于知识选择器的泛化，文本句可以为响应生成提供丰富的信息。知识三元组和句子的融合可以为会话生成提供相互加强的优势，但对此的研究较少。为了解决这一挑战，我们提出了一个由三个部分组成的知识感知聊天机、包含事实和非事实知识的增强知识图、知识选择器和响应生成器。对于图上的知识选择，我们将其表述为一个与以往的单跳知识选择模型相比更加灵活的多跳图推理问题。为了充分利用长文本信息来区分图形和其他图形，我们采用机器阅读理解技术改进了一种最先进的推理算法。我们证明，在这种统一的知识和知识选择方法的支持下，我们的系统可以生成比基线更合适和更信息化的响应。

## 1. 引言

For factoid knowledge, e.g., facts about movies, triple attributes or graph edges provide highquality candidates for knowledge selection decision, and these prior information can enhance generalization capability of knowledge selection models. But it suffers from information insufﬁciency for response generation since there is simply a single word or entity to facilitate generation. 

For nonfactoid knowledge, e.g., comments about movies, the text sentences can provide rich information for generation, but its unstructured (e.g., document based) representation scheme demands strong capability for models to perform knowledge selection or attention from the list of knowledge texts.

**Fusion of knowledge triples (or graph based representation scheme) and text sentences might yield mutually reinforcing advantages for knowledge selection in conversation systems, but there is less study on that.**

In summary, this paper makes the following contributions:
• This work is the ﬁrst attempt that uniﬁes factoid and non-factoid knowledge as a graph,
and conducts more ﬂexible multi-hop graph reasoning for knowledge selection. Supported by such knowledge and knowledge selection method, our system can respond more appropriately and informatively.
• For knowledge selection, to fully leverage long texts in vertices that differentiate our graph from others, we improve a state of the art graph reasoning algorithm (Das et al., 2018) with machine reading comprehension (MRC) technology (Seo et al., 2017).

## 2. 相关工作

### 2.1 基于知识图的对话

### 2.2 基于非结构文本的对话



## 3. 模型

### 3.1 问题定义和模型概述

### 3.2 增强知识图

### 3.3 图上的知识选择

### 3.4 Knowledge Aware Generation

## 4. 实验和结果