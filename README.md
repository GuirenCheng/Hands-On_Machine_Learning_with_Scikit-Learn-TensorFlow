# Hands-On Machine Learning Study Notes

本项目是我学习《机器学习实战：基于 Scikit-Learn和 TensorFlow》的学习记录与实战代码。
![TensorFlow 2.x](https://img.shields.io/badge/TensorFlow-2.x-orange?logo=tensorflow)
![Keras](https://img.shields.io/badge/Keras-Modern_API-red?logo=keras)
![Edition](https://img.shields.io/badge/Edition-3rd_Version-blue)
本项目已全面升级至 《机器学习实战》第二版 (2nd Edition)。

机器学习部分：基于最新的 Scikit-Learn 实践。

深度学习部分：废弃旧版 TF 1.x 静态图模型，全量采用 TensorFlow 2.x & Keras 动态流进行重构。

## 📂 项目结构说明
- `Chapter02_Housing/`: 第 2 章 - 端到端房价预测项目（回归）
- `Chapter03_Classification/`: 第 3 章 - MNIST 数字识别项目（分类）
- `Chapter04_Training_Model/`: 第 4 章 - 模型训练原理（深入线性回归与梯度下降）
- `Chapter05_SVM/`: 第 5 章 - 支持向量机 (SVM) 的理论与实践，涵盖线性与非线性分类、回归及核技巧。
- `Chapter06_Decision_Trees/`: 第 6 章 - 决策树 (Decision Trees)
- `chapter07_Ensemble_Learning_and_Random_Forest/`: 第 7 章 - 集成学习（Bagging, Boosting, Stacking）与随机森林
- `Chapter08_Dimension_Reduction/`: 第 8 章 - 降维技术（PCA, IPCA, kPCA, LLE）
- `Chapter10_Introduction_of_Keras_Artificial_Neural_Network/`: 第 10 章 - Keras 与人工神经网络入门。涵盖感知器、多层感知器（MLP）、使用 Sequential API 和 Functional API 构建模型、模型保存与恢复及超参数调优。
- `Chapter11_Training_Deep_Neural_Networks/`: 第 11 章 - 训练深度神经网络。涵盖梯度消失/爆炸解决方案（He初始化、非饱和激活函数、BN）、迁移学习、高级优化器及正则化技术。
- `Chapter12_Customize_Models_And_Training_With_TensorFlow/`: 第 12 章 - 使用 TensorFlow 自定义模型和训练。深入底层 API，涵盖张量运算、自定义损失函数/指标/层/模型、自动微分（GradientTape）以及静态图（TF Function）性能优化。
- `requirements.txt`: 项目所需的 Python 依赖包清单

## 🚀 学习进度
- [✅] **第 2 章：端到端机器学习项目**
    - 获取数据、可视化探索、特征缩放与预处理。
- [✅] **第 3 章：分类任务**
    - 使用 SGD 分类器进行 MNIST 识别。
    - 混淆矩阵、精度/召回率权衡（PR 曲线与 ROC 曲线）。
    - 多标签分类与多输出分类（图片去噪实验）。
- [✅] **第 4 章：训练模型**
    - 实现各种梯度下降算法 (Batch / Stochastic / Mini-batch GD)。
    - 掌握多项式回归与过拟合处理。
    - 深入理解正则化技术：岭回归 (Ridge)、套索 (Lasso) 与弹性网络 (Elastic Net)。
    - 学习早期停止法 (Early Stopping) 与逻辑回归 (Logistic / Softmax)。
- [✅] **第 5 章：支持向量机**
    - 掌握线性 SVM 的硬间隔与软间隔分类。
    - 深入理解超参数 $C$ 和 $\gamma$ 对模型拟合（过拟合/欠拟合）的影响。
    - 实践多项式核与高斯 RBF 核处理非线性数据集。
    - 学习 SVM 回归（SVR）的 $\epsilon$-不敏感街道原理。
    - 理解 SVM 底层的二次规划 (QP)、对偶问题及核技巧数学背景。
- [✅] **第 6 章：决策树**
    - 学习使用 `DecisionTreeClassifier` 进行分类任务。
    - 掌握决策树的正则化参数（如 `min_samples_leaf`, `max_depth`）以防止过拟合。
    - 理解 CART 训练算法、基尼不纯度（Gini Impurity）与熵（Entropy）的原理。
    - 实践 `DecisionTreeRegressor` 处理回归问题。
    - 分析决策树的局限性（如对训练集旋转和微小变动的高度敏感性）。
- [✅] **第 7 章：集成学习与随机森林**
    - 实现投票分类器（Voting Classifiers）提升模型表现。
    - 掌握 Bagging 和 Pasting 采样技术及随机森林的特征重要性分析。
    - 深入对比 AdaBoost 与梯度提升（Gradient Boosting）的数学原理与迭代过程。
    - 实践早期停止法（Early Stopping）优化 GBRT 模型，防止过拟合。
    - 理解堆叠法（Stacking）的多层架构与元学习器原理。
- [✅] **第 8 章：降维**
    - 掌握 **PCA (主成分分析)** 的投影原理，学习如何保留最大方差以减少特征维度。
    - 实践 **PCA 压缩与还原**，在保留 95% 方差的同时显著减小 MNIST 数据集体积（约缩小 80%）。
    - 学习处理超大数据的 **增量 PCA (IPCA)** 及追求计算速度的 **随机 PCA**。
    - 深入理解 **核 PCA (kPCA)**，通过网格搜索优化超参数（如核函数类型与 $\gamma$ 值）处理非线性分布。
    - 掌握 **LLE (局部线性嵌入)** 算法，成功将“瑞士卷”等卷曲流形数据展开为低维平面。



- [✅] **第 10 章：使用 Keras 搭建人工神经网络**
    - **多 API 实践**：掌握了 `Sequential API` 的快速建模、`Functional API` 的灵活连接以及 `Subclassing API` 的高度自定义。
    - **架构创新**：实现了 **Wide & Deep** 模型，通过跨接（Skip Connection）结合了模型的记忆能力与泛化能力。
    - **多任务学习**：实践了带有辅助输出（Auxiliary Output）的架构，利用多个损失函数协同优化深度路径。
    - **避坑指南**： 
      - 解决了输入层维度不匹配（Flatten 层必要性）导致的 `ValueError`。 
      - 理解了 `batch_size` 增大对起始 Loss 记录点和梯度平滑度的影响。
    - **性能监控**：使用学习曲线（Loss/Accuracy Curve）诊断模型状态，识别并修复了模型不学习的“平行线”现象。

- [✅] **第 11 章：训练深度神经网络 (Training Deep Neural Networks)**
    - **攻克梯度问题**：掌握 **He 初始化** 与 **ELU/SELU** 激活函数，解决深层网络中的梯度消失与爆炸。
    - **加速训练**：实践 **批量归一化 (Batch Normalization)**，对比 **Adam、Nadam、RMSProp** 等先进优化器的收敛速度。
    - **迁移学习**：学习如何重用预训练层，利用**无监督预训练**和**辅助任务**处理小样本数据。
    - **正则化实战**：通过 **Dropout**、**MC Dropout** 和 **最大范数正则化** 显著提升模型的泛化能力。
    - **学习率策略**：实现 **1周期调度 (1cycle)** 和 **ReduceLROnPlateau**，让模型训练兼顾速度与精度。

- [✅] **第 12 章：使用 TensorFlow 自定义模型和训练 (Custom Models and Training)**
    - **张量与 NumPy 互操作**：掌握 `tf.Tensor` 的不可变性，及与 `tf.Variable`、`NumPy` 数组的无缝转换。
    - **自定义模型组件**：实现自定义 **损失函数 (Huber Loss)**、**评估指标**、**初始化器**及**正则化项**。
    - **高级层构建**：通过继承 `Layer` 类构建自定义层（处理多输入输出、状态管理），并实现 **自定义模型类 (Model Subclassing)**。
    - **自动微分机制**：实战 `tf.GradientTape` 手写训练循环，实现比 `model.fit()` 更精细的梯度控制。
    - **性能加速**：理解 **AutoGraph** 机制，利用 `@tf.function` 将 Python 函数即时编译为高效的计算图。

## 🛠️ 技术栈
- Python 3.10+
- **TensorFlow 2.x** (Eager Execution)
- **TensorBoard** (模型可视化)
- Scikit-Learn
- NumPy / Pandas / Matplotlib