## 生成式对话相关论文 [[Ref](https://www.jianshu.com/p/e6b58994c063)]
__Augmenting End-to-End Dialog Systems with Commonsense Knowledge__

__Topic Aware Neural Response Generation__

__Commonsense Knowledge Aware Conversation Generation with Graph Attention__ [[Paper](https://www.ijcai.org/proceedings/2018/0643.pdf)] [[Code](https://github.com/tuxchow/ccm)] [[Note](https://blog.csdn.net/tMb8Z9Vdm66wH68VX1/article/details/81518247)]
本文研究如何通过常识知识的引入提升对话模型在开放领域对话生成任务上的语言理解和生成能力。给定用户输入的语句，对话模型首先从常识知识库中检索出相关的知识图谱，然后使用一种静态的图注意力机制，将这些知识图谱编码成向量输入到编码器中，通过丰富语义知识从而提升模型对语言的理解能力。在语言生成的过程中，模型通过动态的图注意力机制根据当前解码器状态注意到合适的知识图谱以及其内的知识三元组，之后选择合适的常识知识或普通单词去生成，从而加强了模型的语言生成的信息量和知识方面的连贯性。自动评测和人工评测结果说明了我们提出的引入常识知识的对话模型可以生成语义合适且富有信息量的回复。

__Flexible End-to-End Dialogue System for Knowledge Grounded Conversation__

__A Knowledge-Grounded Neural Conversation Model__
