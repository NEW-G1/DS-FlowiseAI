# API Agent OpenAI

**주요내용**

**🤖 OpenAI Cahin 및 OpenAI Function Agent를 사용하여 API를 호출하는 Chatflow 생성**

- `OpenAI Function Agent`와 `Chain`을 사용하여 호출할 API를 자동으로 결정하고 대화에서 URL 및 Body 요청 생성합니다.

<img src="./images/API Agent OpenAI.png" alt="API Agent OpenAI">


## OpenAI Chain 및 Tool 생성

1. `OpenAI Chain`를 사용하여 `Yaml`링크를 통해 API를 호출하는 Chain을 생성합니다. 예시로 만화 정보가 있는 링크를 사용하였습니다.

2. `Chain Tool`을 사용하여 호출한 API를 통해 관련된 질문에 답변하는 Tool을 생성합니다.

<img src="./images/API Agent OpenAI OpenAIChain.png">


## OpenAI Function Agent

앞서 생성한 API를 호출하는 `Chain Tool`과  `ChatOpenAI`의 `Model`을 `OpenAI Function Agent`에 연결하여 `Agent`를 생성합니다.

<img src="./images/API Agent OpenAI Agent.png">

## API Agent OpenAI Chatflow 실행

사용자가 질문했을 때 만화 정보가 있는 링크 API를 호출하여 답변하는 것을 확인할 수 있습니다

<img src="./images/API Agent OpenAI execute.png">