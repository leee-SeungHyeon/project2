## 스마트 거버넌스를 위한 지역혁신 모델 개발

### PurPose
- 스마트 거버넌스 구현을 위한 지역혁신모델의 지능화 및 국내외 확산
- 정책의제 도출, 정책형성, 정책결정, 정책결정 등 정책 과정의 지능화 지원

### Role
- 스마트시티 뉴스 기사 웹 크롤링
- 토픽 모델링 기법 조사
- 스마트시티에 대한 차기 정책 의제 도출하기 위한 토픽 모델링 기법 비교 

### Process
<img src="https://user-images.githubusercontent.com/123627186/232267393-d28eb693-c9c0-46f2-892b-f057e53d1e00.png" width="300" height="350">

### Data
- 네이버 뉴스에서 2017년과 2021년에 ‘스마트 시티’ 키워드로 검색된 뉴스 데이터 크롤링

# Data Preprocessing
- Stopwords (ex:언론사 이름, 기자 이름 등)
- Remove Duplicate Articles
- Noun Extraction

### Method
- Selenium
- Beautifulsoup
- Mecab
- LDA(Latent Dirichlet Allocation)
- BERTopic

### Result
<img src="https://user-images.githubusercontent.com/123627186/232268351-d98a7e43-cd47-4839-93d5-180068862d02.png" width="550" height="400">

### Conclusion
- Mecab 형태소 분석기를 이용하여 불용어 사전을 구축하고 기사에서 필요하지 않은 단어를 제거하고 명사만 추출하여 LDA와 BERTopic 모델링을 진행하였음
- 각 모델별로 20개의 토픽을 도출하였음
- 2017년도에는 스마트시티 개발을 위한 키워드들이 많이 도출되었다면, 2021년도에는 스마트시티 발전을 위한 키워드들이 많이 도출되었음
- BERTopic이 LDA보다 좀 더 다양한 토픽들을 분류해낸것을 확인하였음
- 인재육성, 보안 등의 키워드를 통하여 중앙 정부 및 지방 정부에서 스마트시티를 위한 정책적 의사결정을 위한 근거자료로 활용될 수 있을것으로 생각됨
