# API Agent OpenAI

**주요내용**

**🤖 OpenAI Cahin 및 OpenAI Function Agent를 사용하여 API를 호출하는 Chatflow 생성**

- `OpenAI Function Agent`와 `Chain`을 사용하여 호출할 API를 자동으로 결정하고 대화에서 URL 및 Body 요청 생성합니다.

<img src="./images/API Agent OpenAI.png" alt="API Agent OpenAI">


## Few Shot Prompt Template
1. `Few Shot Prompt Template`를 프롬프트 예제를 구축합니다.

2. `Prompt Template`를 사용하여 사용자가 입력한 단어의 반의어를 출력하는 템플릿을 생성합니다..

<img src="./images/Antonym Prompt Template.png">


## LLMChain 생성

앞서 생성한 `Few Shot Prompt Template`과  `ChatOpenAI`의 `Model`을 `LLMChain`에 연결합니다.

<img src="./images/Antonym LLMChain.png">


## Chatflow 실행

단어 입력 시 반의어를 출력하는 것을 확인할 수 있습니다.

<img src="./images/Antonym execute.png">