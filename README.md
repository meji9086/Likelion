# ๐ฆ Likelion ๐ฆ
**Likelion AI SCHOOL7** ๊ตญ๋น ๊ต์ก์์์ ํ๋ก์ ํธ (๋ณธ์ธ ์ฝ๋)

|์๋ฒ|์ ๋ชฉ|๊ฐ์|ํ์ดํ๋ผ์ธ|๋ฐฐํฌ|             
|:-:|:-------:|:------:|:---:|:------:|             
|1|์นํฐ ์์ ๋ถ์|BeautifulSoup๊ณผ Requests๋ฅผ ์ด์ฉํด ์นํฐ ์์๋ฅผ ์กฐ์ฌํ๋ค.|weboon_rank.ipynb|                            
|2|์ดํผ ์ฌ์  ๋ถ์|์ง์ญ๋ณ ์ดํผ ์ฌ์ ์ ๋ํด ์๊ฐํํ๊ณ  ๋ถ์ํ๋ค.|reason_of_divorce.ipynb|          
|3|๊ตํต์ฌ๊ณ  ์์ธ ๋ถ์|๋ฒ๊ท์๋ฐ์ ๋ํ ๊ตํต์ฌ๊ณ  ์์ธ์ ์๊ฐํํ๊ณ  ๋ถ์ํ๋ค.|traffic_accident.ipynb|<img src="https://img.shields.io/badge/streamlit-FF4B4B?style=flat-square&logo=streamlit&logoColor=A8B9CC"/>     
|4|์ ์ฃผ๋ ๋๋ก ๊ตํต๋ ์์ธก|์ ์ฃผ๋ ๋๋ก ๊ตํต ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ง๊ณ  EDA ๋ฐ Modeling์ ํ๋ค.|traffic_predict_in_Jeju.ipynb|      
|5|๋ธํธ๋ถ ๊ฐ๊ฒฉ ์์ธก|๋ธํธ๋ถ์ ์ ๋ณด ๋ฐ์ดํฐ๋ฅผ ๊ฐ์ง๊ณ  EDA ๋ฐ Modeling์ ํตํด ๊ฐ๊ฒฉ์ ์์ธกํ๋ค.|Laptop_price_predict.ipynb|

## โ mini project      
### 1๏ธโฃ Webtoon Rank        

**BeautifulSoup๊ณผ Requests๋ฅผ ์ด์ฉํ ์นํฐ์ ์์๋ฅผ ๊ฐ์ ธ์ค๊ธฐ**      

