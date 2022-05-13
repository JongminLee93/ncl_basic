# ncl_basic
ncl functions and resources decription

## 유용한 함수
#### 월별 평균 [clmMonTLL(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLL.shtml)   
__Arguments__   
A three-dimensional array of type float or numeric.
* Dimensions must be time, lat, lon. 
* The time dimension must be a multiple of 12. 
* The dimensions must be named.   
   
__Return value__   
An array of the same size and type as x except that the leftmost dimension will be of size 12.   
   
Calculates long term monthly means (monthly climatology) from monthly data: (time,lat,lon) version   
    
자매품 [clmMonTLLL(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonTLLL.shtml), [clmMonLLT(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLT.shtml), [clmMonLLLT(X)](https://www.ncl.ucar.edu/Document/Functions/Contributed/clmMonLLLT.shtml)
