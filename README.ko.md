# Codex용 Playground

[English](README.md) | [한국어](README.ko.md)

시각적 컨트롤, 실시간 미리보기, 복사 가능한 프롬프트 출력을 갖춘 단일 HTML 파일 형태의 인터랙티브 플레이그라운드를 만들 수 있게 해주는 Codex 플러그인입니다.

이 저장소는 Anthropic의 `playground` Claude 플러그인을 Codex에서 사용할 수 있도록 변환한 버전입니다.

## 원본

- 원본 프로젝트: `claude-plugins-official/plugins/playground`
- 원저작자: Anthropic
- 라이선스: Apache License 2.0

이 변환본은 원본의 Apache License 2.0 라이선스 전문을 유지하고, Codex 플러그인용 메타데이터를 추가했습니다.

## 이 변환본의 변경 사항

- Codex 플러그인 검색을 위한 `.codex-plugin/plugin.json`을 추가했습니다.
- 스킬과 README의 Claude 전용 표현을 Codex 기준 표현으로 수정했습니다.
- 브라우저 자동 실행 안내를 Codex의 로컬 파일 전달 방식에 맞게 수정했습니다.
- 원본 스킬 템플릿과 Apache License 2.0 라이선스 전문은 유지했습니다.

## 비공식 프로젝트

이 프로젝트는 독립적인 Codex 호환 변환본입니다. Anthropic과 제휴, 후원, 보증 관계가 없습니다.

Anthropic 명칭과 관련 표기는 Apache-2.0 라이선스로 공개된 원본 저작물의 출처를 표시하기 위한 목적으로만 사용됩니다.

## Playground란?

Playground는 다음 요소를 가진 자체 완결형 HTML 파일입니다.

- 한쪽에는 인터랙티브 컨트롤
- 다른 한쪽에는 실시간 미리보기
- 하단에는 복사 버튼이 있는 프롬프트 출력

사용자는 컨트롤을 조정하며 시각적으로 탐색한 뒤, 생성된 프롬프트를 Codex에 다시 붙여 넣어 사용할 수 있습니다.

## 언제 사용하나요?

사용자가 특정 주제에 대한 인터랙티브 플레이그라운드, 탐색기, 시각적 도구를 요청할 때 사용합니다. 특히 입력 공간이 넓거나, 시각적이거나, 구조적이라서 일반 텍스트로 설명하기 어려운 경우에 유용합니다.

## 템플릿

이 스킬에는 자주 쓰는 플레이그라운드 유형을 위한 템플릿이 포함되어 있습니다.

- `design-playground`: 컴포넌트, 레이아웃, 간격, 색상, 타이포그래피 같은 시각 디자인 결정
- `data-explorer`: SQL, API, 파이프라인, 정규식 같은 데이터 및 쿼리 구성
- `concept-map`: 개념 지도, 지식 공백, 범위 매핑 같은 학습 및 탐색
- `document-critique`: 승인, 거절, 코멘트 흐름이 있는 문서 리뷰
- `diff-review`: diff, commit, PR을 위한 코드 리뷰
- `code-map`: 코드베이스 아키텍처, 컴포넌트 관계, 데이터 흐름, 레이어 다이어그램

## 설치

이 플러그인을 Codex 플러그인 마켓플레이스에 추가하면 `playground` 스킬을 사용할 수 있습니다.

마켓플레이스 저장소로 배포하려면 다음 구조를 사용하세요.

```text
repo-root/
  marketplace.json
  plugins/
    playground/
      .codex-plugin/plugin.json
      skills/
      README.md
      README.ko.md
      LICENSE
      NOTICE
```

마켓플레이스 엔트리는 `./plugins/playground`를 가리켜야 합니다.

## 라이선스

이 변환본은 원본과 동일하게 Apache License 2.0으로 배포됩니다. 자세한 내용은 `LICENSE`와 `NOTICE`를 확인하세요.
