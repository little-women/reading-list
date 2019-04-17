## TODO
**Mem2Seq**: "Mem2Seq: Effectively Incorporating Knowledge Bases into End-to-End Task-Oriented Dialog Systems". ACL(2018) [[Paper]](https://arxiv.org/pdf/1804.08217v3.pdf) [[code]](https://github.com/HLTCHKUST/Mem2Seq) :star::star::star::star::star:

**GTTP**: "Towards Exploiting Background Knowledge for Building Conversation Systems". EMNLP(2018)  [[Paper]](https://arxiv.org/pdf/1809.08205v1.pdf) [[code]](https://github.com/nikitacs16/Holl-E) :star::star::star::star::star:

**HERD**: "Building end-to-end dialogue systems using generative hierarchical neural network models." In Proceedings of AAAI (2016) [[Paper](https://arxiv.org/pdf/1507.04808v3.pdf)] [[code]](https://github.com/julianser/hed-dlg-truncated)

## DONE [[Summarize]](Summarize.md)
**MemNet**:  "A knowledge-groundedneural conversation model." In Proceedings of AAAI 2018.  [[Paper]](https://arxiv.org/pdf/1702.01932v2.pdf) [[code]](https://github.com/mgalley/DSTC7-End-to-End-Conversation-Modeling) [[Note]](http://www.sohu.com/a/129408533_642762)

**CopyNet (GenDS)**: "Flexible End-to-End Dialogue System for Knowledge Grounded Conversation". [[Paper](https://arxiv.org/pdf/1709.04264.pdf)]

**CCM**: "Commonsense Knowledge Aware Conversation Generation with Graph Attention." IJCAIECAI(2018) [[Paper](https://www.ijcai.org/proceedings/2018/0643.pdf)] [[Code](https://github.com/tuxchow/ccm)] [[Note](https://blog.csdn.net/tMb8Z9Vdm66wH68VX1/article/details/81518247)]

**DSTC7 (Wechat)**: “Cluster-based Beam Search for Pointer-Generator Chatbot Grounded by Knowledge”.  [[Paper](http://workshop.colips.org/dstc7/papers/03.pdf)] [[News](https://mp.weixin.qq.com/s/Jnp6jmy-8lloI7p4dAofKg)] [[Note](https://zhuanlan.zhihu.com/p/57571861)]

**DAWnet**: "Chat More: Deepening and Widening the Chatting Topic via A Deep Model". SIGIR(2018) [[PDF]](https://sigirdawnet.wixsite.com/dawnet) [[code]](https://sigirdawnet.wixsite.com/dawnet) [[Note]](http://tech.ifeng.com/a/20180424/44967077_0.shtml)

**AKGCM (Baidu)**: “Knowledge Aware Conversation Generation with Reasoning on Augmented Graph” 2019. [[Paper](https://arxiv.org/pdf/1903.10245v1.pdf)] [[Note](AKGCM.md)] 

## Reading List
### 生成式对话相关论文 [[Ref1](https://www.jianshu.com/p/e6b58994c063)] [[Ref2]](https://blog.csdn.net/qq_36301716/article/details/80071361)
__Augmenting End-to-End Dialog Systems with Commonsense Knowledge__ [[Paper](https://arxiv.org/pdf/1709.05453.pdf)]

__Topic Aware Neural Response Generation__ [[Paper](https://arxiv.org/pdf/1606.08340.pdf)]

__Commonsense Knowledge Aware Conversation Generation with Graph Attention__ [[Paper](https://www.ijcai.org/proceedings/2018/0643.pdf)] [[Code](https://github.com/tuxchow/ccm)] [[Note](https://blog.csdn.net/tMb8Z9Vdm66wH68VX1/article/details/81518247)]

__Flexible End-to-End Dialogue System for Knowledge Grounded Conversation__ [[Paper](https://arxiv.org/pdf/1709.04264.pdf)]

### 第七届对话系统技术挑战赛（DSTC7）[[Home](http://workshop.colips.org/dstc7/)] [[Task Description](http://workshop.colips.org/dstc7/proposals/DSTC7-MSR_end2end.pdf)]

__(微信) Cluster-based Beam Search for Pointer-Generator Chatbot Grounded by Knowledge__ [[Paper](http://workshop.colips.org/dstc7/papers/03.pdf)] [[News](https://mp.weixin.qq.com/s/Jnp6jmy-8lloI7p4dAofKg)] [[Note](https://zhuanlan.zhihu.com/p/57571861)]

### Existing works or baselines

**Seq2Seq**: which is widely used in open-domain conversational systems. 

> Ilya Sutskever, Oriol Vinyals, and Quoc V Le. 2014. Sequence to sequence learning with neural networks. In Proceedings of NIPS, pages 3104–3112.

**HRED**:  A hierarchical recurrent encoder-decoder model

> Iulian Vlad Serban, Alessandro Sordoni, Yoshua Bengio, Aaron C. Courville, and Joelle Pineau. 2016. Building end-to-end dialogue systems using generative hierarchical neural network models. In Proceedings of AAAI, pages 3776–3784.

**MemNet**: an end-to-end knowledge-grounded generation model, where top-k knowledge text candidates are selected by another retrieval model and then are stored into the memory units for generation. 

> Marjan Ghazvininejad, Chris Brockett, Ming-Wei Chang, Bill Dolan, Jianfeng Gao, Wen tau Yih, and Michel Galley. 2018. A knowledge-groundedneural conversation model. In Proceedings of AAAI 2018, pages 5110–5117.

**CCM**: an end-to-end commonsense conversational model, their model cannot effectively process long texts in vertices.

> Hao Zhou, Tom Young, Minlie Huang, Haizhou Zhao, Jingfang Xu, and Xiaoyan Zhu. 2018. Commonsense knowledge aware conversation generation with graph attention. In Proceedings of IJCAIECAI, pages 4623–4629. 

### [NLP 资源合集](NLP.md)
