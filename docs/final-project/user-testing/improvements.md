# 고민일기 사용자 피드백과 개선 결과

## 확인한 개선 내역

사용자 의견과 코드·수정 이력을 연결해 반영 내용을 정리했다. 개선의 효과를 측정한 결과와는 구분한다.

| 의견 | 변경 전의 불편 | 반영 내용 | 근거 |
| --- | --- | --- | --- |
| FB-01 | 입력을 시작하려면 입력창을 선택해야 하고 초록색 박스가 눈에 띈다. | 입력창에 자동 초점을 적용하고 포커스 테두리·입력 영역 스타일을 정리했다. | [PR #49](https://github.com/gomin-diary/gomin/pull/49), [커밋 b036d47](https://github.com/gomin-diary/gomin/commit/b036d47) |
| FB-02 | 컬렉션 상세에서 그림과 요약을 함께 읽기 어렵다. | PC에서 왼쪽 그림·오른쪽 요약을 하나의 모달로 묶고 이미지 비율·본문 스크롤을 유지했다. | [커밋 a0ab402](https://github.com/gomin-diary/gomin/commit/a0ab402), [PR #50](https://github.com/gomin-diary/gomin/pull/50) |
| FB-05 | 대화가 늦게 표시되면 작업 중인지 알기 어렵다. | 응답 대기 표시와 대화·컬렉션 스켈레톤, 사이드 패널 스피너를 추가했다. | [PR #53](https://github.com/gomin-diary/gomin/pull/53), [PR #54](https://github.com/gomin-diary/gomin/pull/54) |
| FB-06 | 다음 고민을 유도하며 같은 방식으로 답한다. | 사용자가 주제를 바꾸기 전 현재 고민에 머물고 필요할 때만 질문하도록 했다. 공감·질문·제안의 고정된 순서를 피하고 마무리 의사를 존중하도록 수정했다. | [커밋 c0d881f](https://github.com/gomin-diary/gomin/commit/c0d881f), [PR #52](https://github.com/gomin-diary/gomin/pull/52) |
| FB-07 | 그림이 대화 내용과 동떨어져 보인다. | 요약의 상황을 장소·행동·복색과 연결하고 모리의 표정·몸짓으로 감정을 표현하도록 했다. 자연 풍경을 강제하던 지시도 정리했다. | [커밋 862806c](https://github.com/gomin-diary/gomin/commit/862806c), [PR #51](https://github.com/gomin-diary/gomin/pull/51) |

스켈레톤·스피너의 추가는 PR #54에 대응하는 Git 이력에서 확인했다. 이 문서의 코드 대조와 실제 배포 화면 확인은 별도 근거로 구분한다.

## 반영 완료로 분류하지 않은 의견

메뉴 이름에 관한 FB-03과 키보드 접근성에 관한 FB-04는 수집한 의견에 포함한다. 다만 현재 확인한 공통 메뉴에는 ‘홈’이 남아 있고, FB-04의 구체적인 수정 범위는 확인되지 않아 위 개선 결과에 넣지 않았다.

## 검증 근거

[기존 QA 기록](../../engineering/talk-mvp-qa.md)에는 이미지 재생성 중 버튼 비활성화, 실패 시 기존 결과 유지, 성공 시 결과 교체·저장 상태 초기화의 모의 API 검증이 기록되어 있다. 이 기록은 실제 사용자 재평가나 프롬프트 수정 후 품질 평가를 대신하지 않는다.

대화 프롬프트는 [대화 AI 어댑터](../../../backend/app/talk/provider.py), 이미지 장면 구성은 [그림일기 구성 코드](../../../backend/app/diary/composition.py)에서 확인할 수 있다.

[테스트 결과](results.md) · [프로젝트 구조](../README.md)
