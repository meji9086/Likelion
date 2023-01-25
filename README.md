# 🦁 Likelion 🦁
**Likelion AI SCHOOL7** 국비 교육에서의 프로젝트 (본인 코드)

|순번|제목|개요|파이프라인|배포|             
|:-:|:-------:|:------:|:---:|:------:|             
|1|웹툰 순위 분석|BeautifulSoup과 Requests를 이용해 웹툰 순위를 조사한다.|weboon_rank.ipynb|                            
|2|이혼 사유 분석|지역별 이혼 사유에 대해 시각화하고 분석한다.|reason_of_divorce.ipynb|          
|3|교통사고 원인 분석|법규위반에 대한 교통사고 원인을 시각화하고 분석한다.|traffic_accident.ipynb|<a href="https://meji9086-traffic-accident-data-analysis-1-j6stsu.streamlit.app/"><img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=A8B9CC"/>|     
|4|제주도 도로 교통량 예측|제주도 도로 교통 데이터를 가지고 EDA 및 Modeling을 한다.|traffic_predict_in_Jeju.ipynb|      
|5|노트북 가격 예측|노트북의 정보 데이터를 가지고 EDA 및 Modeling을 통해 가격을 예측한다.|Laptop_price_predict.ipynb|       
|6|청경채 성장률 예측|인공지능을 활용하여 작물의 효율적인 생육을 위한 최적의 환경을 도출한다.|prediction_bokchoy_growth.ipynb|     
|7|마스크 착용/미착용 분류|마스크 착용/미착용 분류의 서비스를 제공하고자 한다.|Whether_to_wear_a_mask.ipynb|<a href="https://seul1230-mask-classification-main-pqg0f0.streamlit.app/"><img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=A8B9CC"/>      
|8|문장 유형 분류|AI 모델을 할용하여 언어가 쓰이는 모든 영역에서 보다 사용자 친화적인 서비스를 제공하고자 한다.|sentences_type_classification.ipynb|      
|9|브랜드 리뷰 분석|브랜드별 리뷰를 분석하여 약점과 강점을 원샷으로 도출하고자 한다.|brand_review_analysis.ipynb|<a href="https://meji9086-brand-review-analysis-withnlp-app-vqf7p3.streamlit.app/"><img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=A8B9CC"/>|    
|10|olist 기업 분석|브라질 olist 기업을 분석하여 마케팅 전략을 내세우고자 한다.|olist_corporate_analysis.ipynb|          

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

### 4️⃣ Road Traffic Forecasts in Jeju Island         

📌 github : meji9086/5nly-code-repository 참고          

**제주도 도로 교통량 예측하기**         
#### 📊 EDA             

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

#### 🔎 Modeling           
**LightGBM**을 이용해 교통량 예측하였다.                
<img src="https://user-images.githubusercontent.com/72390138/201582425-1f6c99e5-a940-4b44-9863-3e2568d934ef.png" width="380" height="480">    
**GridSearchCV**를 이용한 최적의 하이퍼 파라미터 : {'learning_rate': 0.05, 'max_depth': 5, 'min_child_samples': 5, 'num_leaves': 20}            
🍀 test data MAE 점수 : 5.77352     

---

### 5️⃣ Prediction of Laptop price

📌 github : meji9086/5nly-code-repository 참고   

**노트북 가격 예측하기**

#### 📊 EDA
   
<img src="https://user-images.githubusercontent.com/72390138/203262255-0d0271e7-9ec6-4821-9374-cb4a3f21f4f2.png" weight="550" height="450">         
Notebook의 종류가 월등하게 높은 것을 확인할 수 있다.    
이는, 들고다닐 수 있는 편의성으로 인해 구매율이 높아 생산률도 높을 것이라고 추측할 수 있다.       


<img src="https://user-images.githubusercontent.com/72390138/203263872-972f5506-cea6-42c7-a9d4-51532bb8749b.png">        
제조업은 Dell, Venovom, HP의 제품들이 월등하게 많은 것을 확인할 수 있다.     

#### 🔎 Modeling       
**RandomForestRegressor**를 이용해 노트북 가격을 예측하였다.   
<img src="https://user-images.githubusercontent.com/72390138/203267744-ff0cd8ac-0508-4c54-bf62-476a704473bc.png" weight="500" height="400">         
feature 간 중요도는 **1위 RAM, 2위 Peso(무게)** 순으로 높은 것을 알 수 있다.       
🍀 test data RMSE : 402    
 
