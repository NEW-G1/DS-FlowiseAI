# 🤖 Conversational Agent

### **주요내용**

### **✨💡✨ 채팅 관련 프롬프트를 활용하는 채팅 모델용 대화형 에이전트 Chatflow 생성**

- 채팅 관련 프롬프트를 활용하는 채팅 모델용 대화형 에이전트를 생성합니다.

<img src="./images/Conversational Agent/Conversational Agent.png" alt="API Agent OpenAI">


## ChatOpenAI API 및 Serp API설정

1. `OpenAI`의 `LLM Model`을 사용하가 위해 `ChatOpenAI`를 설정합니다.

2. `Serp API`를 통한 웹서치 Tool을 사용하기 위해 `Serp API Key`를 설정합니다.

<img src="./images/Conversational Agent/OpenAPI_SerpAPI.png">


## Tool 연결 및 Conversational Agent 생성

1. 앞서 생성한 웹서치를 위한 `Serp API`과  계산을 할 수 있는 `Calculator` Tool 을 `Converstional Agent`에 연결하여 `Agent`를 생성합니다.

2. 이전 대화를 기억하기 위한 `Buffer Memory`를 함께 연결합니다.

<img src="./images/Conversational Agent/Conversational Agent Memory.png">