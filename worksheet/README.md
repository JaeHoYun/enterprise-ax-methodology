# 채워넣기 워크시트 (진단·발굴·게이트·확장)

> 본문 방법론을 현장에서 채워 쓰는 양식 모음입니다. 계산용 스프레드시트가 아니라 항목을 따라 직접 적어 넣는 마크다운 양식이며, 빈칸이 많은 것은 채우는 용도이기 때문입니다(미완성이 아닙니다).

이 폴더의 워크시트는 [문서 03 대안](../docs/03-alternative.md)의 실행 루프(진단 → 발굴 → 파일럿 게이트 → 다음 사이클)와 [문서 06 전사 확장](../docs/06-enterprise-scale.md)의 확장 국면, 그리고 [문서 09 브라운필드 AX](../docs/09-brownfield-assessment.md)의 현황 진단·전환에 쓰입니다. 각 양식이 무엇을 위한 것이고, 누가 채우며, 언제 쓰고, 채운 뒤 무엇으로 이어지는지를 먼저 정리합니다.

## 워크시트 개요

| 워크시트 | 무엇을 채우나 | 주 작성자 | 언제 | 채운 뒤 이어지는 곳 |
|----------|---------------|-----------|------|---------------------|
| [성숙도 자가진단](maturity-self-assessment.md) | 현재 AX 성숙도 위치와 병목 차원 | AX 추진 리더 + 각 차원 담당, 임원 검토 | 착수 전, 이후 분기마다 | 병목 차원 → 우선 보강 과제 / 유스케이스 발굴 방향의 입력 |
| [유스케이스 캔버스](use-case-canvas.md) | 후보 유스케이스의 가치 가설 | 현업 프로덕트 오너 + 기획 (실현가능성은 개발·인프라·데이터와 함께) | 발굴·선별 단계, 후보마다 | 채택된 캔버스 → 파일럿 게이트의 가설·성공기준으로 |
| [파일럿 게이트](pilot-gate.md) | 파일럿의 확장/중단 판정 | 현업 오너 + 개발·인프라, 거버넌스, 의사결정자 | 파일럿 착수 시·판정 시 | 확장 → 운영·다음 사이클 / 중단 → 재검증·다음 후보 |
| [확장 준비도](scale-readiness.md) | 전사 확장 전환 신호·아키텍처 결정·기준선 | AX/CoE 리더 + 플랫폼·아키텍처·거버넌스·재무, 임원 검토 | 여러 파일럿의 공통 수요가 보일 때, 이후 분기마다 | 끌어올릴 계층 → platform-pull / 결정 기록 → 결재 근거 / [문서 06](../docs/06-enterprise-scale.md) |

## 누가 쓰나 (역할별)

한 워크시트를 한 사람이 다 채우는 것이 아닙니다. 역할이 각자 자기 칸을 채우고, 파일럿 게이트에서 합쳐 판정합니다.

- **임원·전략 (CIO·CDO·CoE 리더)** — 성숙도 자가진단으로 큰 그림과 투자 우선순위를 잡고, 파일럿 게이트에서 확장/중단을 결정합니다.
- **기획·현업 프로덕트 오너** — 유스케이스 캔버스로 가치 가설을 작성하고, 게이트의 가설·성공/중단 기준을 정의합니다.
- **개발·데이터·인프라** — 캔버스의 데이터 준비도·실현가능성을 평가하고, 게이트에서 실행과 통제 충족을 확인합니다.
- **거버넌스·리스크** — 게이트의 위험 등급과 필요 통제 항목을 점검합니다.

## 어떻게 연계되나 (흐름)

```
  성숙도 자가진단 ──(병목·우선 방향)──> 유스케이스 캔버스 ──(채택 후보)──> 파일럿 게이트
        ▲                                                                    │
        └──────────────(분기 재진단 / 다음 사이클)◀───────(확장·중단 판정)───┘
```

1. **성숙도 자가진단**으로 현재 위치와 병목을 파악합니다. 어느 영역의 유스케이스를 먼저 볼지 방향이 나옵니다.
2. 그 방향으로 **유스케이스 캔버스**를 후보마다 작성합니다. 우선순위가 높은 후보가 파일럿 대상이 됩니다.
3. 채택된 캔버스의 가치 가설·성공기준을 **파일럿 게이트**로 옮겨 착수하고, 판정 시점에 확장/중단을 결정합니다.
4. 판정 결과(특히 platform-pull 신호와 축적된 역량 자산)는 다음 사이클의 입력이 되고, 분기마다 성숙도를 재진단합니다.

## 채운 뒤 어떻게 활용하나

