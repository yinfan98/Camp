### 姓名

谢一帆

### 实习项目

飞桨 PaddlePaddle-PIR 适配 VisualDL 模型可视化

### 本周工作

1. **完成 visualdl 可视化控制流算子的功能开发**

- 针对 ifop 和 whileop 算子开发特定的解析方法，在前端表现为 layer
- 完善对控制流算子传入变量和传出变量的可视化处理，控制流算子内部所有算子接收外部传入的变量均传入控制流算子，控制流算子传出的变量在内部构建一个抽象 output 算子接收 yield 算子的输出，并将 output 作为展开控制流算子后代表控制流算子的输出
- 提升控制流算子 layer 的可视化美观程度

2. **初步实现 json 格式存储的 paddle 模型的计算图可视化**

- 利用 save load 实现提取 json 格式模型的计算图
- 对接接口，初步实现 json 格式模型的计算图的可视化，目前只能全部展开

3. **修复已知 Bug**

### 下周工作

1. **完善 visualdl 对控制流算子的可视化**

- 修改 visualdl 后端，提供每个算子的具体类型以优化前端可视化效果
- 修改 visualdl 后端，对于展开后的计算图中没有参数传入或传出的算子进行隐藏处理

2. **设计从 json 格式模型中获取算子所属 layer 的方法**

### 导师点评

已按计划和要求完成工作。
