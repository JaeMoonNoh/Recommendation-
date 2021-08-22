#### 0. Data Processing

#### colab 환경에서 Mecab을 사용하기 위한 설치 작업

1. bash 셸 명령어를 입력하여 설치

2. 환경변수 설정

3. mecab 설치

#### 1. preprocessing_data를 사용해서 데이터 초기 전처리
ㄱ-ㅎ, ㅏ-ㅣ, 가 - 힣 를 제거
'Unnamed: 0','id','author','day','platform' 컬럼은 사용하지 않으니 drop  
문장을 더 확실하게 만들기 위해서 title,genre,stroy를 합쳐서 사용후 story drop

#### 데이터 전처리 결과


#### 2. Mecab(), stopwords사용해서 더 상세히 분리

