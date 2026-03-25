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
Here are your **PostgreSQL (Postgres) SQL commands** for your practical questions (simple and correct for exam) 👇

---

# ✅ **Q1: Property & Owner Tables**

### 🔹 Create Tables

```sql
CREATE TABLE Owner (
    owner_name VARCHAR(50) PRIMARY KEY,
    address VARCHAR(50),
    phoneno BIGINT,
    income INTEGER
);

CREATE TABLE Property (
    pnumber INTEGER PRIMARY KEY,
    description VARCHAR(50) NOT NULL,
    area CHAR(10),
    owner_name VARCHAR(50),
    FOREIGN KEY (owner_name) REFERENCES Owner(owner_name)
);
```

---

### 🔹 Queries

1. **List properties in specific area**

```sql
SELECT * FROM Property WHERE area = 'Pune';
```

2. **Owners whose name starts with 'A'**

```sql
SELECT * FROM Owner WHERE owner_name LIKE 'A%';
```

3. **Count of properties in area**

```sql
SELECT COUNT(*) FROM Property WHERE area = 'Pune';
```

4. **Count of owners in each area**

```sql
SELECT area, COUNT(*) 
FROM Property 
GROUP BY area;
```

5. **Owners with average income**

```sql
SELECT AVG(income) FROM Owner;
```

---

# ✅ **Q2: Student & Exams Tables**

### 🔹 Create Tables

```sql
CREATE TABLE Student (
    stud_id INTEGER PRIMARY KEY,
    name VARCHAR(50) NOT NULL,
    class CHAR(10)
);

CREATE TABLE Exams (
    exam_id INTEGER PRIMARY KEY,
    s_no INTEGER,
    sub VARCHAR(10),
    score INTEGER,
    exam_date DATE,
    FOREIGN KEY (s_no) REFERENCES Student(stud_id)
);
```

---

### 🔹 Queries

1. **All students and exams**

```sql
SELECT * FROM Student
JOIN Exams ON Student.stud_id = Exams.s_no;
```

2. **Students of specific branch**

```sql
SELECT * FROM Student WHERE class = 'CS';
```

3. **Math scores ascending**

```sql
SELECT * FROM Exams 
WHERE sub = 'Math'
ORDER BY score ASC;
```

4. **Total score of student**

```sql
SELECT SUM(score) 
FROM Exams 
WHERE s_no = 1;
```

5. **Average Computer score**

```sql
SELECT AVG(score) 
FROM Exams 
WHERE sub = 'Computer';
```

6. **Count exams per student**

```sql
SELECT s_no, COUNT(*) 
FROM Exams 
GROUP BY s_no;
```

7. **Student name with score**

```sql
SELECT name, score 
FROM Student 
JOIN Exams ON Student.stud_id = Exams.s_no;
```

---

# ✅ **Q3: Book & Member Tables**

### 🔹 Create Tables

```sql
CREATE TABLE Member (
    m_name VARCHAR(50) PRIMARY KEY,
    address VARCHAR(50),
    phoneno BIGINT,
    age INTEGER
);

CREATE TABLE Book (
    b_id INTEGER PRIMARY KEY,
    title VARCHAR(50) NOT NULL,
    category CHAR(20),
    m_name VARCHAR(50),
    FOREIGN KEY (m_name) REFERENCES Member(m_name)
);
```

---

### 🔹 Queries

1. **Books in category**

```sql
SELECT * FROM Book WHERE category = 'Fiction';
```

2. **Members starting with 'A'**

```sql
SELECT * FROM Member WHERE m_name LIKE 'A%';
```

3. **Total books in category**

```sql
SELECT COUNT(*) FROM Book WHERE category = 'Fiction';
```

4. **Count books per category**

```sql
SELECT category, COUNT(*) 
FROM Book 
GROUP BY category;
```

5. **Average age of members**

```sql
SELECT AVG(age) FROM Member;
```

---

# ✅ **Important Notes (for exam)**

* Use `LIKE 'A%'` → starts with A
* Use `COUNT()` → number of records
* Use `AVG()` → average
* Use `SUM()` → total
* Use `JOIN` → combine tables

---

# 🎯 If you want:

I can also give
✅ **Insert values (sample data)**
✅ **Output tables**
✅ **Viva questions + answers**

Just tell me 👍

