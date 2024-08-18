# Lab-introduction
# Program 1:
```
import pandas as pd
df=pd.DataFrame({"a":[4,5,6],"b":[7,8,9],"c":[10,11,12]},index=[1,2,3])
df
```
# Output:
![Screenshot 2024-08-18 100912](https://github.com/user-attachments/assets/de11a0b3-5f9e-4182-ab00-ba6da1fcdd50)
# Program 2:
```
import pandas as pd
df=pd.DataFrame([[4,5,6],[7,8,9],[10,11,12]],index=[1,2,3],columns=['a','b','c'])
df
```
# Output :
![Screenshot 2024-08-18 101057](https://github.com/user-attachments/assets/971f9506-20f0-4e87-ad96-fe87086ccb9a)

# Program 3:
```
import pandas as pd 
data = [1,2,3,4] 
df = pd.DataFrame(data) 
print (df)
data = [['Alex',10],['Bob',12]]
df = pd.DataFrame(data,columns=['Name','Age']) 
print (df)
```
# Output :
![Screenshot 2024-08-18 101236](https://github.com/user-attachments/assets/077795f2-70f3-4ca1-954a-6a7f13cb038a)

# Program 4:
```
import pandas as pd 
data = {'Name':['Tom', 'Jack', 'Steve', 'Ricky'],'Age':[28,34,29,42]} 
df = pd.DataFrame(data) 
print(df)
```
# Output:
![Screenshot 2024-08-18 101346](https://github.com/user-attachments/assets/6ec8c8e3-703e-4f8d-8b90-95be5513deae)

# Program 5:
```
import pandas as pd
mydataset = {'cars': ["BMW", "Volvo", "Ford"],'passings': [3, 7, 2]}
myvar = pd.DataFrame(mydataset)
print(myvar)
```
# Output:
![Screenshot 2024-08-18 101438](https://github.com/user-attachments/assets/6e727a7c-3339-4b90-ad54-87d56e05042a)
# Program 6:
```
data = [{'a': 1, 'b': 2},{'a': 5, 'b': 10, 'c': 20}]
df = pd.DataFrame(data, index=['first', 'second'])
df
```
# Output:
![Screenshot 2024-08-18 101543](https://github.com/user-attachments/assets/55c067cc-2a56-4593-bc74-2c8f50916ffd)
# Program 7:
```
data = [{'a': 1, 'b': 2},{'a': 5, 'b': 10, 'c': 20}]
df1 = pd.DataFrame(data, index=['first', 'second'], columns=['a', 'b'])
df1
```
# Output:
![Screenshot 2024-08-18 101643](https://github.com/user-attachments/assets/e8ddbde3-d008-4b76-ac2d-4ea31f7ca9ea)
# Program 8:
```
import pandas as pd
data = {'Name': ['Jai', 'Princi', 'Gaurav', 'Anuj'], 'Height': [5.1, 6.2, 5.1, 5.2], 'Qualification': ['Msc', 'MA', 'Msc', 'Msc']} 
df = pd.DataFrame(data) 
address = ['Delhi', 'Bangalore', 'Chennai', 'Patna'] 
df['Address'] = address 
print(df)
```
# Output:
![Screenshot 2024-08-18 101738](https://github.com/user-attachments/assets/b1542443-f534-4c47-9d81-0c841d3e61ba)

# Program 8:
```
import pandas as pd
data = {'Name':['Jai', 'Princi', 'Gaurav', 'Anuj'], 'Age':[27, 24, 22, 32], 'Address':['Delhi', 'Kanpur', 'Allahabad', 'Kannauj'],'Qualification':['Msc', 'MA', 'MCA', 'Phd'],'address':['Delhi', 'Bangalore', 'Chennai', 'Patna'] } 
df = pd.DataFrame(data) 
del df['Address']
df
```
# Output:
![Screenshot 2024-08-18 101830](https://github.com/user-attachments/assets/7c038004-d257-4aad-8184-6bc21b4e9640)
# Program 9:
```
import pandas as pd
data = {'Name':['Jai', 'Princi', 'Gaurav', 'Anuj'], 'Age':[27, 24, 22, 32], 'Address':['Delhi', 'Kanpur', 'Allahabad', 'Kannauj'],'Qualification':['Msc', 'MA', 'MCA', 'Phd'],'address':['Delhi', 'Bangalore', 'Chennai', 'Patna'] } 
df = pd.DataFrame(data)
df.drop(['Address'],axis=1,inplace=True)
df
```
# Output:
![Screenshot 2024-08-18 101925](https://github.com/user-attachments/assets/f1067083-3b5e-4a67-be67-94a00e6d172d)
# Program 10:
```
import pandas as pd
data={'Name':['jai','anuj'],'Age':[12,25],'Address':['Delhi','Kanpur'],'Qualification':['Msc','MA']}
df=pd.DataFrame(data)
print(df)
df.rename(columns={'Address':'place'},inplace=True)
print(df)
```
# Output:
![Screenshot 2024-08-18 102018](https://github.com/user-attachments/assets/c4099129-6646-4634-aedd-0b11163e72e6)
# Program 11:
```
import pandas as pd
df=pd.DataFrame([[1,2],[3,4]],columns=['a','b'])
df2=pd.DataFrame([[5,6],[7,8]],columns=['a','b'])
df=pd.concat([df,df2])
df
```
# Output:
![Screenshot 2024-08-18 102154](https://github.com/user-attachments/assets/956acc58-be05-4144-b4ed-ff605bf66de5)
# Program 12:
```
import pandas as pd
data={'Name':['jai','anuj'],'Age':[12,25],'Address':['Delhi','Kanpur'],'Qualification':['Msc','MA']}
df=pd.DataFrame(data)
df
df.drop(0,axis=0,inplace=True)
df
```
# Output:
![Screenshot 2024-08-18 102247](https://github.com/user-attachments/assets/478289f8-1140-4d4f-b6a4-87d69e6cea5b)
# Program 13:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Dave'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df=df['name']
df
```
# Output:
![Screenshot 2024-08-18 102432](https://github.com/user-attachments/assets/18f4623e-4886-4fc7-8ba3-15fc000ff428)

# Program 14:
```
import pandas as pd
data={'Name':['jai','anuj'],'Age':[12,25],'Address':['Delhi','Kanpur'],'Qualification':['Msc','MA']}
df=pd.DataFrame(data)
print(df[['Name','Qualification']])
```
# Output:
![Screenshot 2024-08-18 102516](https://github.com/user-attachments/assets/dffdeebf-9378-4285-90d1-4bd8fc2b090f)

# Program 15:
```
import pandas as pd
data={'Name':['jai','anuj'],'Age':[12,25],'Address':['Delhi','Kanpur'],'Qualification':['Msc','MA']}
df=pd.DataFrame(data)
df.filter(items=['Name','Age'])
```
# Output:
![Screenshot 2024-08-18 102553](https://github.com/user-attachments/assets/b8030916-9994-4521-8ac3-3f4e0ad78bae)

# Program 16:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Dave'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df.filter(regex='e|a',axis=1)
```
# Output:
![Screenshot 2024-08-18 102625](https://github.com/user-attachments/assets/13d56813-516d-4979-814e-f03d63e48375)

# Program 17:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df=df.drop_duplicates()
df
```
# Output:
![Screenshot 2024-08-18 102655](https://github.com/user-attachments/assets/a1340945-2fed-4b7e-b1eb-380586b47e50)
# Program 18:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'salary':[5000,600000,80000,200000]}
df=pd.DataFrame(data)
top_salaries=df.nlargest(2,columns='salary')
print(top_salaries)
```
# Output:
![Screenshot 2024-08-18 102845](https://github.com/user-attachments/assets/c741cd73-af3f-4810-b690-ef3194787dc9)

# Program 19:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'salary':[5000,600000,80000,200000]}
df=pd.DataFrame(data)
top_salaries=df.nsmallest(2,columns='salary')
print(top_salaries)
```
# Output:
![Screenshot 2024-08-18 102920](https://github.com/user-attachments/assets/6348441c-41ef-4f60-830e-1ddf9bef97ea)

# Program 20:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df=df.query('age >= 30')
print(df)
```
# Output:
![Screenshot 2024-08-18 102950](https://github.com/user-attachments/assets/4140702a-6aac-45cb-8bb8-a2d5daf1b3d5)

# Program 21:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df=df.query('name.str.contains("e") and height > 1.7')
print(df)
```
# Output:
![Screenshot 2024-08-18 103029](https://github.com/user-attachments/assets/2f1557fb-3ac9-4cb8-ac62-07ff84367660)

# Program 22:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df=df.query('gender == ["F","M"] and height > 1.7')
print(df)
```
# Output:
![Screenshot 2024-08-18 103112](https://github.com/user-attachments/assets/35664b21-c77a-4ec1-945e-8e12ddba4a51)

# Program 23:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df.loc[:,'age']
```
# Output:
![Screenshot 2024-08-18 103155](https://github.com/user-attachments/assets/776ed253-71dc-4131-8bb8-298a416814c3)
# Program 24:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df.iloc[:,1]
```
# Output:

# Program 25:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df.loc[:,['name','age']]
```
# Output:

![Screenshot 2024-08-18 103725](https://github.com/user-attachments/assets/4461d869-8c40-429d-969e-40ae7acaeb8a)

# Program 26:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df.iloc[:,0]
```
# Output:
![Screenshot 2024-08-18 103849](https://github.com/user-attachments/assets/7a7cd7e5-7ed6-4675-84c6-b874b34ae5d6)

# Program 27:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df_filtered=df[df['age']>30]
print(df_filtered)
```

# Output:
![Screenshot 2024-08-18 103933](https://github.com/user-attachments/assets/fcc8d304-ce56-42f3-a11f-5194e87d0c5f)

# Program 28:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df_filtered=df[(df['gender']=='M') & (df['height']>1.7)]
print(df_filtered)
```
# Output:
![Screenshot 2024-08-18 103933](https://github.com/user-attachments/assets/323f22fc-d038-4df8-9f71-22100407473c)
# Program 29:
```
import pandas as pd
data={'name':['Alice','Bob','Charlie','Alice'],'age':[25,56,23,42],'gender':['F','M','M','M'],'height':[1.62,1.78,1.65,1.83]}
df=pd.DataFrame(data)
df_filtered=df[df['name'].str.startswith(('A','C'))]
print(df_filtered)
```
# Output:
![Screenshot 2024-08-18 104229](https://github.com/user-attachments/assets/e7d23b54-b947-4b7b-9c0b-7ada0f7b5964)

# Program 30:
```
  import pandas as pd
  data={'Name':['John','Sarah','Mike','Emily','David'],'Age':[25,31,29,35,27],'Gender':['M','F','M','F','M'],'Salary':[50000,70000,60000,80000,55000]}
  df=pd.DataFrame(data)
  print(df.tail(3))
```
# Output:
![Screenshot 2024-08-18 104303](https://github.com/user-attachments/assets/77b64661-1ef8-41ad-bedb-bdc89f152f4f)

# Program 31:
```
  import pandas as pd
  data={'Name':['John','Sarah','Mike','Emily','David'],'Age':[25,31,29,35,27],'Gender':['M','F','M','F','M'],'Salary':[50000,70000,60000,80000,55000]}
  df=pd.DataFrame(data)
  print(df.head(3))
```
# Output:
![Screenshot 2024-08-18 104329](https://github.com/user-attachments/assets/397c11eb-ecb7-4ef9-a834-eff51c036633)

# Program 32:
```
  import pandas as pd
  data={'Name':['John','Sarah','Mike','Emily','David'],'Age':[25,31,29,35,27],'Gender':['M','F','M','F','M'],'Salary':[50000,70000,60000,80000,55000]}
  df=pd.DataFrame(data)
  df.info()
```
# Output:
![Screenshot 2024-08-18 104506](https://github.com/user-attachments/assets/9dfd3085-2d8a-4b84-8299-6dc6ba2fd192)

# Program 33:
```
  import pandas as pd
  data={'Name':['John','Sarah','Mike','Emily','David'],'Age':[25,31,29,35,27],'Gender':['M','F','M','F','M'],'Salary':[50000,70000,60000,80000,55000]}
  df=pd.DataFrame(data)
  print(df.describe())
```
# Output:
![Screenshot 2024-08-18 104537](https://github.com/user-attachments/assets/a956fd4f-2f9d-4468-897d-a86161cfc6d0)

# Program 34:
```
import pandas as pd
data={'Name':['John','Sarah','Mike','Emily','David'],'Age':[25,31,29,35,27],'Score':[90,80,85,95,78]}
df=pd.DataFrame(data)
df_sorted=df.sort_values(by='Age',ascending=False)
print(df_sorted)
```

# Output:
![Screenshot 2024-08-18 104629](https://github.com/user-attachments/assets/45736080-38ec-4396-84b1-c8b3a6a9d944)

# Program 35:
```
import pandas as pd
data={'name':['John','Sarah','Mike','Emily','David'],'gender':['M','F','M','F','M'],'age':[25,31,29,35,27],'salary':[50000,70000,60000,80000,55000]}
df=pd.DataFrame(data)
grouped=df.groupby('gender').mean()['salary']
print(grouped)
```
# Output:
![Screenshot 2024-08-18 104806](https://github.com/user-attachments/assets/7eda1911-d1fe-4404-8899-48656ef18717)



















	


