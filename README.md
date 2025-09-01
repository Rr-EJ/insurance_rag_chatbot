# 운전자 보험 약관 RAG 챗봇



# 팀 소개
<div align="center">
<img width="320" height="320" alt="Image" src="https://github.com/user-attachments/assets/34eb158f-413f-4f38-b1e4-6440ea6ae851" />


| 기현택     | 권도원     | 유의정     | 이소정     | 이준원     | 한승희    |
|:----------:|:----------:|:----------:|:----------:|:----------:|:----------:|
|[@mathplanet](https://github.com/mathplanet)|[@dowonk120](https://github.com/dowonk120)|[@ryu0ej](https://github.com/Rr-EJ)|[@leesojunghub](https://github.com/leesojunghub)|[@none-jun](https://github.com/none-jun)|[@seunghee-han](https://github.com/seunghee-han)|
| Project Manager | Prompt Engineer | Frontend Engineer | Dataset Manager | Evaluation Specialist | Prompt Engineer |

</div>
<br/>
<br/>
<br/>

# 기술 스택

| 항목    | 내용     |
| ---------- | ---------- |
| Language    | <img src="https://img.shields.io/badge/python-3776AB?style=for-the-badge&logo=python&logoColor=white">  <img src="https://img.shields.io/badge/sql-4479A1?style=for-the-badge&logo=sql&logoColor=white"> |
| Development    | <img src="https://img.shields.io/badge/Visual Studio Code-61DAFB?style=for-the-badge&logo=VisualStudioCode&logoColor=white"> |
| Embedding    | <img src="https://img.shields.io/badge/OpenAIEmbedding-181717?style=for-the-badge&logo=openai&logoColor=white">     |
| LLM Model    | <img src="https://img.shields.io/badge/chatgpt_4.1-3776AB?style=for-the-badge&logo=openai&logoColor=white">      |
| Collaboration Tool    | <img src="https://img.shields.io/badge/github-181717?style=for-the-badge&logo=github&logoColor=white"> <img src="https://img.shields.io/badge/Discord-02569B?style=for-the-badge&logo=Discord&logoColor=white">     |
|Framework|<img src="https://img.shields.io/badge/langchain-1C3C3C?style=for-the-badge&logo=openai&logoColor=white">  <img src="https://img.shields.io/badge/RAG-FFCA28?style=for-the-badge&logo=rag&logoColor=white"> <img src="https://img.shields.io/badge/streamlit-7952B3?style=for-the-badge&logo=streamlit&logoColor=white">|
| Vector DB    |<img src="https://img.shields.io/badge/pgvector-00599C?style=for-the-badge&logo=pgvector&logoColor=white"> <img src="https://img.shields.io/badge/psycopg2-3776AB?style=for-the-badge&logo=psycopg2&logoColor=white"> <img src="https://img.shields.io/badge/PostgreSQL-0769AD?style=for-the-badge&logo=postgresql&logoColor=white"> <img src="https://img.shields.io/badge/FAISS-E34F26?style=for-the-badge&logo=faiss&logoColor=white">   |
| API    | <img src="https://img.shields.io/badge/OpenAI API-181717?style=for-the-badge&logo=openai&logoColor=white">    |
|Evaulation|<img src="https://img.shields.io/badge/Ragas-F7DF1E?style=for-the-badge&logo=ragas&logoColor=white"> |


# 프로젝트 기간
2025년 8월 22일, 2025년 8월 25일 (2일)
<br/>
<br/>
<br/>	

# 프로젝트 개요

## 📕 프로젝트 발단

## 1. 프로젝트 배경
보험 약관은 해마다 더 복잡해지고 길어지고 있습니다. 일부 상품은 500~900페이지에 달하며, 전문 용어와 복잡한 조항으로 인해 소비자가 내용을 이해하기 어렵습니다.  
이로 인해 **필요한 정보를 신속하게 찾기 어렵고**, 잘못 이해하거나 중요한 내용을 놓칠 위험이 큽니다.

- 방대한 분량과 복잡한 구조로 **일반 소비자가 읽고 이해하기 어려움**  
- 필요한 조항을 찾기 위해 전체 문서를 탐색해야 하는 **비효율성**  
- 법률·보험 용어의 난해함으로 인한 **정보 접근성 저하**  

- 약관 분량 예시  
| 약관문서 | 페이지 수 |
|----------|-----------|
| DB 운전자보험 | 900 |
| KB Direct 장기 운전자보험 | 634 |
| 무배당 삼성화재 운전자보험 안전운전 파트너 플러스 | 522~528 |
| 한화 운전자상해보험 무배당 | 544 |



## ✅ 프로젝트 배경 및 목적
- **RAG(Retrieval-Augmented Generation)** 기반 챗봇으로 방대한 약관에서 **필요한 정보를 빠르고 정확하게 제공**  
- 사용자가 **자연어로 질문**하면, 약관 원문에서 관련 내용을 찾아 **간결하고 이해하기 쉽게 요약**  
- 소비자의 **정보 접근성 향상**과 **의사결정 지원**

## 주요 기능
- **자연어 질의응답**  
- **약관 검색 및 요약**  
- **다양한 보험사·상품 지원**  
- **전문 용어 해설**

## ❤️ 기대효과

* 가입자 만족도 및 신뢰도 향상
  *  필요한 정보를 쉽고 빠르게 얻을 수 있습니다. 정확한 출처까지 함께 제공되므로 답변의 신뢰도가 높아져 고객 만족도가 크게 향상 할 수 있습니다.
* 정보 비대칭성 완화
  *  보험사는 방대한 정보를 제공하지만, 사용자는 이를 모두 파악하기 어렵습니다. 챗봇은 이 정보 비대칭성을 해소합니다.
* 확장성 및 유지보수 용이
  *  새로운 보험 상품이 출시되거나 약관이 개정될 경우, 해당 문서만 벡터 데이터베이스에 추가하면 챗봇이 즉시 새로운 정보를 바탕으로 답변할 수 있어 유지보수가 간편합니다.
* 콜센터 업무 효율 증대
  *  다양한 상황에 대한 응대를 챗봇이 대신함으로써, 콜센터 직원들이 더 복잡하고 전문적인 상담에 집중할 수 있게 되어 업무 효율이 증대할 수 있습니다.


## 🛠️ 전체 플로우

<img width="1200" height="600" alt="Image" src="https://github.com/user-attachments/assets/efcbcc95-25f5-4b3d-9165-10e86ac5ed8a" />

<img width="1200" height="650" alt="Image" src="https://github.com/user-attachments/assets/9d7f1eaa-7249-417a-8ff9-375e1344fa8f" />

* 데이터 전처리
  * PDF -> PyPDFLoader로 로드 -> RecursiveCharacterTextSplitter 문서 청크
* 임베딩 및 저장
  * OpenAIEmbeddings를 사용 -> 벡터로 변환 -> 보험사별 collection_name을 지정 -> PGVector 사용 -> postgreSQL에 저장
* 다중 검색
  * EnsembleRetriever를 활용 -> 동시에 문서를 검색 -> 가장 관련성 높은 문서
* 질의응답
  * LLM의 컨텍스트로 전달 -> 답변을 생성 -> 출처를 제공


### Vector DB
| Collection    | Embedding     |
| ---------- | ---------- |
| <img width="600" height="300" alt="Image" src="https://github.com/user-attachments/assets/b77924a7-8c06-46e1-897d-e2baa56e0c69" /> | <img width="600" height="300" alt="Image" src="https://github.com/user-attachments/assets/6dc37fde-1434-450c-847e-9f1b7b1146cb" />  |

<br/>
<br/>

### Prompt

<img width="1058" height="877" alt="Image" src="https://github.com/user-attachments/assets/a0726b49-9072-4d6d-8eae-17097c40419e" />


<img width="1200" height="650" alt="Image" src="https://github.com/user-attachments/assets/34de3e8b-0936-4a46-bc78-561973e9aa61" />

|faithfulness|answer_relevancy|nv_context_relevance|
|-----|-----|-----|
|답변 충실도, 환각 방지|답변이 원래 질문에 얼마나 직접적으로 관련되어 있는지를 측정|검색한 문서들이 실제로 질문에 답변하는 데 얼마나 유용한 정보를 담고 있는지 측정|



## Streamlit
<img width="1916" height="888" alt="Image" src="https://github.com/user-attachments/assets/6ada762b-6be4-45eb-8a1a-1469bcee3b9a" />


### 연령별 예시

* 20대

<img width="1142" height="766" alt="Image" src="https://github.com/user-attachments/assets/2e041c33-f606-4f63-ad56-922587400db7" />

* 특정 나이

<img width="1130" height="774" alt="Image" src="https://github.com/user-attachments/assets/8b28d610-76e5-4741-ac4b-737b296c24c9" />


### 상황별 예시

* 무단횡단 보행자 사고
<img width="1156" height="692" alt="Image" src="https://github.com/user-attachments/assets/a6efe2bb-fd34-4f31-90dc-aaad292a4594" />
<img width="1146" height="714" alt="Image" src="https://github.com/user-attachments/assets/8ac5ec5c-fae2-4fec-918f-9e3e3b92d7d7" />

## 프로젝트 확장성

* 다양한 보험 상품으로의 적용 가능
  * 건강보험, 화재보험 등 다양한 약관을 반영하면 챗봇의 목적을 바꿀 수 있게 됩니다.
* 판례 데이터 반영
  * 파인 튜닝(Fine-Tuning)을 통한 판례 기반의 추론 강화
  * 법적 기반을 통한 방향성 확보
  * 챗봇이 더욱 풍부한 역할 가능

# 회고록

* 권도원

* 기현택 : 조용한 스타일의 팀장임에도 다들 너무 잘 해주셔서 감사합니다. 발표 준비를 하면서 RAG와 LLM에 대해 많은 것을 공부할 수 있었던 좋은 시간이었습니다.
  
* 유의정 : 임베딩과 데이터베이스 저장부터 RAG의 전체 코드를 직접 작성하며 구조와 흐름에 대한 이해를 깊게 할 수 있었습니다. 또한 팀원들과의 원활한 협력을 통해 프로젝트를 더욱 완성도 있게 마무리할 수 있었습니다.(ꔷ̥̑.̮ꔷ̥̑) 
  
* 이소정 : 이번 프로젝트에서는 데이터베이스부터 RAG 모델까지 직접 구현하며 문제를 해결하는 과정에서 많은 성장을 느낄 수 있었습니다. 또한 팀원들과 협력하며 서로의 아이디어를 보태 더 완성도 높은 결과를 만들어낼 수 있었습니다.
  
* 이준원 : RAG 프로젝트를 통해 전체적인 구조와 흐름을 이해할 수 있었고, 특히 Retriever와 Embedding의 중요성을 깨달었던 프로젝트였습니다! 또한 적극적이고 열정적인 팀원들과 중심을 잘 잡아주신 팀장님 덕분에 프로젝트를 수월하게 마무리할 수 있었습니다:)
  
* 한승희 : 원했던 주제이기도 하고 직접 prompt 엔지니어링을 해볼 수 있어서 뜻깊은 시간이였습니다. 모두들 수고하셨습니다 ﻿~❥


