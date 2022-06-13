## 눈금
__tmXBOn__ : x축 bottom 틱마커 On/Off | True, False

__tmXBMode__ : x축 bottom 틱마커 모드 변경 "Manual", "Explicit"
* Manual :
* Explicit : 
  * __txXBValues__ : x축 bottom에 틱마커를 표시할 값들
  * __txXBLabels__ : x축 bottom 틱마커 레이블
      
__tmXMajorGrid__ : x축 major 틱마커의 grid line On/Off | True, False

__tmXMajorGridLineDashPattern__ : grid line의 선 모양 설정

__gsnTickMarksOn__ : 자동적으로 그려주는 눈금 제거 ex) gsn_csm_contour_polar() 등등
   
## 산포도
xy-plot의 모드를 바꿔서 그린다. 

__xyMarkLineMode__ :  xy_plot의 형태 결정 | "lines", "markers", "markLines"  

__xyMarkers__ : 점 모양 설정 | 0~16   

__xyMarkerSizes__ : 마커의 크기 설정 | default=0.01   

__xyMarkerThicknesses__ : 마커 선의 굵기 설정 | default=1.0   
   

## 투영법
__mpProjection__ : 지도 투영법 설정 | "LambertConformal", "CylindricalEquidistant", "Robinson", "Stereographic" 등등
* __LambertConformal__ : 람베르트 정각원추도법. 중위도 지역에서 대체로 사용
  * __mpLambertMeridianF__ : 투영법 중심 경도 설정
  * __mpLambertParallel1F__ : 투영법이 교차하는 위도 1층 (대체로 30도)
  * __mpLambertParallel2F__ : 투영법이 교차하는 위도 2층 (대체로 60도)   

__mpCenterLatF__ : 지도 중심 위도 설정

__mpCenterLonF__ : 지도 중심 경도 설정

__mpLimitMode__ : 지도 범위 설정 방법 | "LatLon", "Corners"
* __LatLon__ : 최대, 최소 위경도를 통해 지도 범위 설정
  * __mpMinLatF__ : 최소 위도 설정
  * __mpMaxLonF__ : 최대 경도 설정
* __Corners__ : 좌측 하단 구석 위경도, 우측 상단 위경도를 통해 지도 범위 설정, 정각원추도법일 때 많이 사용
  * __mpLeftCornerLatF__ : 좌측 하단 구석 위도 설정
  * __mpRightCornerLonF__ : 우측 상단 구석 경도 설정

__mpGridAndLimbOn__ : grid line과 틱마커 On/Off | True, False  

__mpGridLineDashPattern__ : grid line의 선 모양 결정 | 0~16   

__mpGridLineThicknessF__ : grid line의 선 굵기 결정 | default=1.0   

__pmTickMarkDisplayMode__ : 틱마커 표현 여부 | "NoCreate", "Never", "Always"


## 등고선
__cnLinesOn__ : 등고선 선 On/Off | True, False

__cnFillOn__ : 등고선 색칠 On/Off | True, False


## 범례
__lgItemType__ : 범례에 쓰일 모양 | "Lines", "MarkLines", "Markers", default="Lines"

__lgLineColors__ : 범례에 쓰이는 선 색깔

__lgMarkerColors__ : 

__lgMarkerIndexes__ : 개별로 마커 모양 선택 | 0~16

__lgMarkerSizeF__ : 마커 크기 변경

__lgDashIndexes__ : 개별로 선 모양 선택 | 0~16

##### 참고 : [gsn_create_legend(workstation, 범례 개수, 범례 이름, res)](https://www.ncl.ucar.edu/Document/Graphics/Interfaces/gsn_create_legend.shtml)

## label
__lbTilteOn__ : label 제목 on/off, lbTitleString속성을 설정하면 default True | True, False

__lbTitleString__ : label 제목 내용

__lbOrientation__ : label 방향 | "Vertical", "Horizontal"

__lbBottomMarginF__ : label Perimeter로부터 margin 설정 가능, Top Left Right 도 가능


## annotation manager
__amParallelPosF__ : 범례 좌우 이동

__amOrthogonalPosF__ : 범례 상하 이동

##### 참고 : [gsn_add_annotation(plot, legend ID, res)](https://www.ncl.ucar.edu/Document/Graphics/Interfaces/gsn_add_annotation.shtml)

