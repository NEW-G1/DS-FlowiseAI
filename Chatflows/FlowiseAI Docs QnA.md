# 문서 기반 QnA 챗봇(Docs QnA)

**주요내용**

- 🤖 문서 기반으로 대화형 QnA를 생성하는 Chatflow 생성

<img src="./images/Docs Qna.png", height="100x", width="100px">

문서 기반으로 대화형 QnA를 생성하는 Chatflow입니다.
PDF, Docs, Github등 다양한 문서를 사용할 수 있습니다.

## PDF File
`PDF File Document Loader`를 사용하여 PDF파일을 로드합니다.

<img src="./images/Docs Qna.png", height="100x", width="100px">

## Markdown Text Splitter

마크다운 기준으로 문서를 분할합니다.

<img src="./images/Docs Qna.png", height="100x", width="100px">

## OpenAI Embeddings / In-Memory Vector Store

`OpenAI`를 사용하여 분할된 문서를 Vector Store에 임베딩 처리합니다.

<img src="./images/Docs Qna.png", height="100x", width="100px">

## ChatOpenAI

`ChatOpenAI`의 LLM Model을 사용하기 위해 발급받은 OpenAI API Key를 설정한 후 Conversational Retrieval QA Chain 연결합니다.

<img src="./images/Docs Qna.png", height="100x", width="100px">

## Conversational Retrieval QA Chain
`Conversational Retrieval QA Chain`를 사용하여 대화형 체인을 생성합니다.

<img src="./images/Docs Qna.png", height="100x", width="100px">

## Chatflow Execute

업로드한 문서와 관련된 질문을 하고 그와 관련된 답변을 확인합니다.

<img src="./images/answer.png", height="100x", width="100px">