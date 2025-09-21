# Zustand Practice App (Counter + Todo + User)

React와 Zustand를 이용해 상태 관리 개념을 연습하기 위한 미니 프로젝트 
초심자가 작성했지만 핵심 개념을 담아 복습과 포트폴리오 모두에 활용할 수 있도록 구성

---

## 프로젝트 개요
- **목표**: Redux보다 가벼운 Zustand로 전역 상태 관리 패턴을 익히기
- **구성**: `Counter`, `TodoList`, `User` 세 가지 상태 관리 예제를 구현
- **특징**: `persist`와 `devtools` 미들웨어를 활용해 상태 유지 및 디버깅 경험

---

## 사용 기술 스택
- React (CRA 기반)
- Zustand (상태 관리)
- Fetch API (샘플 사용자 데이터 요청)
- sessionStorage / localStorage (상태 저장)


---

## 주요 기능
### 1. Counter
- **증가** / **리셋** / **특정 값 설정** / **스토리지 초기화**
- Zustand `persist`로 localStorage 상태 유지
- `devtools`로 상태 변화 추적 가능

### 2. TodoList
- **추가**: 입력창에서 todo 작성 후 Add
- **완료**: 완료 시 체크 → 취소선 표시
- **삭제**: x 버튼으로 삭제
- Zustand `persist` + `sessionStorage`로 페이지 새로고침해도 유지

### 3. User
- **Fetch**: `jsonplaceholder` API에서 사용자 정보(이름·전화번호) 불러오기
- 상태 관리와 API 호출 패턴 연습

---

## 실행 방법
```bash
# 패키지 설치
npx create-react-ap
npm install zustand

# 개발 서버 실행
npm start
```