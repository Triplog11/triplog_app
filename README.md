# triplog_app
2026 관광데이터 활용 공모전 트립로그 프로젝트 
: 여행 기록 및 방문 인증 기반 게이미피케이션 앱 트립로그

협업 규칙

GitHub 협업 규칙은 CONTRIBUTING.md를 참고합니다.

기본 원칙은 다음과 같습니다.

main, develop 브랜치 직접 push 금지
모든 작업은 Issue 생성 후 진행
작업 브랜치는 feature/이슈번호-작업명 형식 사용
작업 완료 후 develop 브랜치로 Pull Request 생성
최소 1명 이상 리뷰 후 merge
API Key, 인증키, .env 파일은 절대 커밋 금지
문서
상세 메뉴트리: docs/planning/menu-tree.md
기능명세서: docs/planning/feature-spec.md
WBS: docs/planning/wbs.md
데이터 스키마: docs/data/data-schema.md
ERD: docs/data/erd.md
GitHub 협업 규칙: docs/rules/github-rules.md
주의사항

API Key, 인증키, .env 파일은 절대 GitHub에 올리지 않습니다.
환경변수는 .env.example에 키 이름만 작성하고, 실제 값은 별도로 공유합니다.
