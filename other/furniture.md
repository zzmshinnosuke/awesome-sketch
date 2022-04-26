
- [Sketch2Scene: Sketch-based Co-retrieval and Co-placement of 3D Models](https://cg.cs.tsinghua.edu.cn/sketch2scene/sketch2scene_paper.pdf), TOG, 2013  
 Pipeline：一篇比较早的草图检索和摆放3D家具的文章。首先对绘制完成的草图（应该是2D的）进行分割，通过用户自己构建层的概念分割，或者通过交互工具来实现（没有实现分割功能）；然后对于每个分割草图检索一个3D物体候选集，再找个一个最佳的候选物体的组合；最后再根据草图描述的空间约束关系，将3D物体放置在合适的位置，同时也会同步地优化物体的位置和方向根据草图和局部空间配置。  
 Stuctural Groups（没有使用概率模型，而是当做一个组合优化问题，通过草图诱导的可能的物体组合找到一个和数据库汇总场景最相似的最优的场景，在物体组合和空间配置）：（1）如何评估局部相似性在合成场景和数据集中场景？考虑到一些关系出现较多，是更可靠的，其他关系出现较少对草图语义的决定性较小。可以通过总结场景中有依赖的局部结构，从库中提取结构组集。通过评估合成草图和结构组而不是跟仓库比较。  
 这个结构组是Graph，节点代表物体类别，边代表物体间的关系。  
 Co-retrieval：草图 通过提取深度图轮廓和Canny lines来获取的，和提取普通图像的Canny lines来获取。检索使用[Sketch-Based Shape Retrieval](https://dl.acm.org/doi/pdf/10.1145/2185520.2185527?casa_token=Y6lhTAhlhRYAAAAA:EY4OZHzpCbctB4s466KgCf6B6VMU2KpRvEjtYvragD1X-Q_9SXZTLt9xNpDYoZGND5ZLsNIx38cWpCY)中的方法。然后又通过Shape Contxt（可以给出一个距离）来对检索结果进行排序。  排序最高并不一定是最合适的，又引入了组合优化的方法，计算组合分数和规模一致性。组合优化需要考虑支持的关系和大致放置的位置。  
 Co-placement 通过改善初始放置，在草图约束的情况下。  
 大致看完一遍了，写的太复杂了，后面再看一下。
 




