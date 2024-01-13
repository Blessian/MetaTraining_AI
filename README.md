<!-- 어떤 연구분야에서 어떻게 성과를 냈는지, 내 역량의 범위는 어떻게 되는지에 집중하여 간략하게 작성하는 것이 중요합니다. -->
<!-- 회사는 여러분들이 회사에서 진행 중인 또는 진행할 프로젝트에 기여를 할 수 있는 역량을 가진 사람인가를 궁금해합니다. 
     때문에 여러분들의 연구나 프로젝트를 상위 레벨에서 쉽게 설명하고 어떤 역량을 키웠으며 내가 가진 역량으로 어떤 산업과 프로젝트에 적용할 수 있는지를 구체적으로 보여주는 것이 중요합니다. -->
<!-- AI기술에 대한 경험기술서 (직접 활용해 본 AI기술들에 대한 구축 경험과 시행착오가 담긴 기술서)
     예시)
          어떠한 목표를 달성하기 위하여, AI 기술 중 Voice Conversion을 활용 하기로 하였음
          이 과정에서 어떠한 모델을 선정 하였고 Raw데이터를 이러한 방식으로 준비하여 파인튜닝을 하였음. 
          그 과정에서 이러한 시행착오를 겪었음. 결과 모델들 중 이러한 기준으로 최종 모델을 선정 함. -->
<!-- -->



# 📢 프로젝트 소개
### 주제 선정 배경
<div align="center">
     
