# 🤖 Conversational Retrieval QA Chain

### **주요내용**

### **✨💡✨ Text파일을 사용한 검색 기반 대화형 Chain Chatflow 생성**

- Text파일을 Pinecone VectorDB에 로드한 후 Pinecone 검색 기반 대화형 챗봇을 생성합니다.

<img src="./images/Conversational Retrieval QA Chain/Conversational Retrieval QA Chain.png" alt="API Agent OpenAI">

## Text File 업로드 및 Pinecone에 Upsert

1. `Text File` Document Loader를 사용하여 Text 파일을 업로드 한 후 `Recursive Character Text Splitter`를 사용하여 텍스트를 분할합니다.

2. 분할한 텍스트를 `OpenAI Embeddings`과 `Pinecone Upsert Document`를 사용하여 `Pinecone`에 임베딩 한 후 Upsert합니다.

<img src="./images/Conversational Retrieval QA Chain/TextFIle_Pinecone_upload.png">


## Pinecone 연결 및 Conversational Retrieval QA Chain 생성

임베딩 및 데이터를 Upsert한 `Pinecone` VectorDB와 LLM Model을 사용하기 위한 `ChatOpenAI`를 `Conversational Retrieval QA Chain`에 연결하여 대화형 체인을 생성합니다.

<img src="./images/Conversational Retrieval QA Chain/ChatOpenAI_Pincone_Chain.png">