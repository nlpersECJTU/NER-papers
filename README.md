Paper List for NER

## Nested named entity recognition

- Tan等。 Boundary Enhanced Neural Span Classification for Nested Named Entity Recognition（AAAI2020）. [paper](http://www.researchgate.net/publication/342542944_Boundary_Enhanced_Neural_Span_Classification_for_Nested_Named_Entity_Recognition)
<br>简介：提出了一种边界增强型神经跨度分类模型。除了对跨度进行分类之外，还加入一个额外的边界检测任务来预测那些作为实体边界的单词。边界检测模型能够生成高质量的候选跨度，大大降低了推理过程的时间复杂度。

- Zheng等。 - 2019 - A Boundary-aware Neural Model for Nested Named Entity Recognition(EMNLP2019)  提出了一种基于边界感知的神经网络模型。该模型利用实体边界预测实体类别标签，引入多任务学习方法，捕获实体边界及其分类标签的依赖关系，提高识别实体的性能。[paper](https://www.aclweb.org/anthology/D19-1034/) [code](https://github.com/thecharm/boundary-aware-nested-ner)

- Wang等。 HIT: Nested Named Entity Recognition via Head-Tail Pair and Token Interaction（2020EMNLP）。提出了一种新的嵌套NER模型HIT。提出属于嵌套命名实体的两个关键属性，包括(1)显式的边界字符;(2)边界内字符之间的内部联系紧密。具体地，设计(1基于多头自注意机制的头尾部检测器和双仿射分类器检测边界标记，以及(2)标记交互标记器基于传统的序列标记方法来表征边界内的内部标记连接。[paper](https://www.researchgate.net/publication/347234290_HIT_Nested_Named_Entity_Recognition_via_Head-Tail_Pair_and_Token_Interaction)

- luo等。Bipartite Flat-Graph Network for Nested Named Entity Recognition (2020ACL)。提出了一种用于嵌套命名实体识别(nested NER)的二部平面图网络(BiFlaG)，该网络包含两个子图模块:一个用于最外层实体的平面平面图模块和一个用于所有位于内层实体的图模块。以前的模型只考虑从最内层到外层(或从外到内)的信息单向传递，而我们的模型有效地捕获了它们之间的双向交互。从图形模块中学习到的更丰富的表示包含了内部实体的依赖关系，可以用来改进最外层实体的预测。[paper](https://www.aclweb.org/anthology/2020.acl-main.571/)  [code](https://github.com/cslydia/BiFlaG)
- ju等。 A Neural Layered Model for Nested Named Entity Recognition（2018NAACL）。多数命名实体识别(NER)系统只处理普通实体，而忽略内部嵌套实体，无法捕获底层文本中的细粒度语义信息。为了解决这一问题，我们提出了一种新的神经模型，通过动态叠加平面NER层来识别嵌套实体。[paper](https://www.aclweb.org/anthology/N18-1131/).[code](https://github.com/meizhiju/layered-bilstm-crf)
- Wang等。 A Neural Transition-based Model for Nested Mention Recognition（2018EMNLP）。首先将带有嵌套实体的句子映射到指定的森林，其中每个实体对应于森林的一个组成部分。基于shift-reduce的系统通过一个最大长度保证为句子长度三倍的动作序列，学习以自底向上的方式构建森林结构，在Stack-LSTM的基础上，系统进一步结合了一个基于字符的组件来捕获字母级别的模式。[paper](https://www.aclweb.org/anthology/D18-1124/) [code](https://github.com/fishjh2/merge_label)
- Fisher等。 Merge and Label: A novel neural network architecture for nested NER（2019ACL）。引入一种新的神经网络体系结构，它首先将token或实体合并到形成嵌套结构的实体中，然后分别对它们进行标记。与以前的工作不同，我们的合并和标签方法预测实值而不是离散的分割结构，这允许它结合单词和嵌套实体嵌入，同时保持可微性。[paper](https://www.aclweb.org/anthology/P19-1585.pdf)  [code](https://github.com/fishjh2/merge_label)
- Katiyar等。 Nested Named Entity Recognition Revisited（2018NAACL）。提出了一种基于RNN网络的嵌套命名实体识别和嵌套实体提及检测方法，在LSTM网络中加入Top Hidden Layer和label embeddings，提取特征学习嵌套实体的超图表示。[paper](https://www.aclweb.org/anthology/N18-1079/)
- Wang等。 Pyramid: A Layered Model for Nested Named Entity Recognition（2020ACL）。提出了一种新的嵌套命名实体识别分层模型——金字塔模型。在本文的方法中，标记或文本区域嵌入递归地输入到平面NER层中，从下到上，以金字塔的形状堆叠。还设计了一个反向金字塔，以允许层之间的双向交互。[paper](https://www.aclweb.org/anthology/2020.acl-main.525/) [code](https://github.com/Nicozwy/Pyramid)
- Li等。A Unified MRC Framework for Named Entity Recognition（2020ACL）第一次提出了将嵌套命名实体识别任务转换成机器阅读任务，采用构建数据集中所用的注释指导原则方式生成阅读理解问题，然后利用机器阅读模型求解问题。[paper](https://www.aclweb.org/anthology/2020.acl-main.519/)  [code](https://github.com/ShannonAI/mrc-for-flat-nested-ner)
- Long等。Hierarchical Region Learning for Nested Named Entity Recognition（2020EMNLP）为了解决嵌套命名实体文本片段分类方法中存在的问题，运用短语结构中的知识，定义两个相连文本片段的相关程度，根据这个相关程度从底向上生成整个句子的所有候选文本片段，大大降低了时间复杂度，提高嵌套实体识别的性能。[paper](https://www.aclweb.org/anthology/2020.findings-emnlp.430/)

## Named entity recognition
- Ma 等。 - 2020 - Simplify the Usage of Lexicon in Chinese NER（ACL2020）提出了一种简单但有效的方法，将词的信息融合到基于字的表示中，避免了设计复杂的序列标注结构，适用于其他的NER神经网络模型。这种方法基于softword，通过构建BMES集合的方式获取词的信息，最后将词的信息融合到字的表示中。[paper](https://www.researchgate.net/publication/335233357_Simplify_the_Usage_of_Lexicon_in_Chinese_NER)  [code](https://github.com/v-mipeng/LexiconAugmentedNER)
- jie等。 Dependency-Guided LSTM-CRF for Named Entity Recognition（2019EMNLP）。提出了一种简单但高效的依赖指导LSTM-CRF模型，能够编码完整的依赖树，并为命名实体识别任务捕获词的长距离和句法关系——通过这些关系能有效地推断出某些实体。分析表明，显著的改进主要来自依赖树提供的依赖关系和远程交互。[paper](https://www.aclweb.org/anthology/D19-1399.pdf)  [code](http://www.statnlp.org/research/information-extraction)

## Others
- Tian等。 - Joint ChineseWord Segmentation and Part-of-speech Tagging via Two-way Attentions of Auto-analyzed Knowledge（ACL2020）。提出了一种用于中文分词和词性标注联合任务的神经网络模型TWASP，遵循基于字符的序列标注，使用双向注意机制将每个输入字符的上下文特征及其对应的句法知识结合起来。双向注意机制用于结合上下文特征及其对应的语法知识的每个输入字符，使用现有的语言处理工具包来获取上下文的自动分析语法知识。[paper](https://www.aclweb.org/anthology/2020.acl-main.735/)
