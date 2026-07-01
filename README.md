# 数据分析项目 (Data Analysis Project)

## 项目简介

本项目主要是一个基于 RFM 模型的数据分析项目，主要进行客户价值分析。RFM 分析是一种常用的客户细分方法，通过三个维度对客户进行评估：

- **R (Recency)**: 最近一次消费时间
- **F (Frequency)**: 消费频率
- **M (Monetary)**: 消费金额

## 项目文件介绍

### 1. RFM_deepseek.ipynb
Jupyter Notebook 文件，包含 RFM 分析的核心代码和实现逻辑。render.html是对应的RFM模型3D数据渲染，便于直观理解！渲染图如下：
<img width="656" height="389" alt="RFM模型3D渲染" src="https://github.com/user-attachments/assets/388843dd-c3d3-4ee8-ac61-6815f1288374" />


### 2. 基于RFM模型的咖啡品牌用户分层与消费特征分析.ipynb 
该文件是 **主要分析的主体** ，对差不多10万条某电商销售数据进行分析，分析的板块有以下：
- 数据清洗与预处理
- 用户个体消费
- 用户整体消费
- 用户分层
- 用户购买周期
- 用户生命周期
- 用户复购率
- 用户回购率

### 3. PowerBI看板搭建项目
基于三年 10 万+条历史订单销售数据，搭建 PowerBI 可视化动态钻取数据看板，实现销售数据多维度展示分析
看板主体内容：
- 设计 4 个切片器（年份/产品/城市/销售渠道），支持全局数据筛选，并配置筛选器清除工具优化用户体验。
- 构建销售收入、毛利、毛利率、销售数量 4 个核心指标卡片，通过 DAX 公式实现自动计算。
- 制作销售渠道、城市、产品收入占比环形图以及销售收入趋势折线图，直观展示数据分布与业务增长变化。
- 开发同比分析柱状图，运用时间智能函数（SAMEPERIODLASTYEAR）对比本期与去年同期数据，差异化颜色标记业绩优劣。

搭建流程：
<img width="302" height="267" alt="搭建流程" src="https://github.com/user-attachments/assets/e6b66cbe-9a16-40bb-9ab9-74b537fd9fd4" />


看板效果图如下：
<img width="754" height="425" alt="成果展示" src="https://github.com/user-attachments/assets/800a8e97-cbba-41ef-b8d9-212ce47fbbd3" />




## 技术栈

- Python
- Jupyter Notebook
- 数据分析库 (Pandas, NumPy 等)
- 数据可视化工具

## 使用方法

1. 确保已安装 Python 3.x 和 Jupyter Notebook
2. 安装所需依赖包：
   ```bash
   pip install pandas numpy matplotlib
   ```
3. 打开 `RFM_deepseek.ipynb` 文件，运行分析代码
4. 在浏览器中打开 `render.html` 查看可视化结果

## 分析流程

1. 数据加载与预处理
2. 计算 RFM 指标
3. 客户分层与评分
4. 结果可视化
5. 业务洞察与建议
