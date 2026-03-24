Got it 👍 Here are **ALL 19 programs**, each written **separately with proper imports in each program** and **clean code**:

---

## ✅ **Program 1**

```python
import pandas as pd

data = {
    "Name": ["Amit","Rahul","Sneha","Priya","Rohan","Neha","Kiran","Pooja","Vikas","Anjali"],
    "Age": [20,21,19,22,20,21,23,19,22,20],
    "Percentage": [85,78,92,88,76,81,79,95,84,90]
}

df = pd.DataFrame(data)
print(df)
```

---

## ✅ **Program 2**

```python
import pandas as pd

data = {
    "Name": ["Amit","Rahul","Sneha","Priya","Rohan","Neha","Kiran","Pooja","Vikas","Anjali"],
    "Age": [20,21,19,22,20,21,23,19,22,20],
    "Percentage": [85,78,92,88,76,81,79,95,84,90]
}

df = pd.DataFrame(data)

new_rows = pd.DataFrame({
    "Name": ["Amit","Rahul",None,"Priya","Rohan"],
    "Age": [20,None,19,22,None],
    "Percentage": [85,78,None,88,76]
})

df = pd.concat([df,new_rows],ignore_index=True)
df["remarks"] = ""

print(df)
```

---

## ✅ **Program 3**

```python
import matplotlib.pyplot as plt

height = [150,160,165,170,175,180]
weight = [50,60,65,70,75,80]

plt.scatter(height,weight)
plt.xlabel("Height")
plt.ylabel("Weight")
plt.show()
```

---

## ✅ **Program 4**

```python
import pandas as pd
from scipy.stats import gmean, hmean

data = {
    "Math":[80,85,90,75,88,92,70,95,89,84],
    "Science":[78,82,88,74,86,91,72,94,87,83],
    "English":[85,80,90,78,88,93,76,96,89,84],
    "History":[70,75,80,65,78,82,68,85,79,74],
    "Computer":[88,90,92,85,91,95,87,97,93,89]
}

df = pd.DataFrame(data)

print(df.mean())
print(gmean(df))
print(hmean(df))
```

---

## ✅ **Program 5**

```python
import pandas as pd

df = pd.read_csv("data.csv")
print(df)
```

---

## ✅ **Program 6**

```python
import numpy as np
import matplotlib.pyplot as plt

arr = np.random.randint(1,100,50)

plt.plot(arr)
plt.show()

plt.scatter(range(50),arr)
plt.show()

plt.hist(arr)
plt.show()

plt.boxplot(arr)
plt.show()
```

---

## ✅ **Program 7**

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn.datasets import load_iris

iris = load_iris()
target = iris.target

unique, counts = np.unique(target, return_counts=True)

plt.bar(unique, counts)
plt.show()
```

---

## ✅ **Program 8**

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn.datasets import load_iris

iris = load_iris()
target = iris.target

unique, counts = np.unique(target, return_counts=True)

plt.pie(counts, labels=unique)
plt.show()
```

---

## ✅ **Program 9**

```python
import matplotlib.pyplot as plt

subjects = ["Math","Science","English","History","Computer"]
marks = [80,85,90,75,88]

plt.bar(subjects,marks)
plt.show()

plt.pie(marks,labels=subjects)
plt.show()
```

---

## ✅ **Program 10**

```python
import matplotlib.pyplot as plt
from sklearn.datasets import load_iris

iris = load_iris()
x = iris.data[:,0]
y = iris.data[:,1]

plt.scatter(x,y)
plt.show()
```

---

## ✅ **Program 11**

```python
import matplotlib.pyplot as plt
from sklearn.datasets import load_iris

iris = load_iris()
data = iris.data

plt.boxplot(data)
plt.show()
```

---

## ✅ **Program 12**

```python
import pandas as pd

df = pd.DataFrame(columns=["Name","Age"])

df.loc[0] = ["Amit",20]
df.loc[1] = ["Rahul",21]

print(df)
```

---

## ✅ **Program 13**

```python
import pandas as pd
import numpy as np

arr = np.array([[1,2],[3,4]])
df1 = pd.DataFrame(arr)

lst = [[1,2],[3,4]]
df2 = pd.DataFrame(lst)

print(df1)
print(df2)
```

---

## ✅ **Program 14**

```python
import pandas as pd

data = [{"Name":"Amit","Age":20},{"Name":"Rahul","Age":21}]

df = pd.DataFrame(data)
print(df)
```

---

## ✅ **Program 15**

```python
import pandas as pd

df = pd.read_csv("data.csv")

print(df.shape)
print(df.isnull().sum())
print(df.head())
```

---

## ✅ **Program 16**

```python
import numpy as np
import matplotlib.pyplot as plt
from sklearn.datasets import load_iris

iris = load_iris()
target = iris.target

unique, counts = np.unique(target, return_counts=True)

plt.bar(unique, counts)
plt.show()
```

---

## ✅ **Program 17**

```python
import matplotlib.pyplot as plt

subjects = ["Math","Science","English"]
marks = [80,85,90]

plt.bar(subjects,marks)
plt.show()

plt.pie(marks,labels=subjects)
plt.show()
```

---

## ✅ **Program 18**

```python
import pandas as pd

df = pd.read_csv("data.csv")

print(df.describe())
print(df.shape)
print(df.head(3))
```

---

## ✅ **Program 19**

```python
import pandas as pd

df = pd.read_csv("data.csv")

df["salary"].fillna(df["salary"].mean(),inplace=True)
df["age"].fillna(df["age"].mean(),inplace=True)

print(df)
```

---

## 🎯 Done!

Now all programs are:
✔ Separate
✔ Clean
✔ Proper imports
✔ Ready for practical / exam

---

If you want next:
✅ PDF for submission
✅ Output screenshots
✅ Viva questions

Just tell 👍