---
 

### 6️⃣ Prediction of bokchoy growth      

📌 github : meji9086/5959-deeplearning-project 참고      
 
**청경채 성장률 예측하기**

#### 📊 EDA       
![image](https://user-images.githubusercontent.com/72390138/214470196-65552494-6942-46d4-a248-833c866abb64.png)     
내부온도관측치, 내부습도관측치, 총주정광량, 월별 비율을 살펴보았다.       
내부온도관측치가 15-35에 몰려있음을 확인할 수 있었고, 내부습도관측치난 25-90에 몰려있음을 확인할 수 있었다.    
총추정광량은 고르게 퍼져있었으며, 11월과 12월에는 자료가 없음을 알 수 있었다.     

![image](https://user-images.githubusercontent.com/72390138/214470651-dcdabf73-474b-4129-a4d1-f1189cc537f3.png)        
적색, 청색, 백색, 총추의 총추정광량의 비율을 살펴보았다.    
백색과 총추는 100에서, 적색가 청색은 0에서 성장률이 높음을 알 수 있었다.      

![image](https://user-images.githubusercontent.com/72390138/214470785-f0b1f41a-5ea5-4c64-bc04-f1152ebb1b35.png)
EC와 CO2의 냉방상태를 확인해보았을 때, EC 관측치가 클수록 냉방상태는 적었으며 반대로 작을수록 냉방상태는 높은 것을 확인할 수 있었다.      
 
#### 🔎 Modeling     
분포를 일정하게 만들기 위해 **RobustScaler**을 이용한 Scaling을 해주었다.     
**Tensorflow**, **Pytorch** 그리고 **LSTM**을 이용해 모델의 성능을 비교하였으며, **Tensorflow**가 가장 높은 성능을 띄었다.   

🍀 Tensorflow          
public score : 17.91     
private score : 17.53    

---
 
### 7️⃣ Whether to wear a mask     

📌 github : meji9086/5959-deeplearning-project 참고     
 
**마스크 착용/미착용 분류하기**     

#### 🔎 Modeling    
**Tensorflow**를 이용해 마스크 착용 여부를 분류하였다.    
**Resnet152V**, **VGG19** 그리고 **DenseNet121**를 이용하여 성능을 비교하였으며, **Resnet152V**이 가장 높은 성능을 띄었다.       

🍀 Resnet152V
![image](https://user-images.githubusercontent.com/72390138/214471581-16d70af0-582b-4900-8c8f-c313a3ecbbdd.png)     
![image](https://user-images.githubusercontent.com/72390138/214471589-bb6b13f3-a87d-4ba4-95fd-eea5be933038.png)    

⭐ 팀원들 사진으로 성능 평가해보기     
![image](https://user-images.githubusercontent.com/72390138/214471714-64d184ad-292d-4c24-a950-dd620ef41d18.png)

---   

### 8️⃣ Sentences type Classification    

📌 github : meji9086/5959-deeplearning-project 참고     

**문장 유형 분류하기**     

#### 📊 EDA      
![image](https://user-images.githubusercontent.com/72390138/214471857-1ca7e2f3-e3a1-4cdc-8036-3aefe596cbd1.png)     
각 label의 빈도수를 시각화하여 확인해본 결과 시제를 제외한 모든 label은 치우쳐진 데이터임을 확인하였다.   
이에 따른 해결책을 생각해야할 것이다.    

![image](https://user-images.githubusercontent.com/72390138/214471950-c2e874f7-0054-4abf-a8fe-96feb8b118a3.png)     
label을 하나로 통합하여 빈도수를 확인해본 결과, 각 클래스 사이에서 불균형이 일어날 수 있음을 알 수 있었다.    
 
#### 🔎 Modeling    
**Resampling**을 통한 label 비율 맞추어 주었다.           
**torch**를 이용하여 문장 유형을 예측하였으며, **BERT Model**이 가장 성능이 좋았음을 확인하였다.     

🍀 BERT Model Score : 0.72838      

---

### 🔟 olist corporate analysis

📌 github : meji9086/olist-corporate-analysis 참고       

---

## ✏ mid project     
### 3️⃣ Analysis of the cause of traffic accidents by violation of laws and regulations          

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
 
## ✏ final project     
### 9️⃣ brand review analysis    
