# 24fall编程基础期末大作业数据文件及代码说明
本项目包含共计6个文件。
1. 代码文件
   * "胡瑞扬 2024104079 编程基础期末代码.ipynb" 本项目报告的代码实现。
   * 运行环境：Python(3.9.12) IDE:VSCode
   * 使用的包及版本：numpy(1.26.4) pandas(2.2.3) seaborn(0.13.2) matplotlib(3.9.2) scikit-learn(1.5.2) xgboost(2.1.3)
2. 数据文件
   源数据来自https://archive.ics.uci.edu/dataset/186/wine+quality，为葡萄牙Vinho Verde红葡萄酒质量数据，包含11项物理化学指标及1项质量评分。本项目仅使用了原始数据集中的winequality-red.csv文件，数据处理及版本如下：
   * "winequality-red-original.csv" 原始数据文件，包含葡萄酒质量数据共计1599条，仅重命名文件名，未进行任何数据处理操作；
   * "winequality-new.csv" 用于实际检验项目模型预测效果的小数据集，包含葡萄酒质量数据共计30条，从original文件中随机抽取得；
   * "winequality-red.csv" 用于项目模型训练的数据集，包含葡萄酒质量数据共计1569条，为original文件中去掉new中条目的剩余部分；
   * "winequality-predictions.csv" 项目模型对new文件预测后的数据集，除11项物理化学指标及原有质量评分（列名重命名为actual_scores）外，另有两列svm_Prediction和rf_Prediction，表示两个模型分别给出的预测评分。
4. 日志文件
   * "wine_predictor_20241221_150023.log" 记录模型训练过程及模型表现评估的训练日志文件。
