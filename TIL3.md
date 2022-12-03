

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