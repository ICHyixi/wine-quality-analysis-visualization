# 基于机器学习的葡萄酒质量预测项目

## 一、项目简介

本项目基于葡萄酒化学指标数据，对葡萄酒质量进行数据分析和预测建模。

通过对数据进行清洗、异常值处理、探索性数据分析以及机器学习建模，最终构建葡萄酒质量预测模型，并对模型效果进行评估。

该项目展示了一个完整的数据分析流程，包括：

* 数据清洗
* 异常值检测与处理
* 数据可视化分析
* 特征分析
* 机器学习模型训练
* 模型评估

该项目适用于数据分析与机器学习实践学习。

---

## 二、数据集介绍

数据集为红酒质量数据集，记录了葡萄酒的多种化学指标以及对应的质量评分。

数据文件：

```
winequality-red.csv
```

数据基本信息：

* 样本数量：1599 条
* 特征数量：11 个
* 目标变量：葡萄酒质量评分（quality）

主要特征包括：

* fixed acidity（固定酸度）
* volatile acidity（挥发性酸度）
* citric acid（柠檬酸）
* residual sugar（残留糖分）
* chlorides（氯化物）
* free sulfur dioxide（游离二氧化硫）
* total sulfur dioxide（总二氧化硫）
* density（密度）
* pH（酸碱度）
* sulphates（硫酸盐）
* alcohol（酒精含量）

预测目标：

```
quality
```

---

## 三、项目结构

项目主要文件结构如下：

```
wine-quality-ml-analysis
│
├─ winequality-red.csv                 原始数据
├─ wine_quality_cleaned.csv            清洗后的数据
├─ wine_quality_best_model.pkl         训练好的模型
├─ model_evaluation_results.csv        模型评估结果
├─ outlier_processing_report.txt       异常值处理报告
│
├─ 代码.ipynb                          数据分析与建模代码

```

---

## 四、数据处理过程

### 1 数据清洗

对数据集进行了基本的数据清洗，包括：

* 检查缺失值
* 检查数据类型
* 统一数据格式

---

### 2 异常值处理

使用 **IQR（四分位距）方法** 对异常值进行检测。

处理流程：

1. 计算第一四分位数 Q1
2. 计算第三四分位数 Q3
3. 计算 IQR = Q3 − Q1
4. 根据上下界识别异常值
5. 对异常值进行处理

处理结果记录在：

```
outlier_processing_report.txt
```

---

## 五、探索性数据分析

对数据进行了多种统计分析和可视化分析，包括：

* 各特征分布情况
* 特征之间的相关性分析
* 不同特征对葡萄酒质量的影响
* 数据统计描述

主要使用的可视化工具：

* Matplotlib
* Seaborn

---

## 六、机器学习建模

在数据预处理完成后，对数据进行机器学习建模。

主要步骤：

1. 数据集划分（训练集 / 测试集）
2. 模型训练
3. 模型评估
4. 模型选择

最终模型保存为：

```
wine_quality_best_model.pkl
```

模型评估结果保存为：

```
model_evaluation_results.csv
```

---

## 七、使用技术

本项目主要使用以下技术：

* Python
* Pandas
* NumPy
* Matplotlib
* Seaborn
* Scikit-learn
* Jupyter Notebook

---

## 八、运行方法

### 1 克隆项目

```
git clone https://github.com/ICHyixi/wine-quality-ml-analysis.git
```

---

### 2 安装依赖

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

---

### 3 运行代码

启动 Jupyter Notebook：

```
jupyter notebook
```

打开文件：

```
代码.ipynb
```

即可运行项目代码。

---

## 九、项目意义

通过本项目，可以学习并实践完整的数据分析流程，包括：

* 数据清洗
* 异常值处理
* 数据可视化分析
* 机器学习建模
* 模型评估

适合数据分析和机器学习入门实践。

---

## 作者

个人学习项目，用于数据分析与机器学习实践。

