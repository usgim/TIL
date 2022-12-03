```python
index = ["037730", "036360", "005760"]
data = [["3R", "1510"],
         ["3SOFT", 1790],
         ["ACTS", 1185]]
columns = ["종목명", "현재가"]
df = pd.DataFrame(data=data, index=index, columns=columns)

df.reset_index(inplace = True) # .reset_index()는 인덱스 값들을 DF의 열로 전송하고 새로운 정소인덱스를 세팅한다.

 index	   종목명	현재가
0	037730	3R	1510
1	036360	3SOFT	1790
2	005760	ACTS	1185

df.set_index('종목코드', inplace=True) # 임의의 index 목룩 추가, index위 종목코드

	종목명	현재가	등락률
종목코드			
037730	3R	1510	7.36
036360	3SOFT	1790	1.65
005760	ACTS	1185	1.28


data = [
    ["037730", "3R", 1510, 7.36],
    ["036360", "3SOFT", 1790, 1.65],
    ["005760", "ACTS", 1185, 1.28],
]
columns = ["종목코드", "종목명", "현재가", "등락률"]
df = pd.DataFrame(data=data, columns=columns)
df.set_index('종목코드', inplace=True)

df[["현재가"]] # 칼럼을 인덱싱 후 데이터프레임 타입으로 들기. [[]]


```