![image](https://user-images.githubusercontent.com/72390138/196094124-b7ba960b-8b29-4732-8d1d-6f0e9c52460c.png)

---

### 2๏ธโฃ Reason of divorce by region by year

**์ง์ญ๋ณ ์ฐ๋๋ณ ์ดํผ ์ฌ์ ์ ๋ํด ๋ถ์ํ๊ธฐ**                 

![image](https://user-images.githubusercontent.com/72390138/196094866-25ca9a0e-7332-47c6-a8c3-799c7ddec738.png)
![image](https://user-images.githubusercontent.com/72390138/196095208-b38309f4-e758-4f33-94da-c4165504affd.png)
 
์ดํผ ์ฌ์ ์๋ ์ฑ๊ฒฉ ์ฐจ์ด๊ฐ ๊ฐ์ฅ ํฐ ์์ธ์ด ๋๋ค๊ณ  ๋ณผ ์ ์๋ค.             
๋ํ, ์ง์ญ์ผ๋ก๋ ๊ฒฝ๊ธฐ๋, ์์ธํน๋ณ์๊ฐ ๊ฐ์ฅ ๋ง์ผ๋ ์ด๋ ์ธ๊ตฌ๋ฐ๋์ง์ญ์ผ๋ก ์ธํ ์ฐจ์ด๋ผ๊ณ  ๋ณผ ์ ์๋ค.

---

### 3๏ธโฃ Road Traffic Forecasts in Jeju Island         

๐ github : meji9086/Jeju-Traffic-Forecast ์ฐธ๊ณ           

**์ ์ฃผ๋ ๋๋ก ๊ตํต๋ ์์ธกํ๊ธฐ**         
#### EDA             

![image](https://user-images.githubusercontent.com/72390138/201580818-0244acd5-e286-4ed5-832d-e418e5c14607.png)            
- base_date : 2022๋ 7์ ๊ธฐ์ค์ผ๋ก ๊ตํต๋ ์ฆ๊ฐํ์๋ค. ์ด๋ ์ฝ๋ก๋ ์ ์ข ์ดํ ์ฒ์ ๊ฑฐ๋ฆฌ๋๊ธฐ๊ฐ ํ๋ฆฐ ์ฌ๋ฆ ํด๊ฐ๋ก ์ธํ ๊ธ์ฆ์ด๋ผ๊ณ  ๋ณผ ์ ์๋ค.              
- base_hour : 00์-05์,18์-24์์ ๊ตํต๋ ๊ฐ์ํ์๊ณ , 05์-18์ ๊ตํต๋ ์ฆ๊ฐํ์๋ค(์ฐจ์ด๊ฐ ํผ).       
- day_of_week : ๊ธ์์ผ์ ๊ตํต๋ ์ฆ๊ฐํ์๊ณ , ์ฃผ๋ง์ ๊ตํต๋ ๊ฐ์ํ์๋ค(ํฐ์ฐจ์ด ์์).       
- road_name : '-'์ผ๋ก ๊ธฐ๋ก๋ null๊ฐ์ด ์กด์ฌํ๋ค.         

![image](https://user-images.githubusercontent.com/72390138/201581387-15fb2df7-c880-4392-bd4b-8df391d18397.png)          
- year : ๋๋ ทํ ์ฐจ์ด ์๋ค.          
- month : 7์ ๊ตํต๋ ๊ธ์ฆ๊ฐํ์๋ค. ์ด๋ ์ฌ๋ฆ ํด๊ฐ๋ฅผ ์์ธ์ผ๋ก ๋ณผ ์ ์๋ค.        
- day : ๋๋ ทํ ์ฐจ์ด ์๋ค.            
- ์๋ณ ์ฐจ์ด๊ฐ ์ ์ผ ๋๋ ทํ ๊ฒ์ ๋ณผ ์ ์๋ค.          

#### Modeling           
**LightGBM**์ ์ด์ฉํด ๊ตํต๋ ์์ธกํ์๋ค.                
<img src="https://user-images.githubusercontent.com/72390138/201582425-1f6c99e5-a940-4b44-9863-3e2568d934ef.png" width="380" height="480">    
**GridSearchCV**๋ฅผ ์ด์ฉํ ์ต์ ์ ํ์ดํผ ํ๋ผ๋ฏธํฐ : {'learning_rate': 0.05, 'max_depth': 5, 'min_child_samples': 5, 'num_leaves': 20}            
๐ test data MAE ์ ์ : 5.77352     

---

### 4๏ธโฃ Prediction of Laptop price

๐ github : meji9086/5nly-code-repository ์ฐธ๊ณ 

**๋ธํธ๋ถ ๊ฐ๊ฒฉ ์์ธกํ๊ธฐ**
#### EDA
   
<img src="https://user-images.githubusercontent.com/72390138/203262255-0d0271e7-9ec6-4821-9374-cb4a3f21f4f2.png" weight="550" height="450">         
Notebook์ ์ข๋ฅ๊ฐ ์๋ฑํ๊ฒ ๋์ ๊ฒ์ ํ์ธํ  ์ ์๋ค.    
์ด๋, ๋ค๊ณ ๋ค๋ ์ ์๋ ํธ์์ฑ์ผ๋ก ์ธํด ๊ตฌ๋งค์จ์ด ๋์ ์์ฐ๋ฅ ๋ ๋์ ๊ฒ์ด๋ผ๊ณ  ์ถ์ธกํ  ์ ์๋ค.       


<img src="https://user-images.githubusercontent.com/72390138/203263872-972f5506-cea6-42c7-a9d4-51532bb8749b.png">        
์ ์กฐ์์ Dell, Venovom, HP์ ์ ํ๋ค์ด ์๋ฑํ๊ฒ ๋ง์ ๊ฒ์ ํ์ธํ  ์ ์๋ค.     



#### Modeling       
**RandomForestRegressor**๋ฅผ ์ด์ฉํด ๋ธํธ๋ถ ๊ฐ๊ฒฉ์ ์์ธกํ์๋ค.   
<img src="https://user-images.githubusercontent.com/72390138/203267744-ff0cd8ac-0508-4c54-bf62-476a704473bc.png" weight="500" height="400">         
feature ๊ฐ ์ค์๋๋ **1์ RAM, 2์ Peso(๋ฌด๊ฒ)** ์์ผ๋ก ๋์ ๊ฒ์ ์ ์ ์๋ค.       
๐ test data RMSE : 402       


---

## โ mid project
### Analysis of the cause of traffic accidents by violation of laws and regulations          

๐ github : meji9086/Traffic-Accident-Data-Analysis ์ฐธ๊ณ 

**๋ฒ๊ท์๋ฐ๋ณ ๊ตํต์ฌ๊ณ  ์์ธ ๋ถ์**                     

![image](https://user-images.githubusercontent.com/72390138/197454540-5b545e1c-e2a6-4af8-a251-371c09cb7b48.png)          

๊ตํต์ฌ๊ณ ์ ์์ธ์ผ๋ก๋ ์ ํธ์๋ฐ, ์์ ๊ฑฐ๋ฆฌ๋ฏธํ๋ณด ๊ทธ๋ฆฌ๊ณ  ๊ต์ฐจ๋ก์ดํ๋ฐฉ๋ฒ์๋ฐ์ผ๋ก ๋ณผ ์ ์๋ค.            

![image](https://user-images.githubusercontent.com/72390138/197454577-9c6bce18-a97c-49ba-a9b1-1be68e7e6948.png)            

ํ์ง๋ง, ์ฌ๋ง์๋ ๊ณผ์์ผ๋ก ๋ง์ด ๋ฐ์ํ๋ค๋ ๊ฒ์ ์ ์ ์๋ค.            


**โ ํด๊ฒฐ๋ฐฉ์ ์ ์**            
1. ์ ํธ์๋ฐ์ ๋ํ ๋ฒ์ ๊ฐํ ๋๋ ๋ฒ์น๊ธ์ ์ฆ๊ฐ์ํจ๋ค.           
2. ๊ณผ์ ํ  ์ ์๋ ๊ตฌ๊ฐ์ CCTV ์ถ๊ฐ์ค์น ๋ฐ ๊ณผ์ ๋ฒ์น๊ธ ์ฆ๊ฐ์ํจ๋ค.          

---
