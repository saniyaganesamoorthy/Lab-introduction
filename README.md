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



	


