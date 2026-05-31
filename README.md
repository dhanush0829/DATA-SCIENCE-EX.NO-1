#EX.NO:1
Data Cleaning Process

# AIM
To read the given data and perform data cleaning and save the cleaned data to a file.

# Explanation
Data cleaning is the process of preparing data for analysis by removing or modifying data that is incorrect ,incompleted , irrelevant , duplicated or improperly formatted. Data cleaning is not simply about erasing data ,but rather finding a way to maximize datasets accuracy without necessarily deleting the information.

# Algorithm
STEP 1: Read the given Data

STEP 2: Get the information about the data

STEP 3: Remove the null values from the data

STEP 4: Save the Clean data to the file

STEP 5: Remove outliers using IQR

STEP 6: Use zscore of to remove outliers

# Coding and Output
```
     import pandas as pd
        df=pd.read_csv('D:Data_set (1).csv') print(df)

       print(data)
```
<img width="728" height="696" alt="image" src="https://github.com/user-attachments/assets/e7002102-ef52-446d-83ad-103a5ca64c10" />
<img width="810" height="374" alt="image" src="https://github.com/user-attachments/assets/23ece2e9-2698-4c07-82aa-59ab8f577010" />

df=pd.DataFrame(data)
print(df.isnull())

<img width="803" height="664" alt="image" src="https://github.com/user-attachments/assets/c1eed309-3262-4689-832c-93f03621bdec" />
<img width="385" height="283" alt="image" src="https://github.com/user-attachments/assets/bf81c194-0bc9-47ec-8a26-d7bef234640b" />

```
import pandas as pd
df = pd.DataFrame(data)
data=pd.read_csv('D:Data_set (1).csv')
df=pd.DataFrame(data)
dfd=df.dropna()
print("AFTER DROPNA")
```

<img width="825" height="717" alt="image" src="https://github.com/user-attachments/assets/e63ab8f2-eae2-46a2-9ead-51558ce9144e" />

dfd=df.dropna(axis=1)
print("AFTER DROPNA")

<img width="656" height="402" alt="image" src="https://github.com/user-attachments/assets/39ce70f2-2c36-437e-b072-ee3e9f2a5f7d" />
<img width="635" height="59" alt="image" src="https://github.com/user-attachments/assets/3cfac7bd-298d-4369-91c0-0a1d26493514" />

```
dfd = df.dropna(axis=1,inplace=True)
print("AFTER DROPNA") dfd=df.dropna(axis=0)
print("AFTER DROPNA")
print(dfd)
```

<img width="806" height="397" alt="image" src="https://github.com/user-attachments/assets/2aa659db-439b-4d4e-9848-6b54ba78bd04" />
<img width="426" height="264" alt="image" src="https://github.com/user-attachments/assets/2cd7413a-7be0-43f8-9394-f923bfdecc2d" />

dfd = df.fillna(method = "ffill")
df = pd.DataFrame
print("AFTER FILLNA")

<img width="808" height="707" alt="image" src="https://github.com/user-attachments/assets/e1f3e463-b2b8-4723-a9b3-fe6adb75c9b2" />

```
dfd=df.fillna({'show_name':'nandy','aired_on':'wednesday','original_network':'Jio','rating':7.5})
print("AFTER FILLNA")
print(dfd) import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
data=pd.read_csv("iris.csv")
df=pd.DataFrame(data)
print(df)
x=df["petal_length"]
y=df["sepal_length"]
plt.bar(x,y)
plt.show()
```

<img width="604" height="681" alt="image" src="https://github.com/user-attachments/assets/0d4c001a-4067-4ae4-813d-d978e1bad39f" />

```
import matplotlib.pyplot as plt
import numpy as np
data=pd.read_csv("iris.csv")
df=pd.DataFrame(data)
print(df)
x=df["petal_length"]
y=df["sepal_length"]
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.plot(x,y)
```

<img width="665" height="752" alt="image" src="https://github.com/user-attachments/assets/f1a59cc2-6eab-488a-aa36-0acb70954c46" />

```
import pandas as pd
import matplotlib.pyplot as plt
import numpy as np
data=pd.read_csv("iris.csv")
df=pd.DataFrame(data)
print(df)
dff=plt.boxplot(x="petal_width",data=df)
print(dff)
```

<img width="1043" height="698" alt="image" src="https://github.com/user-attachments/assets/b16897d1-78c5-45bb-8d00-df7c58108023" />

# Result
          <<include your Result here>>
