# 数据文件夹说明

路径 `main\data`

原始数据在 `Node.csv`, `Link.csv` 应该放在该路径下。（这两个文件未被添加到 repo 中）

- `communities` 存放了对原始图进行社区检测的结果，一共891个 community
- `cache` 每个文件是：把单个团伙所有线索所在的 community 合并，得到的子图
  - 相比原数据，为每条边增加了 `weight`, 各个重要程度分别对应 `0.8 0.6 0.4 0.2`

- `subgraph` 每个文件是：以单个团伙所有线索为起点，在原始数据中搜索3跳内的节点，再经过一定的筛选得到的子图
  - 为每个节点计算了 `pagerank` 和 `betweenness`，值越高表示节点越重要





