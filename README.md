# Gemini Text Generation API - TouchDesigner Component

## 개요
Gemini Text Generation API는 TouchDesigner에서 Google의 Gemini AI 모델을 사용하여 텍스트 생성을 수행할 수 있는 컴포넌트입니다. 이 컴포넌트를 통해 대화형 AI 기능을 TouchDesigner 프로젝트에 쉽게 통합할 수 있습니다.

## 기능

- **Gemini AI 모델 지원**: Google의 Gemini AI 모델을 사용한 텍스트 생성
- **시스템 지시사항 설정**: AI의 동작을 정의하는 시스템 프롬프트 설정
- **대화형 프롬프트**: 사용자 입력을 통한 텍스트 생성
- **채팅 히스토리**: 대화 기록 관리 및 초기화
- **구조화된 출력**: JSON 형태의 구조화된 응답 생성 (향후 업데이트 예정)
- **함수 호출**: 개발중 (현재 비활성화)


## 시작하기

### 1. 파일 구성
- `GeminiTextGenerationAPI.tox`: 메인 컴포넌트
- `GeminiTextGenerationAPI-Example.toe`: 사용 예제 파일

### 2. 설정 방법
1. TouchDesigner에서 `GeminiTextGenerationAPI.tox` 파일을 열거나 프로젝트에 추가
2. **Settings** 섹션에서 Google Gemini API 키 입력
3. **Message** 섹션에서 시스템 지시사항과 프롬프트 설정
4. **Run** 섹션에서 **Active** 토글을 **On**으로 설정

### 3. API 키 발급
Google AI Studio에서 Gemini API 키를 발급받아야 합니다:
1. [Google AI Studio](https://aistudio.google.com/) 방문
2. API 키 생성
3. 생성된 키를 컴포넌트의 **APIKey** 필드에 입력


## 주요 섹션

### Message
- **System Instructions**: AI의 기본 동작을 정의하는 시스템 프롬프트
- **prompt**: 사용자가 입력하는 메시지

### Settings
- **APIKey**: Google Gemini API 키
- **Model**: 사용할 Gemini 모델 (기본: gemini-2.0-flash-lite)

### Tools
- **Structured output**: 구조화된 출력 기능
- **Function calling**: 함수 호출 기능 (향후 업데이트 예정)

### Chat History
- **Activate History**: 채팅 히스토리 활성화/비활성화
- **Reset Pulse**: 채팅 히스토리 초기화
- **Clear Response Message Pulse**: 응답 메시지 초기화

### Run
- **Active**: 컴포넌트 활성화/비활성화
- **Request Pulse**: API 요청 실행
- **Stop Pulse**: 실행 중인 요청 중지
- **Clear Log Pulse**: 로그 초기화

## 예제 사용법

1. 예제 파일 `GeminiTextGenerationAPI-Example.toe`를 열어 기본 설정 확인
2. API 키를 입력하고 프롬프트 설정
3. **Send** 버튼을 클릭하여 텍스트 생성 실행
4. 생성된 응답 확인

## 주의사항

- Google Gemini API 사용을 위해서는 유효한 API 키가 필요합니다
- 네트워크 연결이 필요합니다

## 작성자

**doodlefingers (Jeonghyo)** - [Instagram](https://www.instagram.com/doodlefingers/)

## 버전

**v0.1.0**

## 라이선스

MIT

---

# Gemini Text Generation API - TouchDesigner Component

## Overview

Gemini Text Generation API is a TouchDesigner component that enables text generation using Google's Gemini AI model. This component allows you to easily integrate conversational AI functionality into your TouchDesigner projects.

## Features

- **Gemini AI Model Support**: Text generation using Google's Gemini AI model
- **System Instructions**: Configure system prompts to define AI behavior
- **Interactive Prompts**: Text generation through user input
- **Chat History**: Conversation history management and reset
- **Structured Output**: JSON structured response generation (planned for future updates)
- **Function Calling**: Under development (currently disabled)

## Getting Started

### 1. File Structure
- `GeminiTextGenerationAPI.tox`: Main component
- `GeminiTextGenerationAPI-Example.toe`: Usage example file

### 2. Setup Instructions
1. Open or add `GeminiTextGenerationAPI.tox` file to your TouchDesigner project
2. Enter your Google Gemini API key in the **Settings** section
3. Configure system instructions and prompts in the **Message** section
4. Set the **Active** toggle to **On** in the **Run** section

### 3. API Key Setup
You need to obtain a Gemini API key from Google AI Studio:
1. Visit [Google AI Studio](https://aistudio.google.com/)
2. Generate an API key
3. Enter the generated key in the **APIKey** field of the component

## Main Sections

### Message
- **System Instructions**: System prompt that defines the basic behavior of the AI
- **prompt**: Message entered by the user

### Settings
- **APIKey**: Google Gemini API key
- **Model**: Gemini model to use (default: gemini-2.0-flash-lite)

### Tools
- **Structured output**: Structured output functionality
- **Function calling**: Function calling functionality (planned for future updates)

### Chat History
- **Activate History**: Enable/disable chat history
- **Reset Pulse**: Reset chat history
- **Clear Response Message Pulse**: Clear response messages

### Run
- **Active**: Enable/disable component
- **Request Pulse**: Execute API request
- **Stop Pulse**: Stop running request
- **Clear Log Pulse**: Clear logs

## Example Usage

1. Open the example file `GeminiTextGenerationAPI-Example.toe` to check basic settings
2. Enter API key and configure prompts
3. Click the **Send** button to execute text generation
4. Check the generated response

## Important Notes

- A valid API key is required to use Google Gemini API
- Network connection is required

## Author

**doodlefingers (Jeonghyo)** - [Instagram](https://www.instagram.com/doodlefingers/)

## Version

**v0.1.0**

## License

MIT