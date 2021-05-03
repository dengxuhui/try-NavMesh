# try-NavMesh
本项目是从[NavMesh-Tutorial](https://github.com/Brackeys/NavMesh-Tutorial)克隆而来。
由于原本NavMesh教程中缺少部分代码，所以在这个项目中把缺失的代码补全。如果您也是初次尝试NavMesh，可以配合
youtube教程一同学习，学习链接：[NavMesh-Tutorial视频教程](https://www.youtube.com/watch?v=CHV1ymlw-P8&t=600s)

## Notes

### NavMeshSurface
新建一个空GameObject添加NavMeshSurface，点击Bake烘焙Walkable

一个NavMeshSurface对应一个代理类型。不同代理类型对应的Agent设置不一致，行动路径图会不一致。

#### AgentType
设置这个NavMeshSurface对什么Agent生效，不同Agent生成的路径图不一致，取决于Agent的身形跟行走能力。

#### CollectObjects
计算范围设置
- All:场景所有对象
- Volume：计算NavMeshSurface所在GameObject范围内
- Children：计算NavMeshSurface子节点所有范围

#### IncludeLayers
根据Layer Tag来计算
#### Use Geometry
依据Render来计算还是Collider来计算


### NavMeshAgent
让角色能在网格中导航的代理