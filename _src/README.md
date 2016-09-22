## 代码说明

### 查看数据

查看文件类型

```
file filename
```

各列变量类型

```
csvstat ACMETelephoneABT.csv | egrep '(^  [^a-z])|(^ [^a-z])|(^\t<)'
```

查看列相对应的列号

```
csvcut -n filename
```

查看部分列的头部

```
csvcut -c 1,2 filename | head | csvlook
csvcut -c 1-5 filename | head | csvlook  # 1 至 5
```

获取存在 null 值的列

```
csvstat ACMETelephoneABT.csv --nulls | grep 'True$'
```

去除头部后统计行数

```
csvcut -c 3 ACMETelephoneABT.csv |  header -a count | wc -l
```

获取样本数据

```
shuf -n 500 file > newfile
```

### 数据清理

替换掉空格

```
cp ACMETelephoneABT.csv ACMETelephoneABT_backup.csv # 备份源数据
sed -i 's/ ,/,/g' ACMETelephoneABT.csv
sed -i 's/, /,/g' ACMETelephoneABT.csv
```

ACMETelephoneABT.csv这个文件的换行符是^M，导致很多 *nix 命令无法使用。

```
csvcut -c 1: ACMETelephoneABT.csv > ACMETelephoneABT_convertM.csv
```

