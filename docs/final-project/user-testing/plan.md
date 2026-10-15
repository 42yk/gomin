# 고민일기 사용자 테스트 계획

## 목적

배포한 고민일기의 이용 흐름과 AI 결과를 점검한다. 대화에서 요약·그림일기·컬렉션으로 이어지는 과정에서 사용자가 겪는 불편을 확인한다.

## 진행 방식

실사용자 5명이 배포 환경을 이용했고 피드백은 대면으로 수집했다. 서비스 주소는 [www.gomin.today](https://www.gomin.today)다. 참여자는 기획 타겟과 다른 사용자들이다.

사전에 배포한 질문지나 개인별 수행 과제는 확인된 자료가 없어 기재하지 않았다. 아래 항목은 Jira에 정의된 기능 검증 기준이며, 모든 참여자가 같은 순서로 수행했다는 의미는 아니다.

## 기능 검증 항목

| 단계 | 확인할 내용 | 근거 |
| --- | --- | --- |
| 대화 시작 | 입력창에 바로 작성할 수 있고 메시지 전송 결과가 표시되는지 | [GOMIN-117](https://younkim.atlassian.net/browse/GOMIN-117) |
| 대화 | 앞선 내용과 연결된 응답을 받고 사용자가 원하는 시점에 마무리할 수 있는지 | [GOMIN-71](https://younkim.atlassian.net/browse/GOMIN-71) |
| 요약 | 지금의 마음·주요 고민·감정 태그를 확인하고 확정하거나 대화를 재개할 수 있는지 | [GOMIN-71](https://younkim.atlassian.net/browse/GOMIN-71) |
| 그림 생성 | 확정 요약으로 그림을 만들고 다른 그림을 요청할 수 있는지 | [GOMIN-115](https://younkim.atlassian.net/browse/GOMIN-115) |
| 저장·조회 | 완성 결과를 저장하고 목록·상세에서 같은 이미지와 요약을 확인할 수 있는지 | [GOMIN-74](https://younkim.atlassian.net/browse/GOMIN-74), [GOMIN-115](https://younkim.atlassian.net/browse/GOMIN-115) |
| 상세 화면 | PC에서 그림과 요약을 함께 읽고 모달을 닫을 수 있는지 | [GOMIN-118](https://younkim.atlassian.net/browse/GOMIN-118) |
| 예외 상황 | 생성·업로드·저장·조회 실패와 계정 전환을 구분해 처리하는지 | [GOMIN-115](https://younkim.atlassian.net/browse/GOMIN-115) |

## 피드백 정리 기준

의견은 입력·화면 구성·로딩 안내·대화 품질·이미지 품질로 나눴다. 개인별 응답 자료가 없는 의견은 전체 피드백으로 정리하며, 참가자나 응답 빈도를 임의로 붙이지 않는다. 개선 내용은 코드·PR·커밋으로 연결한다.

[테스트 결과](results.md) · [피드백과 개선](improvements.md) · [프로젝트 구조](../README.md)
