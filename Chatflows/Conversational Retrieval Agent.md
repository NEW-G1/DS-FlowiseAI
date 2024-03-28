# Conversational Retrieval Agent

**주요내용**

**🤖 대화 중 벡터 검색과 이전 대화를 기반으로 한 질문에 답변하는 데 최적화된 에이전트 Chatflow 생성**

- 대화 중 벡터 검색과 이전 대화를 기반으로 한 질문에 답변하는 데 최적화된 에이전트를 생성합니다.

<img src="./images/Conversational Retrieval Agent/Conversational Retrieval Agent.png" alt="API Agent OpenAI">

## Pinecone VectorDB 로드 및 Tool 생성

1. `Pinecone Load Existing Index`에서 Pinecone API Key 설정 후 `Pincecone Index`에 사용할 인덱스를 설정합니다.

2. 설정한 `Pinecone`을 `OpenAI Embeddings` 사용하여 임베딩 후 `Retirever Tool`을 사용하여 검색기 Tool을 생성합니다.

<img src="./images/Conversational Retrieval Agent/Pinecone Tool.png">


## Tool 연결 및 Conversational Retrieval Agent 생성

1. 앞서 생성한 `Retirever Tool`과 LLM Model을 사용하기 위한 `ChatOpenAI`를 `Conversational Retrieval Agent`에 연결하여 `Agent`를 생성합니다.

2. 이전 대화를 기억하기 위한 `Buffer Memory`를 함께 연결합니다.

<img src="./images/Conversational Retrieval Agent/Conversational Retrieval Agent Memory.png">