![스크린샷 2023-09-30 181502](https://github.com/Blessian/MetaTraining_AI/assets/74029539/27090ed3-66e1-4a2c-87a3-bf91ed9e3b3a)
![스크린샷 2023-09-30 181551](https://github.com/Blessian/MetaTraining_AI/assets/74029539/5aedba1d-0c58-4662-8f12-bd19fbb5a06a)

</div>

- 공부법의 정석으로 여겨져 왔던 일명 "엉덩이 학습법"의 비효율이 다른 나라 학생들과의 성취도 평가 비교에서 드러나고 있다.
- 따라서 그저 오랜 시간을 투자하는 방법이 아닌 실제 자신이 잘 학습하고 있는지 자문할 수 있는 능력인 "메타인지"의 함양이 대두되었다.
- 본 프로젝트는 글쓰기를 통해 효과적으로 메타인지를 향상시킬 수 있도록 AI챗봇의 도움을 받을 수 있는 글쓰기 플랫폼을 서비스하는 것을 목표로 한다.

### 주요 기능
- 챗봇
     - 의도 분류: 챗봇에 입력된 문자열에서 사용자의 의도를 파악하여 자유대화와 링크 제공 중 적절한 서비스를 제공
     - 링크 제공: 사용자가 주제에 대한 배경지식 보충을 요구했을 때 적절한 자료를 검색하여 링크를 제공
     - 자유 대화: 사용자와 자유대화를 주고받지만, 글을 대신 적성해주지 않도록 제한
- 주제
     - 카테고리 분류: 사용자가 입력한 주제의 카테고리를 서비스에서 제공하는 카테고리로 자동 분류
     - 주제 추천 (최신 이슈 반영): 글의 주제를 자동 생성하여 추천 (주제 추천에 최신 이슈가 반영)
- 교정
     - 제목 추천: 사용자가 작성한 글의 제목을 자동 생성
     - 어색한 문장 찾기: 작성된 내용 중 어색한 문장을 찾아 수정을 제안

### 사용 기술
[![Python Badge](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff&style=for-the-badge)](https://www.python.org/)
[![Openai](https://img.shields.io/badge/openai_gpt4-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Google Bard Badge](https://img.shields.io/badge/Google%20Bard-886FBF?logo=googlebard&logoColor=fff&style=for-the-badge)](https://bard.google.com/chat?hl=ko)
[![Langchain](https://img.shields.io/badge/%F0%9F%A6%9C%F0%9F%94%97langchain-fff?style=for-the-badge)](https://www.langchain.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com/ko/)
[![BeautifulSoup](https://img.shields.io/badge/BeautifulSoup-fff?style=for-the-badge)](https://www.crummy.com/software/BeautifulSoup/)
![SQLite Badge](https://img.shields.io/badge/SQLite-003B57?logo=sqlite&logoColor=fff&style=for-the-badge)

| Tech | Purpose |
| --- | --- |
| OpenAI GPT-4 | 프롬프트 튜닝을 통해 다양한 역할을 수행할 수 있으며, GPT-3.5 Turbo에 비하여 신뢰할 수 있는 결과물을 보여줌 |
| Google Bard | 최신 이슈 검색에 활용 |
| Langchain | LLM을 쉽게 제어할 수 있도록 돕는 프레임워크 |
| FastAPI | LLM API를 호출할 수 있도록 API서버를 구성 |
| BeautifulSoup | 검색 결과를 크롤링하기 위해 사용 |
| SQLite | 자체 모델을 훈련시킬 목적으로 데이터 수집 |


<br>

# 👥 팀원 소개 및 역할
### [김나래]
- 역할: 
  - 카테고리 분류: 사용자가 입력한 주제의 카테고리를 서비스에서 제공하는 카테고리로 자동 분류
  - 자유대화: 사용자와 자유대화를 주고받지만, 글을 대신 적성해주지 않도록 제한
  - 주제 추천에 최신 이슈 반영: 주제 추천에 최신 이슈가 반영될 수 있도록 함

### [원예찬]
- 역할:
  - 메타인지 향상을 위한 질문 생성: 사용자가 자신이 작성하는 글의 내용을 잘 파악하고 있는지 되물을 수 있도록 질문한다
  - 제목 추천: 사용자가 작성한 글의 제목을 자동 생성한다
  - 어색한 문장 찾기: 작성된 내용 중 어색한 문장을 찾아 수정은 제안한다

### [이승현] << Me!
- 역할:
  - 주제 추천: 글의 주제를 자동 생성하여 추천한다
  - 의도 분류: 챗봇에 입력된 문자열에서 사용자의 의도를 파악하여 자유대화와 링크 제공 중 적절한 서비스를 제공한다
  - 링크 제공: 사용자가 주제에 대한 배경지식 보충을 요구했을 때 적절한 자료를 검색하여 링크를 제공한다
  - Langchain을 이용한 "대화 내역 기억" 기능 구현
  - 자체 모델 학습 데이터 수집을 위한 DB구축


<br>

# 📅 프로젝트 진행과정
### 일정관리
![스크린샷 2023-09-30 190808](https://github.com/Blessian/MetaTraining_AI/assets/74029539/141dc622-264f-413e-88c7-362147467ad2)
- [Notion을 통해 회의록 작성](https://www.notion.so/AI-2324eb03fe8e47d797e7b3c72fe89e47?pvs=4)

![스크린샷 2023-09-30 190919](https://github.com/Blessian/MetaTraining_AI/assets/74029539/d18a5f9b-409a-4e6f-8e43-240b09ee9651)
- [간트차트 작성](https://docs.google.com/spreadsheets/d/1lLzEKg-K05hdMZLEdZCs5oLfDxMPo0d_rpSOa-5KKJ0/edit#gid=1737882262)

<br>

### 진행과정 (시행착오)
#### 프롬프트 작성 및 결과 확인
![스크린샷 2023-10-03 005646](https://github.com/Blessian/MetaTraining_AI/assets/74029539/2f03ea2d-d81c-46cf-8307-0a7d39e1b981)
- 기능별 프롬프트를 작성하고 의도한 결과가 출력되는지 확인했다.
- GPT-4의 경우 출력 양식(ex. Json 형식, 리스트 형식 등)을 예시로 제공하면 출력 양식에 맞춰 출력되는 것을 확인

<br>

#### API를 통해 주고받을 자료형, 양식 확정
![스크린샷 2023-10-03 105307](https://github.com/Blessian/MetaTraining_AI/assets/74029539/79b931a1-b6d1-4889-9225-c0d4eab94881)
- API 호출 밥법 정의
- 변수 자료형 정의
- 변수명 정의

<br>

#### BeautifulSoup을 이용한 링크 제공 구현
![스크린샷 2023-10-03 011225](https://github.com/Blessian/MetaTraining_AI/assets/74029539/42fba675-2383-4ca6-9d26-2a8cebedc357)
- GPT-4에게 링크를 제공해달라는 요청을 했을 때, 언뜻 보면 요청을 잘 수행하는 것 처럼 보이지만, GPT-4는 그럴싸하게 보이는 링크를 "생성"할 뿐 실제로 확인해보면 존재하지 않는 페이지(404 ERROR)이다. (할루시네이션)
- 사용자가 어떤 정보를 필요로 할지 예상할 수 없고, 또한 제공되는 정보가 정확해야 글쓰기에 도움을 줄 수 있기 때문에 인터넷 검색을 통한 링크 제공이 필수였고 이 이슈를 해결해야 했다.
- 마이크로소프트의 Bing Chat이 인터넷 검색을 통해 정확한 링크를 제공하는 방식을 관찰하여 링크를 직접 생성하는 대신 적절한 검색어를 생성하여 검색 결과를 크롤링하는 방식으로 구현했다.
     ![화면 캡처 2023-09-13 203249](https://github.com/Blessian/MetaTraining_AI/assets/74029539/41174af8-43e1-4684-9bd7-b9f36aee12da)
     - 링크를 수집하던 중 한글로 이루어진 링크들이 수집 과정에서 변형되어 기능을 상실하는 이슈가 있었다.
     - urllib의 unquote_plus()함수를 통해 url을 재가공하여 해결했다.

<br>

#### API 서버 구축
- 구현된 기능들의 API를 호출하여 사용할 수 있도록 FastAPI를 통해 API 서버를 구축했다
- API를 호출하여 사용하는 서버팀의 편의를 위해 API의 호출과 반환값의 양식을 수정하는 과정을 거쳤다.

<br>

#### DB 구축
- 서비스를 테스트하는 과정에서 주요한 이슈 중 하나는 서비스 비용에 돤한 것이었다.
- OpenAI의 API를 사용하여 서비스하는 방식은 사용자가 글 하나를 완성하는데 300 ~ 400원 정도가 부담될 것으로 예상했고, 서비스를 확대하면 이 비용은 상당한 부담이 될 것으로 보였다.
- 자체적인 LLM을 구축하여 서비스해야 하는 것이 장기적으로 유리하다는 판단을 했고, 당장 프로젝트에는 반영할 수 없더라도 데이터 수집에 대한 전략이 필요하다는데 의견이 모아졌다.
- 프롬프트, 사용자 입력, 대화 내역, 출력 등을 수집하고 DB에 저장하도록 했다.

<br>

# 📊  결과
### 프로젝트 시연 영상
[![스크린샷 2023-09-30 202728](http://img.youtube.com/vi/PF1W-fF4AwQ/0.jpg)](https://youtu.be/PF1W-fF4AwQ?si=dT6OQE_0Vbe-UHCc)

### 프로젝트에서 얻은 교훈과 인사이트
- OpenAI의 API를 사용하며 프롬프트 작성 요령을 습득하는 기회였고, LLM을 이용한 서비스에서 겪을 수 있는 할루시네이션, 지연시간, 비용 등에 관해 생각해 볼 수 있었다.
- API 사용에 따른 비용 부담:
  - 시연 영상을 녹화하며 사용자가 한 편의 글을 작성하는데 약 300~400원의 API비용이 부담되는 것으로 나타났다
  - 사용자가 늘어날 경우 적잖은 비용 부담이 예상되기 때문에 수익모델을 고민해야 했고, 자체모델 구축 필요성을 느꼈다
- 길어지는 프롬프트와 늘어나는 지연시간
  - 의도된 결과물을 도출하기 위해 프롬프트에 여러가지 요구사항과 제한사항을 반영해야 했고, 그에 따라 사용자가 결과를 받기 위해 기다려야 하는 시간이 늘어났다

<br>

# 🔗 참고 자료
### 사용한 논문 및 자료
