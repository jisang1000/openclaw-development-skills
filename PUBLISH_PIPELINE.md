# PUBLISH_PIPELINE.md

`openclaw-development-skills`용 반복 가능한 publish 파이프라인.

## 목표
- 개별 성공을 넘어서, 여러 스킬을 일관된 규칙으로 publish한다.
- slug / version / 검증 / 승인 경계를 명확히 한다.

## 현재 확인된 publish 성공
- `jisang1000-verification-before-completion@1.0.0`
- `jisang1000-systematic-debugging@1.0.0`
- `jisang1000-writing-plans@1.0.0`

## slug 규칙
- 최종 slug는 `jisang1000-<skill-folder-name>` 기준으로 본다.
- 폴더명은 소문자 kebab-case 유지.
- display title은 자유롭게 두되, 배포 식별자는 폴더명 기준으로 고정한다.

## version 규칙
- 첫 publish: `1.0.0`
- 문서/설명만 보강: patch (`1.0.1`)
- 사용법/동작 범위가 늘어남: minor (`1.1.0`)
- 호환성 깨짐/구조 개편: major (`2.0.0`)

## publish 전 체크리스트
1. `SKILL.md` 존재 확인
2. 설명이 실제 사용 사례를 포함하는지 확인
3. 위험한 자동화/과도한 자율성 표현 제거
4. README 또는 예시가 있으면 최신 상태인지 확인
5. git diff 확인
6. publish 대상 slug / version 결정
7. 외부 publish 승인 확인

## 추천 다음 publish 후보
- `development-workflow`
- `executing-plans`
- `requesting-code-review`

## 운영 원칙
- 한 번에 여러 개를 억지로 publish하지 않는다.
- 승인 없는 외부 배포는 하지 않는다.
- publish 후에는 slug, version, 성공 여부를 별도 로그에 남긴다.
