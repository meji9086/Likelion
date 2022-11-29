# 🦁 Likelion 🦁
**Likelion AI SCHOOL7** 국비 교육에서의 프로젝트 (본인 코드)

|순번|제목|개요|파이프라인|배포|             
|:------:|:---:|:------:|:------:|:------:|             
|1|웹툰 순위 분석|BeautifulSoup과 Requests를 이용해 웹툰 순위를 조사한다.|weboon_rank.py|                            
|2|이혼 사유 분석|지역별 이혼 사유에 대해 시각화하고 분석한다.|reason_of_divorce.py|          
|3|교통사고 원인 분석|법규위반에 대한 교통사고 원인을 시각화하고 분석한다.|traffic_accident.py|<img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=A8B9CC"/>     
|4|제주도 도로 교통량 예측|제주도 도로 교통 데이터를 가지고 EDA 및 Modeling을 한다.|traffic_predict_in_Jeju.py|           

## ✏ mini project      
### 1️⃣ Webtoon Rank        

**BeautifulSoup과 Requests를 이용한 웹툰의 순위를 가져오기**      

![image](https://user-images.githubusercontent.com/72390138/196094124-b7ba960b-8b29-4732-8d1d-6f0e9c52460c.png)

---

### 2️⃣ Reason of divorce by region by year

**지역별 연도별 이혼 사유에 대해 분석하기**                 

![image](https://user-images.githubusercontent.com/72390138/196094866-25ca9a0e-7332-47c6-a8c3-799c7ddec738.png)
![image](https://user-images.githubusercontent.com/72390138/196095208-b38309f4-e758-4f33-94da-c4165504affd.png)
 
이혼 사유에는 성격 차이가 가장 큰 원인이 된다고 볼 수 있다.             
또한, 지역으로는 경기도, 서울특별시가 가장 많으나 이는 인구밀도지역으로 인한 차이라고 볼 수 있다.

---

### 3️⃣ Road Traffic Forecasts in Jeju Island         

📌 github : meji9086/Jeju-Traffic-Forecast 참고          

**제주도 도로 교통량 예측하기**         
#### EDA             

![image](https://user-images.githubusercontent.com/72390138/201580818-0244acd5-e286-4ed5-832d-e418e5c14607.png)            
- base_date : 2022년 7월 기준으로 교통량 증가하였다. 이는 코로나 접종 이후 처음 거리두기가 풀린 여름 휴가로 인한 급증이라고 볼 수 있다.              
- base_hour : 00시-05시,18시-24시에 교통량 감소하였고, 05시-18시 교통량 증가하였다(차이가 큼).       
- day_of_week : 금요일에 교통량 증가하였고, 주말에 교통량 감소하였다(큰차이 없음).       
- road_name : '-'으로 기록된 null값이 존재한다.         

![image](https://user-images.githubusercontent.com/72390138/201581387-15fb2df7-c880-4392-bd4b-8df391d18397.png)          
- year : 뚜렷한 차이 없다.          
- month : 7월 교통량 급증가하였다. 이는 여름 휴가를 원인으로 볼 수 있다.        
- day : 뚜렷한 차이 없다.            
- 월별 차이가 제일 뚜렷한 것을 볼 수 있다.          

#### Modeling           
**LightGBM**을 이용해 교통량 예측하였다.                
<img src="https://user-images.githubusercontent.com/72390138/201582425-1f6c99e5-a940-4b44-9863-3e2568d934ef.png" width="380" height="480">    
**GridSearchCV**를 이용한 최적의 하이퍼 파라미터 : {'learning_rate': 0.05, 'max_depth': 5, 'min_child_samples': 5, 'num_leaves': 20}            
test data MAE 점수 : 5.77352                   


---

## ✏ mid project
### Analysis of the cause of traffic accidents by violation of laws and regulations          

📌 github : meji9086/Traffic-Accident-Data-Analysis 참고

**법규위반별 교통사고 원인 분석**                     

![image](https://user-images.githubusercontent.com/72390138/197454540-5b545e1c-e2a6-4af8-a251-371c09cb7b48.png)          

교통사고의 원인으로는 신호위반, 안전거리미확보 그리고 교차로운행방법위반으로 볼 수 있다.            

![image](https://user-images.githubusercontent.com/72390138/197454577-9c6bce18-a97c-49ba-a9b1-1be68e7e6948.png)            

하지만, 사망자는 과속으로 많이 발생한다는 것을 알 수 있다.            


**☘ 해결방안 제시**            
1. 신호위반에 대한 법의 강화 또는 벌칙금을 증가시킨다.           
2. 과속 할 수 있는 구간에 CCTV 추가설치 및 과속 벌칙금 증가시킨다.          

---
