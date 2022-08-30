# Statistics Class

## Necessary Imports

`import pandas as pd`
`import numpy as np`
`import seaborn as sns`
`import math`
`import collections`

## Make a data frames with pandas

```sh
data = { 'columnName':[data, from, column],
          'columnName':[data, from, column],
}

df = pd.DataFrame(data)
```

## Operations

| Name | Calculation | Pandas Format |
| ------ | ------ | ------ |
| Max Value | - | ```df.max()/df['ColumnName'].max()```|
| Min Value | - | ```df.min()/df['ColumnName'].min()```|
| Mean | - | ```df.mean()/df['ColumnName'].mean()```|
| Count Values | - | ```df.count()/df['ColumnName'].count()```|
| Counter Range | - | ```print(collections.Counter(df['column']))```|
| Resume from data | - | ```df.decribe```|
| Total Range | At = maxValue - minValue | ```totalRange = max - min```|
| Interval Class Range | k = √N(countOfData) | ```h = math.sqrt(len(df))```|
| Amplitude Class Range | h = At/k | ```h = totalRange/k```|

## Graphics with Seaborn

### Histogram
```sh
sns.histoplot(data=df, x='someData', stat='percert')
```
