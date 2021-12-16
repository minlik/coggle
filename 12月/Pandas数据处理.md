## Pandas数据处理

https://shimo.im/docs/dqiwqt0T7fwl8Day/read

## 打卡汇总

| 任务名称                              | 难度  | 所需技能                |
| ------------------------------------- | ----- | ----------------------- |
| 任务1：Pandas数据读取、保存和数据类型 | 低、1 | DataFrame               |
| 任务2：Pandas数据位置索引             | 低、1 | loc、iloc               |
| 任务3：Pandas数据逻辑索引             | 中、2 | loc、where              |
| 任务4：Pandas数据分组聚合             | 高、3 | groupby、agg、transform |
| 任务5：Pandas日期数据处理             | 中、2 | dt                      |
| 任务6：Pandas缺失值处理               | 中、2 | fillna                  |
| 任务7：Pandas数据可视化               | 中    | plot                    |
| 任务8：Pandas多表合并和聚合           | 中    | merge                   |
| 任务9：Pandas透视表和交叉表操作       | 高    |                         |
| 任务10：Pandas性能优化                | 高    | Numpy、joblib           |

## 学习资料

[https://github.com/datawhalechina/joyful-pandas](https://github.com/datawhalechina/joyful-pandas?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://blog.csdn.net/u010161379/article/details/79187614](https://blog.csdn.net/u010161379/article/details/79187614?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

**任务1：Pandas数据读取、保存和数据类型**

任务要点：文件读取、保存、数据类型分析

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：将读取的进行保存，表头也需要保存

- 步骤3：分析每列的类型，取值个数

- 步骤4：分析每列是否包含缺失值

**任务2：Pandas数据位置索引**

任务要点：数据选择、数据索引

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：选择出Total列

- 步骤3：选择出Total列和HP列

- 步骤4：选择出第10-40行数据

- 步骤5：选择出第10-40行的Total列和HP列



**任务3：Pandas数据逻辑索引**

任务要点：逻辑索引

[https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.where.html](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.where.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/indexing.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：筛选出Type 1 为 Grass的数据

- 步骤3：筛选出Type 1 为 Grass的数据 且 Type 2 为 Poison的数据

- 步骤4：筛选出HP大于50 或 Speed小于90的数据

- 步骤5：筛选出Type 1 取值为Grass 或 Fire，且 HP 位于 70 与 90之间，且 Speed以数字8开头的数据

**任务4：Pandas数据分组聚合**

[https://pandas.pydata.org/pandas-docs/stable/user_guide/groupby.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/groupby.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

任务要点：groupby、agg、transform

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：学习groupby分组聚合的使用

- 步骤3：学习agg分组聚合的使用

- 步骤4：学习transform的使用

- 步骤5：使用groupby、agg、transform，统计数据在Type 1分组下 HP的均值



**任务5：Pandas日期数据处理**

[https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/timeseries.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://pandas.pydata.org/pandas-docs/stable/user_guide/timedeltas.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/timedeltas.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

任务要点：日期处理

- 步骤1：创建一列dt，dt取值为从1638263656 到 1638283656 的 unix时间

- 步骤2：将dt列转为datatime格式

- 步骤3：筛选出dt列中小时为10的行

- 步骤4：将dt列整体增加8小时的时间



**任务6：Pandas缺失值处理**

[https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/missing_data.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：分析每列的缺失值

- 步骤3：对每列的缺失值进行填空



**任务7：Pandas数据可视化**

[https://www.cnblogs.com/zhangyafei/p/10518826.html](https://www.cnblogs.com/zhangyafei/p/10518826.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/visualization.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

任务要点：plot

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：统计Type 1分组下HP、Attack、Defense的均值，并进行绘制柱状图

- 步骤3：将所有样本的HP、Attack绘制散点图



**任务8：Pandas多表合并和聚合**

[https://blog.csdn.net/jasonzhoujx/article/details/81665558](https://blog.csdn.net/jasonzhoujx/article/details/81665558?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/merging.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://queirozf.com/entries/pandas-dataframes-merge-join-examples](https://queirozf.com/entries/pandas-dataframes-merge-join-examples?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

![merge](/home/kuan/Desktop/coggle/12月/merge.png)

任务要点：merge、join

- 步骤1：创建如下数据

```python
data1 = pd.DataFrame({"ID":range(101, 106),          
                      "x1":range(1, 6),
                      "x2":["a", "b", "c", "d", "e"],
                      "x3":range(16, 11, - 1)})

data2 = pd.DataFrame({"ID":range(104, 108),        
                      "y1":["x", "y", "x", "y"],
                      "y2":range(8, 1, - 2)})

data3 = pd.DataFrame({"ID":range(102, 110),     
                      "z1":range(10, 18),
                      "z2":["z", "b", "z", "z", "d", "z", "d", "a"],
                      "z3":range(18, 10, - 1)})
```

- 步骤2：Merge data1 and data2 Using Inner Join

- 步骤3：Merge data1 and data2 Using Outer Join

- 步骤4：Merge data1 and data2 Using Left Join

- 步骤5：Merge data1 and data2 Using Right Join

- 步骤6：Merge data1 ,data2 and data3 Using Outer Join

- 步骤7：Merge data1 and data2 based on Index



**任务9：Pandas透视表和交叉表操作**

[https://pandas.pydata.org/pandas-docs/stable/user_guide/reshaping.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/reshaping.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

![pivot](/home/kuan/Desktop/coggle/12月/pivot.png)

- 步骤1：读取文件[https://cdn.coggle.club/Pokemon.csv](https://cdn.coggle.club/Pokemon.csv?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤2：统计Type 1和Type 2分组下HP,Attack,Defense的均值

- 步骤3：统计Type 1为index，Type 2取值为不同列的情况下，Attack的均值



**任务10：Pandas性能优化**

[https://pandas.pydata.org/pandas-docs/stable/user_guide/enhancingperf.html](https://pandas.pydata.org/pandas-docs/stable/user_guide/enhancingperf.html?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

[https://realpython.com/fast-flexible-pandas/](https://realpython.com/fast-flexible-pandas/?accessToken=eyJhbGciOiJIUzI1NiIsImtpZCI6ImRlZmF1bHQiLCJ0eXAiOiJKV1QifQ.eyJhdWQiOiJhY2Nlc3NfcmVzb3VyY2UiLCJleHAiOjE2Mzk2MjczODIsImciOiJkcWl3cXQwVDdmd2w4RGF5IiwiaWF0IjoxNjM5NjI3MDgyLCJ1c2VySWQiOjM5MzI4OTU2fQ.iTOAuQqWr7pBIFiEHj2-8-avQ8zN0IegnF9yQg3EYkA)

- 步骤1：创建如下数据

```python
data = pd.DataFrame({
    "x1":list(range(1000, 2000))*1000,          
    "x2":list(range(1000))*1000
})
```

- 步骤2：使用iloc遍历数据集，并记录下时间。

- 步骤3：使用`itertuples`和`iterrows` 遍历数据集，并记录下时间。

- 步骤4：使用cython和ndarray完成数据遍历，并统计统计下x1分组下x2的均值。

