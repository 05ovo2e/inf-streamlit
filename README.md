# inf-streamlit

소득세법 관련 질문에 답변하는 RAG 기반 AI 챗봇

## Tech Stack

| Category | Technology |
|---|---|
| Language | Python |
| Frontend | Streamlit |
| LLM | OpenAI GPT-4o |
| Embedding | OpenAI text-embedding-3-large |
| Vector Database | Pinecone |
| Framework | LangChain |
| Environment | pyenv, python-dotenv |

## Project Structure

```text
inf-streamlit/
├── chat.py          # Streamlit 채팅 인터페이스
├── llm.py           # LLM 및 RAG 체인 구성
├── config.py        # Few-shot 예시 및 설정
├── .env             # API 키 및 환경 변수
├── .gitignore
├── .python-version
└── README.md
```

## Notes

- Pinecone에 소득세법 문서가 사전에 저장되어 있어야 합니다.
- API 키는 `.env` 파일로 관리하며 GitHub에 업로드하지 않습니다.
- 실제 답변의 정확성은 검색된 문서와 모델의 해석에 따라 달라질 수 있습니다.
