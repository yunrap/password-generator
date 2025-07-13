# Password Generator

npx 명령어를 통해 사용자가 원하는 길이의 비밀번호를 생성하는 패키지를 만들것입니다. (npm deep dive 참고)

## 특징

- Node.js 기반
- 사용자가 원하는 길이의 비밀번호를 생성하는 기능 제공
- 비밀번호 생성 문자열 배열에서 Math.random()을 사용해 사용자가 입력한 길이만큼 문자열을 무작위로 선택하여 반환

## 지원 환경

- Node.js 18 이상

## 개발 환경 및 프로젝트 구조

- 번들러: 비트와 롤업을 사용하여 모듈 번들링
- 트랜스파일: 바벨
- 타입: 타입스크립트로 작성
- 단위테스트 : Vitest 사용
- 모듈시스템 : ESM (ECMAScript Modules) 사용

## 의존성포함

- `chalk`: 콘솔 출력에 색상을 추가하기 위한 라이브러리
- `core-js`: Node.js 18버전까지 안정적으로 동작하는 폴리필 라이브러리
- `meow`: meow는 사용자 친화적인 CLI(Command Line Interface) 애플리케이션을 만들기 위한 라이브러리로, 명령어 파싱과 옵션 관리를 쉽게 해줍니다.

## CI/CD

- lefthook을 사용하여 Git pre-commit 훅 설정
- GitHub Actions를 사용하여 CI/CD 파이프라인 구축
- changesets를 자동으로 생성하여 배포 시 변경 사항을 기록
