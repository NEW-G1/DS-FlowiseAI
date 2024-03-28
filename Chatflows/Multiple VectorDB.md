# Multiple VectorDB Chain

**주요내용**

# **✨💡✨ 여러개의 VectorDB를 기반으로 검색기를 생성하여 대화형 Agent Chatflow 생성**

- `Vectara`, `Pinecone` 등의 여러개의 VectorDB 기반 Retriever를 생성하여 대화형 Agent를 생성합니다.


<img src="./images/Multiple VectorDB/Multiple Vector DB.png" alt="API Agent OpenAI">


## VectaraDB Chain Tool 생성

1. `Pdf File` Document Loader를 사용하여 PDF 파일을 업로드 합니다. `CSV`, `text`등 다른 파일도 업로드 가능합니다.

    그 다음 `Recursive Character Text Splitter`를 사용하여 텍스트를 분할합니다.

2. 분할한 텍스트를 `Vectara`에 임베딩 한 후 `Retrieval QA Chain`와 `Chain Tool`을 사용하여 검색형 체인 및 Tool을 생성합니다.

<img src="./images/Multiple VectorDB/Multiple Vectara.png">


## PineconeDB Chain Tool 생성

1. `Text File` Document Loader를 사용하여 PDF 파일을 업로드 합니다. 그 다음 `Recursive Character Text Splitter`를 사용하여 텍스트를 분할합니다.

2. 분할한 텍스트를 `Pinecone`에 임베딩 한 후 `Retrieval QA Chain`와 `Chain Tool`을 사용하여 검색형 체인 및 Tool을 생성합니다.

<img src="./images/Multiple VectorDB/Multiple Pinecone.png">


## Multiple VectorDB Agent 생성

앞서 생성한 `Vectara Chain Tool`, `Pinecone Chain Tool`, LLM Model을 사용하기 위한 `ChatOpenAI`, `Buffer Memory`를 

`Conversational Agent`에 연결하여 `Agent`를 생성합니다.

<img src="./images/Multiple VectorDB/Multiple Vector DB_Agent.png">