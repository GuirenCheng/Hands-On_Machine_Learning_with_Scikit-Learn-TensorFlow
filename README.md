# Hands-On Machine Learning Study Notes

本项目是我学习《机器学习实战：基于 Scikit-Learn、Keras 和 TensorFlow》的学习记录与实战代码。

## 📂 项目结构说明
- `Chapter02_Housing/`: 第 2 章 - 端到端房价预测项目（回归）
- `Chapter03_Classification/`: 第 3 章 - MNIST 数字识别项目（分类）
- `Chapter04_Training_Model/`: 第 4 章 - 模型训练原理（深入线性回归与梯度下降）
- `Chapter05_SVM/`: 第 5 章 - 支持向量机 (SVM) 的理论与实践，涵盖线性与非线性分类、回归及核技巧。
- `Chapter06_Decision_Trees/`: 第 6 章 - 决策树 (Decision Trees)
- `chapter07_Ensemble_Learning_and_Random_Forest/`: 第 7 章 - 集成学习（Bagging, Boosting, Stacking）与随机森林
- `Chapter08_Dimension_Reduction/`: 第 8 章 - 降维技术（PCA, IPCA, kPCA, LLE）
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
## 🛠️ 技术栈
- Python 3.10+
- Scikit-Learn
- NumPy / Pandas / Matplotlib