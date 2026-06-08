# triplog_app
2026 관광데이터 활용 공모전 트립로그 프로젝트 
: 여행 기록 및 방문 인증 기반 게이미피케이션 앱 트립로그

# 트립로그 Triplog

2026 관광데이터 활용 공모전 출품 프로젝트입니다.

트립로그는 사용자가 지역, 랜드마크, 이벤트를 탐색하고 실제 방문 후 GPS 인증, 사진 인증, 평점/만족도 입력, 리뷰 작성을 통해 여행 기록을 남기는 앱입니다.

방문 인증 기록을 바탕으로 배지 획득, 레벨 성장, 활동 히스토리 등 게이미피케이션 요소를 제공합니다.

## 서비스 개요

트립로그는 단순한 여행 정보 탐색 앱이 아니라, 사용자의 실제 방문 경험을 기록하고 보상하는 여행 기록 서비스입니다.

사용자는 한국관광공사 Tour API 기반의 지역, 랜드마크, 이벤트 정보를 탐색할 수 있으며, 특정 장소를 방문한 뒤 인증을 완료하면 자신의 여행 기록이 쌓입니다.

## 주요 기능

### MVP 기능

* 소셜 로그인
* 약관 동의
* 닉네임 설정
* 홈 화면
* 전국 지도 조회
* 특정 지역 지도 조회
* 지역 상세 조회
* 랜드마크 상세 조회
* 이벤트 상세 조회
* 찜한 지역, 랜드마크, 이벤트 관리
* GPS 기반 방문 인증
* 사진 인증
* 평점, 만족도 입력
* 리뷰 작성
* 인증 결과 확인
* 배지 획득
* 전체 배지 목록 확인
* 배지 상세 확인
* 레벨 정보 확인
* 활동 히스토리 확인
* 인증 상세 확인
* 마이페이지
* 데이터 없음 처리
* 시스템 오류 처리

### 2차 기능

* 커뮤니티 피드
* 피드 상세
* 댓글
* 좋아요
* 전체 사용자 리그
* 지역별 리그
* 알림 센터
* 알림 설정
* 앱 이용 가이드

## 데이터 활용

본 프로젝트는 한국관광공사 OpenAPI를 활용합니다.

활용 예정 데이터는 다음과 같습니다.

* 지역 정보
* 관광지, 랜드마크 정보
* 이벤트 정보
* 주소 정보
* 좌표 정보
* 이미지 정보
* 콘텐츠 상세 정보

Tour API 원천 데이터는 가능한 원본값을 유지하고, 트립로그 자체 서비스 데이터는 별도 테이블로 분리하여 관리합니다.

예시:

* Tour API 원천 데이터: contentId, title, address, latitude, longitude, imageUrl
* 트립로그 자체 데이터: 방문 인증 기록, 찜 여부, 리뷰, 배지, 레벨, 활동 히스토리

## 프로젝트 구조

```text
triplog-app/
  .github/
    ISSUE_TEMPLATE/
      feature_request.md
      bug_report.md
    PULL_REQUEST_TEMPLATE.md

  docs/
    planning/
      menu-tree.md
      feature-spec.md
      wbs.md
    data/
      data-schema.md
      erd.md
    rules/
      github-rules.md

  frontend/
    README.md

  backend/
    README.md

  README.md
  CONTRIBUTING.md
  .gitignore
```

## 기술 스택

### Frontend

* React Native
* 추후 확정

### Backend

* 추후 확정

### Database

* 추후 확정

### External API

* 한국관광공사 OpenAPI

## 협업 규칙

GitHub 협업 규칙은 `CONTRIBUTING.md`를 참고합니다.

기본 원칙은 다음과 같습니다.

* `main`, `develop` 브랜치 직접 push 금지
* 모든 작업은 Issue 생성 후 진행
* 작업 브랜치는 `feature/이슈번호-작업명` 형식 사용
* 작업 완료 후 `develop` 브랜치로 Pull Request 생성
* 최소 1명 이상 리뷰 후 merge
* API Key, 인증키, `.env` 파일은 절대 커밋 금지

## 문서

* 상세 메뉴트리: `docs/planning/menu-tree.md`
* 기능명세서: `docs/planning/feature-spec.md`
* WBS: `docs/planning/wbs.md`
* 데이터 스키마: `docs/data/data-schema.md`
* ERD: `docs/data/erd.md`
* GitHub 협업 규칙: `docs/rules/github-rules.md`

## 주의사항

> API Key, 인증키, `.env` 파일은 절대 GitHub에 올리지 않습니다.
> 환경변수는 `.env.example`에 키 이름만 작성하고, 실제 값은 별도로 공유합니다.
