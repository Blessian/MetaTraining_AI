# 📢 프로젝트 소개
### 프로젝트 목표
#### 주제 선정 배경
![스크린샷 2023-09-30 181502](https://github.com/Blessian/MetaTraining_AI/assets/74029539/27090ed3-66e1-4a2c-87a3-bf91ed9e3b3a)

![스크린샷 2023-09-30 181551](https://github.com/Blessian/MetaTraining_AI/assets/74029539/5aedba1d-0c58-4662-8f12-bd19fbb5a06a)

- 공부법의 정석으로 여겨져 왔던 일명 "엉덩이 학습법"의 비효율이 다른 나라 학생들과의 성취도 평가 비교에서 드러나고 있다.
- 따라서 그저 오랜 시간을 투자하는 방법이 아닌 실제 자신이 잘 학습하고 있는지 자문할 수 있는 능력인 "메타인지"의 함양이 대두되었다.
- 본 프로젝트는 메타인지 향상법 중 하나인 글쓰기를 위한 플랫폼을 서비스하여 메타인지를 효율적으로 높일 수 있도록 돕는다

# 📚 사용 기술

[![Python Badge](https://img.shields.io/badge/Python-3776AB?logo=python&logoColor=fff&style=for-the-badge)](https://www.python.org/)
[![Openai](https://img.shields.io/badge/openai-412991?style=for-the-badge&logo=openai&logoColor=white)](https://openai.com/)
[![Google Bard Badge](https://img.shields.io/badge/Google%20Bard-886FBF?logo=googlebard&logoColor=fff&style=for-the-badge)](https://bard.google.com/chat?hl=ko)
[![Langchain](https://img.shields.io/badge/%F0%9F%A6%9C%F0%9F%94%97langchain-fff?style=for-the-badge)](https://www.langchain.com/)
[![FastAPI](https://img.shields.io/badge/FastAPI-005571?style=for-the-badge&logo=fastapi)](https://fastapi.tiangolo.com/ko/)

### OpenAI GPT-4 API
- 프롬프트 튜닝을 통해 다양한 역할을 수행할 수 있으며, GPT-3.5 Turbo에 비하여 신뢰할 수 있는 결과물을 보여준다.
### Google Bard
- 최신 이슈 검색에 활용
### Langchain
- LLM을 쉽게 제어할 수 있도록 돕는 프레임워크이다.
### FastAPI
- LLM API 를 호출할 수 있도록 API서버를 구성하는데 사용했다.

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

# 📅 프로젝트 진행과정
### 일정관리
![스크린샷 2023-09-30 190808](https://github.com/Blessian/MetaTraining_AI/assets/74029539/141dc622-264f-413e-88c7-362147467ad2)
- [Notion을 통해 회의록 작성](https://www.notion.so/AI-2324eb03fe8e47d797e7b3c72fe89e47?pvs=4)

![스크린샷 2023-09-30 190919](https://github.com/Blessian/MetaTraining_AI/assets/74029539/d18a5f9b-409a-4e6f-8e43-240b09ee9651)
- [간트차트 작성](https://docs.google.com/spreadsheets/d/1lLzEKg-K05hdMZLEdZCs5oLfDxMPo0d_rpSOa-5KKJ0/edit#gid=1737882262)
### 진행과정과 시행착오
- OpenAI API Playground에서 프롬프트 작성 및 테스트
  ![스크린샷 2023-09-30 211320](https://github.com/Blessian/MetaTraining_AI/assets/74029539/2c19f790-772f-49b7-8ad9-978ddb3cca16)

- 최근 들려오는 소식에는 ChatGPT가 인터넷에 연결되어 검색된 정보와 링크를 제공할 것이라고 하지만, 프로젝트 진행 당시에는 GPT-4 API는 인터넷에 직접 연결되어 있지 않았음
  - 사용자의 요구사항을 해결할 수 있는 검색어를 생성하도록 하고 BeautifulSoup을 이용하여 검색과 크롤링으로 링크 수집 후 제공
- 주제 추천에 최신 이슈를 반영하기 위한 방법을 모색하였으나 각 주제에 대한 최신 이슈를 골고루 반영하는 것에 여려움을 겪음
  - 구글의 바드가 검색엔진에 연결되어 있다는 것을 알게되어 각 분야의 최신 이슈를 얻는데 바드를 이용함

# 📊  결과
### 프로젝트 시연 영상
[![스크린샷 2023-09-30 202728](http://img.youtube.com/vi/PF1W-fF4AwQ/0.jpg)](https://youtu.be/PF1W-fF4AwQ?si=dT6OQE_0Vbe-UHCc)

### 프로젝트에서 얻은 교훈과 인사이트
- API 사용에 따른 비용 부담:
  - 시연 영상을 녹화하며 사용자가 한 편의 글을 작성하는데 약 300~400원의 API비용이 부담된다
  - 사용자가 늘어날 경우 적잖은 비용 부담이 예상되기 때문에 수익모델을 고민해야 했고, 자체모델 구축 필요성을 느꼈다
- 길어지는 프롬프트와 늘어나는 지연시간
  - 의도된 결과물을 도출하기 위해 프롬프트에 여러가지 요구사항과 제한사항을 반영해야 했고, 그에 따라 사용자가 결과를 받기 위해 기다려야 하는 시간이 늘어났다

# 📝 향후 계획
### 자기평가
프로젝트에서 본인이 수행한 역할과 기술 습득 정도에 대한 자기평가. 예를 들어, "데이터 전처리와 모델 구현을 담당했고, PyTorch와 음성 처리 기술에 대한 실력이 향상되었다."
### 향후 계획
AI 기술에 대한 추가 학습 계획이나 심화 프로젝트에 대한 기획 소개. 예를 들어, "자연어 처리 분야에서 더 깊은 지식을 쌓고, 실세계 문제에 적용할 수 있는 프로젝트를 계획 중이다."

# 🔗 참고 자료
### 사용한 논문 및 자료
프로젝트 진행에 참고한 논문, 레퍼런스, 온라인 자료 등 명시. 예를 들어, "DeepSpeech 논문 및 관련 논문들을 참고하여 모델을 구현하고 학습함."
### 🔗 프로젝트 관련 코드 링크
프로젝트에 사용된 코드 저장소 링크 (GitHub 등). 예를 들어, "프로젝트 코드는 GitHub 저장소에서 확인할 수 있습니다: [링크]"
