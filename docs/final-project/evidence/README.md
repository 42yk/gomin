# 고민일기 화면·실행 증빙

## 서비스

- [고민일기 배포 서비스](https://www.gomin.today)
- [GitHub 저장소](https://github.com/gomin-diary/gomin)

## 기능·실행 근거

| 내용 | 근거 |
| --- | --- |
| 회원가입·로그인 | [회원가입 구현](../../engineering/signup.md), [로그인·세션](../../engineering/login-auth.md) |
| 대화·요약·확정 | [GOMIN-71](https://younkim.atlassian.net/browse/GOMIN-71), [대화 구현](../../engineering/talk-mvp.md) |
| 그림일기 생성·저장 | [그림일기 구현](../../engineering/diary-mvp.md), [그림일기 API](../../../backend/app/api/routes/diary.py) |
| 컬렉션 목록·상세 | [컬렉션 화면](../../frontend/collection-ui.md) |
| 모의·DB·브라우저 검증 | [기존 QA 기록](../../engineering/talk-mvp-qa.md) |
| 배포 환경 전체 흐름 확인 | [검증·배포 결과](../verification.md) |
| 사용자 테스트 | [테스트 결과](../user-testing/results.md) |
| 피드백 반영 | [개선 내역과 수정 이력](../user-testing/improvements.md) |

## 캡처·시연 자료

이 폴더에 등록된 캡처·시연 파일은 없다. 기존 QA 문서에는 모의 API 화면 캡처의 저장 위치로 Git에서 제외한 `.dev/talk-qa/`가 명시되어 있으나, 현재 작업 공간에서 해당 이미지 파일을 확인하지 못해 증빙으로 연결하지 않았다.

캡처를 등록할 때는 실제 파일과 설명을 함께 연결하고 실제 서비스 화면인지 모의 API 화면인지 구분한다. 사용자 원문·계정 정보·인증정보가 포함된 자료는 공개 문서에 넣지 않는다.

[프로젝트 구조](../README.md)
