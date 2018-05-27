# 数据分析学习
|学校|专业|姓名|邮箱|
|:-------:|:-------------: | :----------:|:-------------: |
|成都大学|软件工程(本)15-2|钟宇航|18990051970@163.com|

## 利用Python进行NBA比赛数据分析
---
>## 函数解释：
>* initialize_data
>	>根据每支队伍的Miscellaneous Opponent，Team统计数据csv文件进行初始化

>* get_elo
>	>获取每支队伍的Elo Score等级分，当在开始没有等级分时，将其赋予初始base_elo值

>* calc_elo
>	>计算每个球队的elo值

>* build_dataSet
>	>基于我们初始好的统计数据，及每支队伍的Elo score计算结果，建立对应2015~2016年常规赛和季后赛中每场比赛的数据集（在主客场比赛时，我们认为主场作战的队伍更加有优势一点，因此会给主场作战队伍相应加上100等级分）

>* main
>	>在main函数中调用以上处理函数，使用sklearn的Logistic Regression方法建立回归模型

>* predict_winner
>	>最终利用训练好的模型在16~17年的常规赛数据中进行预测。利用模型对一场新的比赛进行胜负判断，并返回其胜利的概率

### [源码](https://github.com/zhongyuhang/data-analysis/blob/master/nba-prediction/prediction.py)
### [分析结果](https://github.com/zhongyuhang/data-analysis/blob/master/nba-prediction/16-17Result.csv)


