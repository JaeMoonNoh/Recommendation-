### 0. Data Processing

#### colab 환경에서 Mecab을 사용하기 위한 설치 작업

##### 0 - 0. bash 셸 명령어를 입력하여 설치

![bashshell명령어설치](https://user-images.githubusercontent.com/62277037/130345115-9803e17d-e5d8-4ba5-ba18-d924fecdbcd1.PNG)


##### 0 - 1. 환경변수 설정

![환경변수 설정](https://user-images.githubusercontent.com/62277037/130345116-e443bac1-64ff-484a-95cf-f7ffec28f954.PNG)

##### 0 - 2. mecab 설치

![mecab설치](https://user-images.githubusercontent.com/62277037/130345117-5443d41e-7b3f-4de5-9370-6f7d5977e56d.PNG)


### 1. preprocessing_data를 사용해서 데이터 초기 전처리

##### 1 - 0. 전처리 전

![전처리 전](https://user-images.githubusercontent.com/62277037/130345118-17049d43-382d-4b75-bc81-4d29b549dcae.PNG)

##### 1 - 1. ㄱ-ㅎ, ㅏ-ㅣ, 가 - 힣 를 제거

##### 1 - 2. 'Unnamed: 0','id','author','day','platform' 컬럼은 사용하지 않으니 drop  

##### 1 - 3. 문장을 더 확실하게 만들기 위해서 title,genre,stroy를 합쳐서 사용후 story drop

![초기전처리후](https://user-images.githubusercontent.com/62277037/130345119-13ea2f14-2408-4489-8bcf-c24168490bda.PNG)


### 2. 데이터 전처리 결과

##### 2 - 0. Mecab(), stopwords사용해서 더 상세히 분리

![메컵후](https://user-images.githubusercontent.com/62277037/130345120-c0b472f0-4cd4-4fe2-a853-bf3d4559f2dd.PNG)

##### 2 - 1. 불용어를 사용해서 세세하게 분리를 하려고 했지만 더 추가를 해야될 것 같다.

!!! stopwords = ['의','가','이','은','들','는','좀','잘','걍','과','도','를','으로','자','에','와','한','하다'] !!!
더 추가해야됩니다.

