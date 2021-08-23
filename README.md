# Recommendation-

### Word2Vec

#### Word2Vec : 단어의 의미를 벡터화 하는 과정
###### 벡터화를 시키면 연산이 가능한데 벡터간 유사도를 반영해 연산을 진행할 수 있기 때문입니다.

벡터화 하는 과정중에서는 One-hot-encoding이 존재하는데 이것은 Sparse vector(희소행렬)이기 때문에 각 단어간의  
유사도를 표현할 수 없습니다. 유사도를 표현하기 위해서는 단어의 의미를 다차원 공간에 벡터화 해야합니다.

word2vec은 분산표현(Dirstributed representation)입니다.
 - 분산표현으로 단어의 유사도를 벡터화 하는 워드 임베딩에 속합니다.
 - 저차원을 가지므로 밀집벡터를 갖습니다.
 - 분포가설이라는 가정하에 만들어진 표현방법입니다.(비슷한 위치에서 등장하는 단어는 비슷한 의미를 갖는다.)


Word2Vec은 두가지 방식이 존재합니다.

1. 주변에 있는 단어들을 가지고, 중간에 있는 단어를 예측 -> CBOW(Continous Bag of Words)
2. 중간에 있는 단어를 가지고 주변에 있는 단어를 예측 -> Skip-gram


#### [CBOW : Continous Bag of Words]

주변에 있는 단어들을 가지고, 중간에 있는 단어를 예측
 - 중심단어를 예측하기 위해 앞,뒤로 몇개의 단어를 볼지 결정(window)
 - Sliding Window로 주변과 중심단어를 옮겨가며 Data Set을 만듦


#### [Skip-gram]

중심에 있는 단어를 가지고, 주변에 있는 단어를 예측


-Word2Vec에 대한 설명  

### Doc2Vec

Word2Vec의 확장해서 사용

-Doc2Vec에 대한 설명  

### Naver Webtoon crawling

- 제목, 작가, 스토리, 장르 등을 크롤링하기
- Doc2Vec에 필요한 열만 남기기

### Naver Webtoon Recommendation

-사용된 라이브러리 정리  
-개선점

### Data Processing

-데이터 처리 어떻게 했는지

### Etc.

-tokenize  
-etc...
