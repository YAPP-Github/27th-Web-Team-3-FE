# PRD 001 - Init: FSD/Conventions/ReactQuery/Templates

- Issue: #1
- Branch: `chore/1-init-conventions`
- Owner: TBD

## 목표

- FSD 스캐폴드, 컨벤션 문서, React Query 도입, 이슈/PR 템플릿 정비

## 배경

- 초기 구조/규칙 부재로 코드 위치·프로세스 일관성 확보 필요

## 범위

- `.cursorrules`, `docs/guides/*`, `README.md`
- FSD 폴더 생성(기존 코드 이동 없음)
- React Query + query-key-factory 설치 및 Provider 연결
- GitHub Issue/PR 템플릿 추가

## 비범위

- 기존 코드 FSD 리팩토링, 신규 기능 개발

## 완료 기준(AC)

- 컨벤션 문서 5종(FSD/TYPES/REACT_QUERY/COMMITS/PROCESS) 추가 및 README 링크
- `.cursorrules`에 규칙+few-shot 예시 반영
- FSD 레이어 폴더가 Git에 트래킹됨
- React Query Provider 동작(앱 부트 시 QueryClient 적용)
- 한글 Issue/PR 템플릿 동작

## 산출물

- 문서 파일: `docs/guides/*`, `docs/tasks/001-init.md`
- 코드/설정: `.cursorrules`, `src/app/providers/*`, `src/main.tsx`, `.github/*`, `README.md`

## 리스크/롤백

- 설치/빌드 실패 시 패키지 추가분 제거 후 이전 상태로 롤백
- Provider 적용 오류 시 `main.tsx`의 래핑만 되돌리면 영향 최소
