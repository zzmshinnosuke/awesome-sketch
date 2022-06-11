
[Multi-Graph Transformer for Free-Hand Sketch Recognition](https://arxiv.org/abs/1912.11258), TNNLS, 2021, [[code]](https://github.com/PengBoXiangShang/multigraph_transformer)
- 这是一篇结合graph和transformer做草图识别的文章，源码按照README很容易跑起来。
- 文中使用QuickDraw数据集，对于每张草图提取前100个关键点，对于多于100个点进行截断，对于少于100个点补(-1,-1)(padding)操作。每个节点表示为一个4维的向量，前两位是该节点在的横纵坐标，第三位用于描述节点的标注状态，第四位是位置编码。对坐标使用Linear，对状态和位置使用nn.Embedding 都是映射到512维，拼接起来512*3维。
- MultiGraph 使用了关键点的跳连接（k-hop）分为三种来构建邻接矩阵（初始化为-1e10）：1-hop 属于同一个笔画的点按顺序连接； 2-hop 属于同一个笔画的点间隔连接；global 相邻笔画的末点和首点连接。
- 实验结果，MGT所取得的识别结果远高于LSTM和GRU，还超越了大部分的CNN网络，低于Inception V3和MobileNet V2。