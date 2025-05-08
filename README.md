# NAME: MOHANRAJ.S
# REG NO: 212224100036
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
~~~python
import pandas as pd
import numpy as np
import seaborn as sns
import matplotlib.pyplot as plt
x = [1, 2, 3, 4, 5]
y = [3, 6, 2, 7, 1]
plt.plot(x,y,label='line1')
~~~
![image](https://github.com/user-attachments/assets/7e002c55-b7c3-43f9-8d47-448520474672)
~~~python
x1 = [1,2,3]
y1 = [2,4,1]
x2 = [1,2,3]
y2 = [4,1,3]

plt.plot(x1,y1,label='line1')
plt.plot(x2,y2,label='line2')
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Two lines on same graph!')
plt.legend()
plt.show()
~~~
![image](https://github.com/user-attachments/assets/9b928f87-fbed-4c0f-a00b-fa21c5bc5711)
~~~python
import matplotlib.pyplot as plt
x=[1,2,3,4,5,6]
y=[2,4,1,5,2,6]
plt.plot(x,y,color='green',linestyle='dashed',linewidth=3,marker='o',markerfacecolor='blue',markersize=12)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('Some cool customizations!')
plt.show()

~~~
![image](https://github.com/user-attachments/assets/315973e9-7463-4f9d-9b69-54791d0a04f9)
~~~python
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(yield_apples)
~~~
![image](https://github.com/user-attachments/assets/050155f4-4684-46ac-ae02-6ca42549d8f2)
~~~python
years=[2010,2011,2012,2013,2014,2015]
yield_apples=[0.895,0.91,0.919,0.926,0.929,0.931]
plt.plot(years,yield_apples)
~~~
![image](https://github.com/user-attachments/assets/a40f0d77-ad35-4956-9770-d43a29183929)
~~~python
years=range(2000,2012)
apples=[0.895,0.91,0.919,0.926,0.929,0.931,0.934,0.936,0.937,0.9375,0.9372,0.939]
oranges=[0.926,0.941,0.930,0.923,0.918,0.908,0.907,0.904,0.901,0.898,0.9,0.896, ]
plt.plot(years, apples)
plt.plot(years, oranges)
plt.xlabel('Year')
plt.ylabel('Yield (tons per hectare)')
plt.title('Crop Yields in Kanto')
plt.legend(['Apples','Oranges']);
~~~
![image](https://github.com/user-attachments/assets/8300ce7b-0302-42a7-80b5-61ca025953d4)
~~~python
plt.figure(figsize=(12,6))
plt.plot(years,oranges,marker='o')
plt.title("Yield of Oranges (tons per hectare)");
~~~
![image](https://github.com/user-attachments/assets/45c483a9-409e-48f5-b476-283886eb7877)
~~~python
import matplotlib.pyplot as plt
import numpy as np
import pandas as pd
x=np.arange(0,10)
y=np.arange(11,21)
x
~~~
![image](https://github.com/user-attachments/assets/a10f59a9-dd4c-4e24-b5d3-8e6a61547bf0)
~~~python
y
~~~
![image](https://github.com/user-attachments/assets/9516dea1-bca9-414e-a46b-a45de3cac7d0)
~~~python
plt.scatter(x,y,c='r')
plt.xlabel('X-axis')
plt.ylabel('Y-axis')
plt.title('Graph in 2D')
plt.savefig('Test.png')
~~~
![image](https://github.com/user-attachments/assets/9505b454-d5cf-4259-b66f-048ae70fc39a)
~~~python
y=x*x
y
~~~
![image](https://github.com/user-attachments/assets/e7c7e69e-351e-49f7-bf14-5b3ff0f52c33)
~~~python
plt.plot(x,y,'g*',linestyle='dashed',linewidth=2,markersize=12)
plt.xlabel('X axis')
plt.ylabel('Y axis')
plt.title('2d Diagram')
plt.legend(['y-values']);
~~~
![image](https://github.com/user-attachments/assets/744982cb-a4ff-4e8d-86cc-c1d50a5d8eac)
~~~python
x=np.arange(0,4*np.pi,0.1)
y=np.sin(x)
plt.title("sine wave form")
plt.plot(x,y)
plt.show()
~~~
![image](https://github.com/user-attachments/assets/f88c7007-b80b-4a9a-bc7e-ae92711b9a7a)
~~~python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
~~~
![image](https://github.com/user-attachments/assets/3245b2e2-e6d9-4596-ab93-3cb6fa132039)
~~~python
import matplotlib.pyplot as plt
import numpy as np
x=[1,2,3,4,5]
y1=[10,12,14,16,18]
y2=[5,7,9,11,13]
y3=[2,4,6,8,10]
plt.fill_between(x,y1,color='blue')
plt.fill_between(x,y2,color='green')
plt.plot(x,y1,color='red')
plt.plot(x,y2,color='black')
plt.legend(['y1','y2'])
plt.show()
~~~
![image](https://github.com/user-attachments/assets/3d71d075-a32a-43d2-8936-00b1126e97e3)
~~~python
import matplotlib.pyplot as plt
height=[10,24,36,40,5]
names=['one','two','three','four','five']
c1=['red','green']
c2=['b','g']
plt.bar(names,height,width=0.8,color=c1)
plt.xlabel('x-axis')
plt.ylabel('y-axis')
plt.title('My bar chart!')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/448ee9cd-226c-4add-97b8-2156fcc8e653)
~~~python
x=[2,8,10]
y=[11,16,9]
x2=[3,9,11]
y2=[6,15,7]
plt.bar(x,y,color='r')
plt.bar(x2,y2,color='g')
plt.title('Bar graph')
plt.ylabel('Y axis')
plt.xlabel('X axis')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/d8a21162-fbcf-489a-a886-d586044c12a0)
~~~python
import matplotlib.pyplot as plt
ages=[2,5,70,40,30,45,50,45,43,40,44,60,7,13,57,18,90,77,32,21,20,40]
range=(0,100)
bins=10
plt.hist(ages,bins,range,color='green',histtype='bar',rwidth=0.8)
plt.xlabel('age')
plt.ylabel('No. of people')
plt.title('My histogram')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/7c45f4bc-1c04-4f21-b5dd-5a1a13575cbf)
~~~python
import matplotlib.pyplot as plt
import numpy as np
np.random.seed(0)
data=np.random.normal(loc=0,scale=1,size=100)
data
~~~
![image](https://github.com/user-attachments/assets/a822f0d5-441e-45b8-84c9-a54b84b1f5ab)
~~~python
fig,ax=plt.subplots()
ax.boxplot(data)
ax.set_xlabel('Data')
ax.set_ylabel('Values')
ax.set_title('Box Plot')
~~~
![image](https://github.com/user-attachments/assets/cd61305b-a7c0-437d-b503-0cb6b56f269c)
~~~python
labels='Python','C++','Ruby','Java'
sizes=[215,130,245,210]
colors=['gold','yellowgreen','lightcoral','lightskyblue']
explode=(0,0.4,0,0.5)
plt.pie(sizes,explode=explode,labels=labels,colors=colors,autopct='%1.1f%%',shadow=True)
plt.axis('equal')
plt.show()
~~~
![image](https://github.com/user-attachments/assets/cdbb8854-188f-4f3c-a9f3-e6ff76d3dd52)
~~~python
activities=['eat','sleep','work','play']
slices=[3,7,8,6]
colors=['r','y','g','b']
plt.pie(slices,labels=activities,colors=colors,startangle=90,shadow=True,explode=(0,0,0.1,0),radius=1.2,autopct='%1.1f%%')
plt.legend()
~~~
![image](https://github.com/user-attachments/assets/ea669d60-4162-4414-b164-961851a80714)

# Result:
 To perform Data Visualization using matpolt python library for the given data is successful.
