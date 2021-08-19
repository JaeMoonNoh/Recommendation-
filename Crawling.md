# Crawling description


# 1. from selenium import webdriver
python에서 웹 크롤링을 하기 위한 도구로 selenium을 사용해 크롤링을 진행  
selenium을 사용하기위해서 pip로 selenium을 설치하고 브라우저에 맞는 driver설치  
![pipinstall](https://user-images.githubusercontent.com/62277037/130061077-5c4dbce2-8a21-4dd5-9c62-aa8f336df138.PNG)  

### Crome driver를 설치하는 방법 

## Crome 버전확인
#### 방법
chrome://settings/help 에 들어가서 확인


![크롬버전](https://user-images.githubusercontent.com/62277037/130061068-52f51618-4990-42b5-bfd3-4812d904bdfa.PNG)

## Crome 버전에 맞는 driver설치  
#### https://chromedriver.chromium.org/downloads  


![크롬_버전_release](https://user-images.githubusercontent.com/62277037/130061070-d10bdd6b-12a6-422d-9892-357a2e2c24b5.PNG)  


## Os에 맞는 버전 설치  


![버전설치](https://user-images.githubusercontent.com/62277037/130061073-0298b31b-4e30-44a7-99d2-ad2cfa2039c6.PNG)

## Crome Driver 경로 입력  
-driver = webdriver.Chrome('본인 경로')  
-driver.get('웹사이트주소')  


![드라이버경로설정](https://user-images.githubusercontent.com/62277037/130061075-688826ec-29df-4e7c-837b-913d003c3049.PNG)  


#### 진행이 잘 안될 시에는  
#### 1. '본인경로' 앞에 r'본인경로'  
#### 2. \대신 /사용  
#### 3. \ 대신 \\ 사용하는 경로 지정하는 방법이 있습니다.  


# 2. 네이버 웹툰 사이트 데이터 요청하기  


#### data = request.get('네이버웹툰사이트').text : text tag부분을 제외하고 text부분만을 추출한 후에
#### soup = BeautifulSoup(data,'html.parser') : html.parser를 통해서 html부분만을 파싱해줍니다.  


![html_](https://user-images.githubusercontent.com/62277037/130057480-e82524bf-fd74-4171-9fbd-b84a8787748f.PNG)


# 3. 제목(Title) 부분 데이터 받기
#### title = soup.find_all('a',{'class':'title'}) 
#### a 테그에 class title부분이 제목부분이기 때문에 이 부분만을 찾아서 title에 저장을 해줍니다. 
![타이틀만뽑아오기](https://user-images.githubusercontent.com/62277037/130057085-f9d0ce0c-a5a2-4b48-8549-b18a892bba02.PNG)


# 4. 제목(Title) 데이터 받은 결과
![타이틀_뽑은_결과](https://user-images.githubusercontent.com/62277037/130057511-e8a006ae-5cb1-4e73-a695-ac3437371d69.PNG)


# 5. 제목의 길이 바탕으로 데이터 추출하기
#### 요일 부분
day = soup.find_all('ul', {'class':'category_tab'} 부분에 요일이 들어가 있습니다.  
('li', {'class':'on'}) 부분에서 예를 들어 월요일 전체를 가져오지 않고 앞자리 한글자만 가져옵니다. 그래도 구분이 가능하기 때문에  


![네이버웹툰크롤링 페이지클릭하면서데이터수집](https://user-images.githubusercontent.com/62277037/130057512-0e40754e-08c1-482a-b818-cecf59085676.PNG)


#### 장르, 줄거리, 작가 부분  
작가 부분 : 2 테그 안에 class : wrt_nm 부분에 작가  
장르 부분 : span 부분 class : genre 부분에 장르  
줄거리 부분 : p 테그 부분 줄거리  


![네이버웹툰크롤링 줄거리,장르](https://user-images.githubusercontent.com/62277037/130057516-7a14a23c-8226-4dc5-8159-1b8713a28ce2.PNG)


# 6. 결과
![결과](https://user-images.githubusercontent.com/62277037/130059389-84a3f6a2-6aae-44b7-acd8-e666ba71cde5.PNG)
