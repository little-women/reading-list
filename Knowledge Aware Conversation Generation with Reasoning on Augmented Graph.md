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

KG 定义为 $\mathcal{G}=\{\mathcal{V},\mathcal{E}, \mathcal{L}^{\mathcal{E}}\}​$

给定输入文本 $X=\{x_1,x_2,,x_m\}$ 和 $\mathcal{G}$

目标生成 $Y = \{y_1,y_2,,y_n\}$

分成两个阶段：

- 知识选择：最大化下面概率的节点 v，v 与 $v_X$ 联通， $v_X$ 是根据 $X$ 中的实体或者单词从图 $\mathcal{G}​$ 中检索到的节点。

  $v_Y = \arg \max_\limits{v} P_{KS}(v|v_X, \mathcal{G}, X)​$

- 回复生成：$P_{RG}(Y|X,v_Y) = \prod_\limits{t=1}^n P(y_t|y_{<t}, X, v_Y)​$

### 3.2 增强知识图

### 3.3 图上的知识选择

**任务定义**：给定一个 input query $(v_X,X)$，RL agent 从图中对应于 X 的 vertex $v_X$，游走到与 answer 对应的 $v_Y$.

**状态**：$S_t=(v_t, v_X, X, v_{gt})​$, $v_t​$ 表示 RL agent 当前位置，$v_{gt}​$ 是 ground-truth vertex。

**观测**：我们把问题定义为部分可观察的马尔科夫决策模型 (POMDP)，当前位置 $(v_t)$ 和 $(v_X, X)$ 是可观察的，ground-truth $(v_{gt})$ 是不可观察的。定义观察函数为：$O(S_t=(v_t, v_X, X, v_{gt}))=(v_t, v_X, X)​$

**Actions**: $\mathcal{A}_{S_t} = \{(v_t,l_e,v_d) \in \mathcal{E}: S_t=(v_t, v_X, X, v_{gt}), l_e\in \mathcal{L}^{\mathcal{E}},v_d\in\mathcal{V} \} \cup \{(S_t,\empty, S_t)\}​$ . 

**Transition**: $\delta(S_t, A)=(v_d,v_X,X,v_{gt})​$ ,其中 $S_t=(v_t, v_X, X, v_{gt})​$, $A=(v_t,l_e,v_d)​$

**Rewards**：$R(S_T)=I\{v_T=v_{gt}\}$, 其中$S_T=(v_T,v_X,X,v_{gt})$ 是最终状态。

**Policy**: $\pi=(d_0,d_1,...,d_{T-1})$, 其中 $d_t=P(\mathcal{A}_{S_t})$ 是在时间步 t 的一个策略。

### 3.4 Knowledge Aware Generation

## 4. 实验和结果