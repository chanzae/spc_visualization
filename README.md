# Intro
SPC 브랜드 매장 정보를 크롤링을 통해 수집하고 시각화하여 분석하였습니다.<br> 
본 프로젝트는 [링크](https://hellp-world.tistory.com/327)에서 확인할 수 있습니다.
<br>
<br>

# Process
- Crawling : BeautifulSoup, selenium을 이용하여 SPC 브랜드 각 홈페이지와 네이버 지도 검색 등을 크롤링 하였습니다.
- Preprocessing : 수집된 데이터를 병합하여 중복 제거, 결측치 처리, 컬럼 제거, geocoding을 통한 위경도 좌표 추가 및 상세 주소 수정을 진행하였습니다.
- Visualization : plotly를 이용하여 bar graph, treemap을 구현하였고, folium을 이용하여 choropleth을 구현하였습니다. 이외 matplotlib을 사용하였습니다.
<br>
<br>

# Data Info
- datasets : spc_geo_final_230222.csv
- date : 23.02.22 
- shape : 6530 rows x 8 columns
- columns 
	- brand : 브랜드명
	- branch : 지점명
	- addr : 상세 주소
	- sido : 시도명
	- sigugun : 시구군명
	- dongmyun : 읍면동명
	- lat : 위도
	- lng : 경도