- **보관·갱신** — 팀 내부에 두고 분기마다(성숙도)·파일럿마다(캔버스·게이트) 갱신합니다.
- **의사결정 근거** — 파일럿 게이트 기록은 확장/중단 결재의 근거이자 사후 감사 추적이 됩니다.
- **경영진 보고** — 성숙도 추이와 게이트 통과·중단 이력은 [문서 08 측정](../docs/08-roadmap.md)의 학습 지표로 그대로 보고에 씁니다.
- **수치 연계** — GPU·노드·용량 등 정량 산정이 필요하면 사이징·비용 편([⑥ vcf-private-ai-sizing-cost](https://github.com/JaeHoYun/vcf-private-ai-sizing-cost))의 계산 워크북을 사용하고, 그 결과 수치를 이 양식의 해당 칸에 옮겨 적습니다. 본 워크시트 자체에는 자동 계산이 없습니다.

## 파일

| 파일 | 연계 본문 |
|------|-----------|
| [`maturity-self-assessment.md`](maturity-self-assessment.md) | [docs/02 성숙도](../docs/02-maturity.md) |
| [`use-case-canvas.md`](use-case-canvas.md) | [docs/04 유스케이스](../docs/04-portfolio.md) |
| [`pilot-gate.md`](pilot-gate.md) | [docs/03 대안](../docs/03-alternative.md) |
| [`scale-readiness.md`](scale-readiness.md) | [docs/06 전사 확장](../docs/06-enterprise-scale.md) |
| [`ai-estate-inventory.md`](ai-estate-inventory.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`gap-register.md`](gap-register.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`disposition-matrix.md`](disposition-matrix.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`ai-finops-scorecard.md`](ai-finops-scorecard.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`governance-sovereignty-gap.md`](governance-sovereignty-gap.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`transition-report.md`](transition-report.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |
| [`transition-charter.md`](transition-charter.md) | [docs/09 브라운필드](../docs/09-brownfield-assessment.md) |

## 브라운필드 트랙 워크시트 (이미 AI를 쓰는 조직)

위 네 워크시트가 신규 구축(그린필드) 정규 루프(진단 → 발굴 → 게이트 → 확장)에 쓰인다면, 아래 일곱은 **이미 AI를 광범위하게 쓰는 조직**이 현존 자산을 거꾸로 거슬러 점검·정리하는 [문서 09 브라운필드 AX](../docs/09-brownfield-assessment.md)의 입력입니다. 전방용 `scale-readiness`와 반대 방향(기존 자산 감사)입니다.

흐름: **자산 인벤토리** → **갭 레지스터** → (**처분 매트릭스**·**FinOps 스코어카드**·**거버넌스/주권 갭**) → **종합 개선안 보고서** → **전환 차터** → 검증 유스케이스는 위 정규 루프(캔버스 → 게이트)로 합류.

| 워크시트 | 무엇을 채우나 |
|----------|---------------|
| [자산 인벤토리](ai-estate-inventory.md) | 현황(AS-IS) 9개 블록(컴퓨트·워크로드·데이터·퍼블릭 클라우드 AI·에이전트·조직·비용·보안·MLOps 플랫폼/파이프라인) 실측 |
| [갭 레지스터](gap-register.md) | 항목별 결함을 안티패턴 9종·6차원에 태깅, 심각도×영향 우선순위 |
| [처분 매트릭스](disposition-matrix.md) | 자산별 6R(잔류·이전·회수·통합·재구성·폐기) 결정 |
| [FinOps 스코어카드](ai-finops-scorecard.md) | 기존 AI 지출 감사(단위경제·가동률·회수 손익분기) |
| [거버넌스·주권 갭](governance-sovereignty-gap.md) | NIST AI RMF·EU AI Act·ISO 42001 대비 통제 격차 + 데이터주권 소급 |
| [종합 개선안 보고서](transition-report.md) | 현황→갭→TO-BE→마이그레이션→조직→비용/통제→로드맵 (경영진 제출 템플릿) |
| [전환 차터](transition-charter.md) | 전환 프로젝트 목표·범위·게이트0·리스크·성공기준 |

## 중요

- 이 워크시트는 **채워넣기 양식**입니다. 항목별로 직접 값을 적고 판단을 기록하는 용도이며, 자동 계산은 없습니다.
- 모든 항목은 작성 시점 기준이며 환경에 따라 달라집니다. 적용 전 [상위 README](../README.md)와 본문으로 재확인하세요.

---

[← 상위 README](../README.md) · [02 성숙도](../docs/02-maturity.md) · [03 대안](../docs/03-alternative.md) · [04 유스케이스](../docs/04-portfolio.md)
