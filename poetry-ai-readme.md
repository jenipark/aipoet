# 인공지능 시인 (AI Poet)

LangChain과 OpenAI를 활용한 한국어 시 생성 웹 애플리케이션입니다.

## 프로젝트 소개

사용자가 입력한 주제에 맞는 아름다운 한국어 시를 자동으로 생성해주는 Streamlit 기반 웹 애플리케이션입니다. OpenAI의 GPT-4o-mini 모델을 사용하여 창의적이고 감성적인 시를 작성합니다.

## 주요 기능

- 🎨 사용자 정의 주제로 시 생성
- 🔐 안전한 API 키 관리 (사이드바에서 입력)
- 🚀 실시간 시 생성
- 💬 직관적인 사용자 인터페이스

## 기술 스택

- **Frontend**: Streamlit
- **LLM Framework**: LangChain
- **AI Model**: OpenAI GPT-4o-mini
- **Language**: Python 3.11
- **Development Environment**: Dev Container (VS Code)

## 설치 방법

### 1. 저장소 클론

```bash
git clone <repository-url>
cd <project-directory>
```

### 2. 의존성 설치

```bash
pip install -r requirements.txt
```

### 3. 애플리케이션 실행

```bash
streamlit run app.py
```

## Dev Container 사용하기

이 프로젝트는 VS Code Dev Container를 지원합니다.

1. VS Code에서 프로젝트 폴더 열기
2. Command Palette (Ctrl+Shift+P / Cmd+Shift+P) 열기
3. "Dev Containers: Reopen in Container" 선택
4. 컨테이너가 자동으로 빌드되고 애플리케이션이 실행됩니다

포트 8501에서 자동으로 애플리케이션이 시작됩니다.

## 사용 방법

1. **API 키 입력**
   - 사이드바에서 OpenAI API 키를 입력하세요
   - API 키는 [OpenAI Platform](https://platform.openai.com/api-keys)에서 발급받을 수 있습니다

2. **주제 입력**
   - 메인 화면의 입력창에 시의 주제를 입력하세요
   - 예: "봄날의 햇살", "가을의 낙엽", "별이 빛나는 밤"

3. **시 생성**
   - "시 작성 요청하기" 버튼을 클릭하세요
   - AI가 입력한 주제로 아름다운 시를 생성합니다

## 주요 의존성

- `langchain==1.0.5` - LLM 애플리케이션 프레임워크
- `langchain-openai==1.0.2` - OpenAI 통합
- `openai==2.7.2` - OpenAI API 클라이언트
- `streamlit` - 웹 애플리케이션 프레임워크

전체 의존성 목록은 `requirements.txt`를 참조하세요.

## 프로젝트 구조

```
.
├── .devcontainer/
│   └── devcontainer.json    # Dev Container 설정
├── app.py                    # 메인 애플리케이션
├── requirements.txt          # Python 의존성
└── README.md                 # 프로젝트 문서
```

## 환경 설정

### OpenAI API 키 발급

1. [OpenAI 웹사이트](https://platform.openai.com/)에 가입
2. API Keys 페이지로 이동
3. "Create new secret key" 클릭
4. 생성된 키를 안전하게 보관

### 시스템 요구사항

- Python 3.11 이상
- 인터넷 연결 (OpenAI API 통신용)
- OpenAI API 키

## 보안 주의사항

⚠️ **중요**: API 키는 절대 코드나 공개 저장소에 직접 포함하지 마세요!

- API 키는 애플리케이션 실행 시 사이드바에서 입력하세요
- 환경 변수나 `.env` 파일을 사용하여 관리할 수 있습니다
- 공개 저장소에 푸시하기 전에 API 키가 포함되지 않았는지 확인하세요

## 문제 해결

### API 키 오류
- API 키가 올바른지 확인하세요 (`sk-`로 시작)
- OpenAI 계정에 크레딧이 있는지 확인하세요

### 의존성 오류
```bash
pip install --upgrade pip
pip install -r requirements.txt
```

### 포트 충돌
```bash
streamlit run app.py --server.port 8502
```

## 라이선스

이 프로젝트는 교육 목적으로 만들어졌습니다.

## 기여하기

기여를 환영합니다! Pull Request를 보내주세요.

## 문의

프로젝트에 대한 질문이나 제안이 있으시면 Issue를 생성해주세요.