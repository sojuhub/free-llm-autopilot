# Aside, 무료 LLM으로 시작하세요

**무료 모델을 찾고, 가입하고, Aside에 연결하고, 매일 점검하는 에이전트 스킬.**

Space Bunny, OpenRouter, NVIDIA처럼 계속 바뀌는 무료 LLM을 직접 따라다니는 대신, Aside에게 설정과 관리를 맡겨보세요.

[바로 시작하기](#바로-시작하기) · [실행 지침 읽기](SKILL.md) · [현재 확인 범위](#현재-확인-범위) · [English](#english)

> 여기서 “무료”는 조건을 충족한 **LLM API의 추가 사용료 $0**를 뜻합니다. Aside 자체 요금, 초기 설정을 수행하는 모델 비용, 무제한 사용을 보장하지 않습니다. Aside 및 각 공급자와 무관한 커뮤니티 프로젝트입니다.

## 무료 모델 찾기에서 끝나지 않습니다

무료라는 글을 보고 가입했는데 내 앱에서는 연결이 안 되거나, 며칠 뒤 무료 제공이 끝나는 경우가 있습니다. 짧은 답변은 잘해도 브라우저 도구를 사용하면 한도에 걸릴 수도 있습니다.

이 프로젝트의 목표는 **내 Aside에서 실제 작업이 끝나는 무료 경로를 만들고, 그 경로를 최신 상태로 유지하는 것**입니다.

```text
현재 환경·계정 확인
        ↓
무료 모델 탐색 → 필요한 무료 계정 가입
        ↓
Aside 연결 → 공개 페이지 읽기·최종 답변 확인
        ↓
하루 한 번 점검
        ├─ 새 무료 경로 추가
        ├─ 일시 제한은 대기
        └─ 종료·유료화된 경로 제거
```

## 바로 시작하기

준비물은 사용할 수 있는 [Aside](https://aside.com/), 최초 설정을 진행할 모델, 가입에 사용할 본인 계정입니다. 자동 가입에는 해당 계정에 대한 접근이, 매일 점검에는 실행 가능한 루틴 기능이 필요합니다. 비밀번호나 API 키를 채팅에 붙여 넣을 필요는 없습니다.

### 1. Aside에 아래 요청을 붙여 넣으세요

```text
https://github.com/sojuhub/free-llm-autopilot 의 SKILL.md를 읽고
내 Aside 환경에 Free LLM Autopilot을 설치하고 설정해줘.

현재 프로필·연결된 계정·모델·기존 루틴을 먼저 확인해줘.
무료 제공 조건이 맞는 새 업체는 내가 지정한 본인 계정으로
무료 약관 동의·회원가입·인증·API 키 연결까지 진행해줘.
가입 계정을 모르면 먼저 물어봐. 키와 인증 코드는 채팅에 출력하지 마.
유료 결제·카드 등록·자동 충전은 하지 마.

무료 모델 하나로 공개 웹페이지를 읽고 최종 답변까지 확인해줘.
기존 기본 모델은 유지하고, 무료 모델을 선택하는 방법을 알려줘.
매일 내 시간대 오전 9시에 무료 목록을 갱신하는 루틴도 하나 등록해줘.
신규 경로는 검증 후 추가하고, 종료·유료화된 관리 경로는 제거해줘.
업데이트한 공급자 지식은 설치된 SKILL.md에 반영해줘.
마지막에 실제 확인한 결과와 아직 안 된 부분을 구분해서 알려줘.
```

설치 경로를 외울 필요는 없습니다. 에이전트가 현재 버전의 사용자 스킬 위치를 확인합니다. 파일을 직접 설치하려면 [SKILL.md](SKILL.md)를 받아 사용하는 앱의 사용자 스킬 폴더 아래 `free-llm-autopilot/SKILL.md`로 두세요. 등록된 스킬 목록에서 발견되는지도 확인해야 합니다.

### 2. 첫 성공을 확인하세요

“연결 완료”라는 말 대신 다음 결과가 나오는지 보세요.

- Aside에서 선택할 수 있는 정확한 공급자·모델 이름
- 그 모델이 공개 페이지를 읽은 도구 결과와 최종 답변
- 무료 판단의 근거와 남은 제한
- 일일 루틴의 활성 상태·시간대·다음 실행 시각

어느 단계가 막혔다면 그 단계만 이어서 처리합니다. 키가 만들어졌다고 브라우저 작업까지 성공한 것은 아닙니다.

### 3. 평소에는 이렇게 요청하세요

**공개 자료 조사**

```text
Free LLM Autopilot 기준으로 지금 사용 가능한 무료 모델을 선택해서
이 공개 페이지의 핵심 내용을 정리해줘. 무료 경로가 없으면 알려줘.
```

**목록 갱신**

```text
무료 LLM 연결 상태를 점검하고, 새 무료 제공을 찾아 연결해줘.
일시적인 한도 초과는 대기 처리하고, 확실히 종료된 경로만 제거해줘.
```

**기본 모델 변경**

```text
검증된 무료 모델을 Aside의 새 일반 작업 기본값으로 설정해줘.
어떤 모델 범주에 적용했는지 알려주고, 중요한 작업의 설정은 유지해줘.
```

모델을 직접 고를 수도 있습니다. 이 스킬은 에이전트에게 선택·관리 절차를 가르칩니다. 모든 GUI 호출을 가로채거나 진행 중인 작업을 자동 이관하는 플러그인은 아닙니다.

## 어떤 무료 모델을 찾나요?

아래는 탐색 출발점입니다. **모두 Aside에서 동작한다고 보증하는 지원 목록은 아닙니다.** 확인 기준일: 2026-10-04.

| 경로 | 살펴볼 점 | 공식 출처 |
| --- | --- | --- |
| OpenCode Zen / Space Bunny | 기간 한정 무료 모델. 다른 Zen 모델의 요금·데이터 정책은 각각 확인 | [Zen](https://opencode.ai/docs/en/zen/) |
| OpenRouter Free | 필요한 기능을 지원하는 무료 모델 중 선택. 품질 순위 기반 선택은 아님 | [Free Router](https://openrouter.ai/openrouter/free) |
| NVIDIA API Catalog | 평가용 조건·계정·할당량·데이터 제한 확인 | [시작 안내](https://docs.api.nvidia.com/nim/re/docs/api-quickstart) |
| Gemini / Groq / Cerebras | 무료 플랜과 실제 Aside 입력 크기·도구 호환성을 검증한 뒤 추가 | [Gemini](https://ai.google.dev/gemini-api/docs/pricing) · [Groq](https://console.groq.com/docs/rate-limits) · [Cerebras](https://inference-docs.cerebras.ai/) |

Space Bunny는 Zen 공식 문서에서 기간 한정 무료로 안내하며, 공급자의 데이터 미보관·학습 미사용 정책을 설명합니다. 다른 무료 모델에는 다른 조건이 적용됩니다. 이름에 “Free”가 있다고 민감한 계정·고객 데이터를 보내도록 설정하지 않습니다.

## 매일 무엇을 관리하나요?

| 발견한 변화 | 스킬이 지시하는 처리 |
| --- | --- |
| 새 무료 업체·모델 | 조건 확인 → 허용된 무료 가입 → 연결·검증 → 후보 추가 |
| 가격 인상·무료 기간 종료 | 해당 스킬이 관리하는 활성 경로에서 제거 |
| 429·일시 장애 | 삭제하지 않고 재시도 시각까지 대기 |
| 인증 만료 | 계정 접근을 복구하거나 필요한 사용자 단계를 표시 |
| 공식 목록 조회 실패 | 기존 설정 보존, 확인되지 않은 경로의 새 사용 보류 |

관리 대상은 이 스킬이 추가했거나 사용자가 맡긴 경로입니다. 다른 설정·계정·공유 키를 지우지 않습니다. 기본 점검은 하루 한 번, 신규 업체 최대 3곳·15분 이내로 제한해 점검 자체가 무료 한도를 소진하지 않게 합니다.

루틴이 실행될 때는 호스트·모델·도구가 사용 가능해야 합니다. 등록 성공과 다음 날 실행 성공은 별도로 확인합니다. 로컬 SKILL.md 갱신은 GitHub에 자동 게시하는 것과도 별개입니다.

## 왜 README와 SKILL.md인가요?

| 파일 | 누구를 위한 것인가요? |
| --- | --- |
| `README.md` | 사람이 이해하고 시작하는 입구: 목적, 설치 요청, 사용 예시, 확인 범위 |
| `SKILL.md` | 에이전트가 읽는 실행 지침: 환경 파악, 가입, Aside 연결, 라우팅, 정리, 루틴 |

별도 서버나 설치용 프로그램 없이 기존 Aside 기능을 활용합니다. 실행 지침은 여전히 파일 하나라 다른 환경에도 옮길 수 있고, 사람은 긴 운영 지침을 먼저 읽지 않아도 시작할 수 있습니다. 구체적인 도구 이름과 설정 형식은 설치된 Aside의 최신 안내를 따릅니다.

## 현재 확인 범위

이 저장소는 **실험 단계의 지침 기반 스킬**입니다.

- 현재 스킬: Codex·Aside 형식 검사 통과. Aside의 프로필·설정·실제 응답·루틴 확인 절차를 포함합니다.
- 기반이 된 개인 환경 기록: Space Bunny·OpenRouter의 Aside 도구 실행 성공 기록이 있습니다. 공개판 신규 설치에서 재현했다는 의미는 아닙니다.
- 과거 제한 사례: NVIDIA는 다단계 작업 중 한도 오류, Groq는 초기 입력 크기 제한을 경험했습니다. 지금도 같다고 단정하지 않으며 설치 시 재확인합니다.
- 아직 미검증: 다양한 사용자 환경의 처음부터 끝까지 설치, 새 공급자 가입의 보편적 성공, 장기간 무인 일일 관리.

공급자 목록과 실행 결과를 구분해 보고하는 것이 이 프로젝트의 원칙입니다. 무료 제공 조건·사이트 인증·모델 품질에 따라 일부 단계는 완료되지 않을 수 있습니다.

## 피드백과 기여

[Issue](https://github.com/sojuhub/free-llm-autopilot/issues)에 Aside 버전, OS, 공급자·모델, 실패한 단계, 비밀정보를 제거한 오류를 남겨주세요. 계정 이메일·키·인증 코드·개인 페이지 캡처는 올리지 마세요.

새 공급자를 제안할 때는 공식 가격·조건 출처와 확인 날짜를 함께 적어주세요. API 한 번 응답, Aside 도구 실행, 최종 답변 성공 중 어디까지 확인했는지 구분하면 다른 사용자가 재사용하기 쉽습니다.

## English

**Use free LLM APIs with Aside — and let your agent maintain the setup.**

Free LLM Autopilot is an Aside-first instruction skill. It guides an agent to discover eligible free providers, complete authorized account onboarding, connect and verify a model in Aside, retire unusable managed routes, and register one daily maintenance routine using the existing scheduler.

“Free” means zero incremental API spending for eligible routes. It does not promise free Aside access, a free bootstrap executor, unlimited quota, or compatibility with every provider. This is an independent community project.

Paste into Aside:

```text
Read https://github.com/sojuhub/free-llm-autopilot/blob/main/SKILL.md
and install Free LLM Autopilot for my current Aside environment.
Use my designated account to register eligible free providers and connect keys.
Ask for the account if it is not established. No payments, cards or auto-recharge.
Verify one public browser task under a free model, preserving my current defaults.
Register one daily maintenance routine at 09:00 in my timezone, reusing any match.
Update the installed skill's provider facts and remove retired managed routes.
Report verified outcomes separately from blocked or untested steps.
```

Read [SKILL.md](SKILL.md) for the full self-contained workflow. The runtime does the work; Markdown alone is not a background service. Public-release onboarding across different user environments and long-running daily operation remain unverified.

## License

MIT. The full license is included in [SKILL.md](SKILL.md#license).
