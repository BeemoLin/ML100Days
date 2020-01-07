# 3rd-ML100Days

![img](https://raw.githubusercontent.com/BeemoLin/ML100Days/master/E9813924.jpg)

# Day009
Day 009 用到的 ecdf

Python经验分布函数(ecdf)实现

寫成Function
```
def ecdf(data):
    sq = data.value_counts()
    return sq.sort_index().cumsum()*1/len(sq)
```
如果data 已經排序則不需要跑sq.sort_index()
```
def ecdf(data):
    sq = data.value_counts()
    return sq.cumsum()*1/len(sq)
```

https://codeday.me/bug/20190309/727401.html
