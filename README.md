# ncl_basic
ncl functions and resources decription

## 유용한 함수
   
### 월별 평균 [clmMonTLL(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLL.shtml)   
Calculates long term monthly means (monthly climatology) from monthly data: (time,lat,lon) version    
   
__Arguments__   
(시간, 위도, 경도)로 이루어진 3차원 행렬   
   
__Return value__   
An array of the same size and type as x except that the leftmost dimension will be of size 12.   
    
###### 자매품 [clmMonTLLL(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLLL.shtml), [clmMonLLT(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLT.shtml), [clmMonLLLT(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLLT.shtml)
---------------------------------------------------------------------------------------------------------------------------------------------------------------------
### 연 합계 / 연평균 [month_to_annual(X, opt)](https://www.ncl.ucar.edu/Document/Functions/Contributed/month_to_annual.shtml)
Converts monthly values to annual values.   
   
__Arguments__   
__X__ = 월별 자료, 다차원 자료인 경우에 첫번째 차원이 시간 차원이어야 함.   
__opt__ = 0 : 월별 자료의 연 합계 / 1 : 연 평균

__Return value__   
시간 차원이 연도로 변경, 매개변수에 fillvalue 데이터가 있으면 결과도 fillvalue로 나옴.   
*Note: Upon return the 'temporal' dimension will be named year to avoid confusing dimension names.*

---------------------------------------------------------------------------------------------------------------------------------------------------------------------
