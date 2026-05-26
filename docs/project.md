项目经验 / Project Experience
项目名称：基于 LangChain 的智能旅行规划 Agent 系统
技术栈： Python, LangChain, LangGraph, FastAPI, Vue3, MongoDB, Redis

核心 Agent 架构与状态管理： 采用 LangChain 框架构建底层智能体逻辑，并引入 LangGraph 管理多轮对话中的复杂状态（State Graph）。实现上下文记忆提取、意图路由与节点流转，支持用户随时通过自然语言中断、微调或重写当前旅行计划。

自定义工具（Tools）集成： 将高德地图 API（POI 搜索、天气查询、多交通路线规划）封装为 LangChain 自定义工具链。利用 ReAct 范式驱动 Agent 按需调用外部服务，有效消除大模型幻觉，确保行程方案的真实落地性。

全栈工程化与持久化： 使用 FastAPI 搭建高并发接口层；基于 Redis 和 MongoDB 实现 BaseChatMessageHistory 的持久化，管理高并发会话状态与行程快照；前端采用 Vue3 + TS 构建交互界面，并编写 Docker 脚本完成全栈容器化自动化部署。

项目名称：基于 SegFormer 的道路裂缝图像语义分割系统
技术栈： PyTorch, SegFormer, Mix Transformer (MiT), 计算机视觉

模型架构优化： 引入轻量级 SegFormer 架构解决传统 CNN 感受野受限问题。使用 Mix Transformer (MiT) 替代卷积骨干网络，利用 Overlapping Patch 机制（无需位置编码）提取多尺度特征，提升复杂背景下的长程依赖建模能力。

解码器重构与样本均衡： 弃用计算密集型卷积解码器，采用纯 MLP（多层感知机）融合多尺度特征，大幅降低计算复杂度；针对裂缝与背景像素极度不平衡问题，采用 Dice Loss 与交叉熵（CE Loss）联合优化模型参数。

量化成果： 独立完成近 4000 张图像的数据清洗与端到端训练闭环。模型迭代 16 万步后平稳收敛，测试集平均交并比（mIoU）达 80%，准确率近 100%，成功实现高精度、细粒度的裂缝像素级分割。

项目三
主导设计并实现了一套OCT影像分析系统，以课题组内多个成熟的深度学习模型为基础，成功将支架检测与三维重建、关键帧提取与渲染、斑块分割、病例检索、血栓识别、以及坐标转换等关键功能整合进一个统一的智能分析平台。

技术栈：LangChain + RAG + Electron +MCP
基于 LangGraph构建ReAct核心智能体，实现影像分析任务的自主规划与执行；使用 Faiss + Bm25构建病例检索引擎；通过Function Call / MCP集成深度学习模型，可实现分布式模型调用；使用 Electron 构建用户友好的统一UI 界面。
