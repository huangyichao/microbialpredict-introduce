# Microbial Predict 在线预测微生物建模工具

## 使用教程

### 1 加载网页

```
cd code # 切换到网页代码文件夹
nohup Rscript runShiny.R > ~/nohup.out 2>&1 & # 后台运行
```

打开网页：http://127.0.0.1:6468/

### 2 功能使用

#### 估计参数

1. 一级模型

   生长

   1. 完整模型：使用数据growthcurve1.csv验证
   2. 无延滞期模型：使用数据growthcurve3.csv验证
   3. 无最大浓度模型：使用数据growthcurve2.csv验证

   失活

   1. 完整模型：使用数据survivalcurve1.csv验证
   2. 无延滞模型：使用数据survivalcurve3.csv验证
   3. 无拖尾模型：使用数据survivalcurve2.csv验证

2. 二级模型

   温度模型：使用数据cmp_T.csv验证

   pH模型：使用数据cmp_pH.csv验证

   水分活度模型：使用数据cmp_aw.csv验证

3. 竞争模型

   ①  时间，1类数量，2类数量：使用数据competition1-2.csv验证

   ②  时间，类别，数量：使用数据competition1.csv验证

4. 变温模型：不支持

#### 预测模拟

1. 恒态条件

   生长

   失活

2. 变温条件：不支持

