# Pandas Practice
```python
sr1[[0,2]] # 시리즈에서 슬라이싱처럼 이어서 출력하는거 외에 갭을둬서 출력하는것도 가능

df = pd.DataFrame({'food': ["KFC",'McDonald','School'],'price' : [1000,2000,2500], 'rating' : [4.5,3.9,4.2]})
print(df) # dict로 DataFrame 만들기

'''
DataFrame indexing
 df.food = "place" #값이 바뀜
 df"food"] = "place" 도 값만 바뀜/ 이거는 인덱싱

DataFrame Colums의 이름 바꾸기 .rename()
 df.rename(columns = {'food':'place'}, inplace = True)
'''
import numpy as np

np1 = np.arange(0, 8) 
gohome = np1.reshape(2, 4)

df = pd.DataFrame(gohome, columns= ['0','1','2','3'])

# columns도 이름 설정 따로 하지 않으면 0,1,2,3인가보다.



```