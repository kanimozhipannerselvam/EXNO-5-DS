# EXNO-5-DS-DATA VISUALIZATION USING MATPLOT LIBRARY

# Aim:
  To Perform Data Visualization using matplot python library for the given datas.

# EXPLANATION:
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data.

# Algorithm:
STEP 1:Include the necessary Library.

STEP 2:Read the given Data.

STEP 3:Apply data visualization techniques to identify the patterns of the data.

STEP 4:Apply the various data visualization tools wherever necessary.

STEP 5:Include Necessary parameters in each functions.

# Coding and Output:

```
import matplotlib.pyplot as plt
x_val = [0,1,2,3,4,5]
y_val = [0,1,4,9,16,25]
plt.plot(x_val,y_val)
plt.show()
```
![326323870-c3b1567c-eda6-46f9-97c0-5edcbc751613](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/d7d92972-4b97-4841-ab7a-70f7a56b8e8d)

```
import matplotlib.pyplot as plt
x = [1,2,3]
y = [2,4,1]
plt.plot(x,y)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My first graph')
plt.show()
```
![326323898-0e9fe2e2-0d99-4f7e-bdb7-85543ac9252b](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/7248a80b-c0b2-43d6-8dd9-13c9ba348e70)

```
import matplotlib.pyplot as plt
x1 = [1,2,3]
y1 = [2,5,3]
plt.plot(x1,y1,label = 'line 1')
x2 = [1,2,3]
y2 = [3,1,6]
plt.plot(x2,y2,label = 'line 2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title("Two lines on the same graph")
plt.legend()
plt.show()
```
![326323923-7678c654-4c38-4d56-9739-82c396ee8ada](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/9694ef58-0b87-49e9-a281-a70d06ebca2c)

```
import matplotlib.pyplot as plt
import numpy as np
x = [1,2,3,4,5]
y1 = [10,12,14,16,18]
y2 = [5,7,9,11,13]
y3 = [2,4,6,8,10]
plt.fill_between(x,y1,color = 'blue')
plt.fill_between(x,y2,color = 'orange')
```
![326323942-73207267-25b7-4d47-8ddc-8de6c259faa8](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/731da65b-c04a-4937-9ac3-752b9f592564)

```
plt.stackplot(x,y1,y2,y3,labels = ['line1','line2','line3'])
plt.legend(loc = 'upper left')
plt.title('Stacked line charts')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.show()
```
![326323981-85a5c274-6f3c-4644-916f-8911a32ab070](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/ab83c4b0-dcef-404a-9697-7eadadfff36b)


```
import numpy as np
import matplotlib.pyplot as plt
val = [2,4,7,3]
names = ['A','B','C','D']
plt.bar(names, val,color = 'purple')
plt.show()
```
![326324010-bbef76a4-0018-454e-81af-c4c29f91cc01](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/1df9ae73-abe4-4b51-bc89-41184ed7fb2b)


```
import matplotlib.pyplot as plt
import numpy as np
ages = [2,6,4,12,13,12,16,18,18,19,26,24,39,34,45,42,54,56,90,56,86,79]
range = (0,100)
bins = 10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('no of people')
plt.title('histogram')
plt.show()
```

![326324408-45c9d44d-536f-4d4b-a30a-a1556a5e4762](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/66068b55-745d-46e4-a02d-bd4d1f4d5dc0)


```
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
```

![326324171-57013638-cf5c-4384-807d-a5ae720fac62](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/cec76ee1-a050-4968-b6ab-0257bd348d36)

```
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel("data")
ax.set_ylabel("values")
ax.set_title("box plot")
```

![326324369-c1307c5c-99e4-4e67-b0a0-2a59ef9eecc6](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/43dbeac9-0b61-4bf4-ac08-791a4b76c383)


```
import matplotlib.pyplot as plt
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels = slices,colors=colors,startangle=90,shadow = True,explode = (0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
plt.show()
```
![326324333-aff6791e-db9d-4bff-8f4a-6ee9444d5913](https://github.com/kanimozhipannerselvam/EXNO-5-DS/assets/119476060/25a8f714-1b81-4f8f-87ee-2de131db817c)


# Result:
  Thus, We have successfullu performed Data Visualization using matplot python library for the given datas.
