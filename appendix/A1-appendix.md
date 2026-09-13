# A1 — FAQ, 참고

> 자주 묻는 질문과 참고 자료를 모았습니다. 용어는 각 문서에서 처음 나오는 절에서 정의합니다.

---

## A1.2 자주 묻는 질문

**Q. 전사 AX 전략과 로드맵을 먼저 그려야 하지 않나요?**
방향성과 원칙은 정하되, 실행은 전사 빅뱅이 아니라 구체적 파일럿에서 시작합니다. 전사 로드맵을 상세히 확정한 뒤 착수하면 검증되지 않은 가설 위에 큰 계획을 세우게 됩니다. 큰 방향은 가볍게, 첫 파일럿은 구체적으로가 원칙입니다([문서 03](../docs/03-alternative.md)).

**Q. 빠른 파일럿만 반복하면 전사 차원의 큰 가치는 못 얻는 것 아닌가요?**
점진적 확장은 작게 머무르는 것이 아닙니다. 검증된 것을 의사결정을 거쳐 확장하고, 공통 수요를 플랫폼으로 공통화해 규모를 키웁니다. 차이는 "검증 전에 크게"가 아니라 "검증 후에 크게"라는 순서입니다([문서 08](../docs/08-roadmap.md)).

**Q. ROI를 사전에 제시하지 않으면 예산 승인이 어렵습니다.**
사전 점추정 대신 기대값 범위, 옵션 가치, 학습 가치로 제시하고, 파일럿의 비용 상한을 명시합니다. "작은 상한 안에서 큰 가능성을 검증한다"는 틀이 오히려 승인받기 쉽습니다([문서 04](../docs/04-portfolio.md)).

**Q. 처음부터 Private AI(사내 인프라)를 깔아야 하나요?**
아닙니다. 민감 데이터가 없으면 외부 환경에서 빠르게 검증하고, 데이터 주권, 규제, 단가, 지연 임계가 확실해지는 유스케이스부터 Private AI로 전환합니다([문서 07](../docs/07-private-ai-strategy.md)).

**Q. 도구(코파일럿 등)를 도입했는데 왜 효과가 없나요?**
도구 도입은 전환이 아닙니다. 업무 흐름 재설계, 사용 정착 설계, 재사용 자산 축적이 없으면 라이선스 가동률만 낮습니다([문서 01](../docs/01-diagnosis.md), [문서 05](../docs/05-operating-model.md)).

**Q. "빠르게 실패하라"는데, 실패하면 누가 책임지나요?**
선의의 실험적 실패와 명백한 위반(윤리, 규제, 안전)은 다르게 다룹니다. 전자는 사전에 비용과 기간 상한을 둔 게이트 안에서 일어나는 정상적 학습이며, 게이트의 "중단(kill)"은 처벌이 아닙니다. 후자만 위험 등급에 따라 통제합니다. 핵심은 "사람을 탓하기"가 아니라 "문제 원인을 향하기"입니다([문서 05 5.6절](../docs/05-operating-model.md)).

**Q. 직원들이 개인 AI 도구를 몰래 쓰고 있는 것을 발견했습니다. 금지해야 하나요?**
금지는 사용을 없애지 않고 더 깊이 숨깁니다. 먼저 등록하고, 넣는 데이터의 등급으로 위험을 판정한 뒤, 저위험은 승인 경로로 옮기고 고위험은 대체재를 먼저 준 다음 중단합니다. 섀도 AI의 규모는 통제의 약함이 아니라 공식 경로가 수요에서 떨어진 거리이므로, 발견된 사용은 곧 유스케이스 발굴의 입력이기도 합니다([문서 10 10.4절](../docs/10-governance.md)).

**Q. 이 방법론은 특정 벤더 제품을 전제하나요?**
방법론 자체는 벤더 중립적입니다. Private AI 구현 단계에서 한 가지 구체 경로로 PAIF/VCF 기반 시리즈를 참조로 연결할 뿐, 다른 구현으로도 동일한 원칙을 적용할 수 있습니다.

## A1.3 참고

- 본 가이드의 의사결정과 점진적 실행 개념(결정의 되돌림 가능성 구분, 최소 관통 파일럿, 가치 가설과 게이트, 역량 축적)은 제품 개발, 린 방법론, 전환 관리 분야에서 널리 통용되는 사고를 AX 맥락에 맞춰 정리한 것입니다.
- **심리적 안전감**(5.6절) — Amy C. Edmondson, *The Fearless Organization* (2018). 심리적 안전감을 "처벌, 창피 없이 아이디어, 질문, 우려, 실수를 말할 수 있다는 믿음"으로 정의하며, 성과가 높은 팀일수록 오류를 더 솔직히 드러낸다는 연구를 제시합니다.
- **자동화와 증강 분류**(4.2절) — Anthropic Economic Index. 실제 AI 사용 데이터에서 증강(augmentation)이 완전 자동화보다 우세하게 나타나며, 직무와 인터페이스별로 사용 패턴이 크게 다릅니다("할 수 있다"와 "실제로 쓰인다"의 차이, 4.6.1절). 회차마다 수치가 갱신되므로 인용 시 해당 회차와 발간 시점을 병기하시기 바랍니다. (원문: [Anthropic Economic Index](https://www.anthropic.com/economic-index))
- **과업 기반 분류**(4.2절) — 직무→과업→활동으로 분해한 뒤 목적을 먼저 정의하고, 각 활동을 자동화, 증강, 사람 전담(Human-only) 영역으로 나누는 접근. 자동화/증강 구분은 위 Anthropic Economic Index 등 실증과 맞닿아 있습니다. 본 가이드는 이를 일반 개념으로 반영하며, 분류가 기존 사고 틀에 갇히는 한계도 함께 짚습니다.
- **시장 신호: 프로덕션 AI의 프라이빗 클라우드 이동**(7.1절) — Broadcom, *Private Cloud Outlook 2026*(2회차 연례 조사). 응답 기업의 56%가 프로덕션 AI 추론을 프라이빗 클라우드에서 운영 중이거나 계획 중이라고 답했고, AI가 IT에 새로 부과하는 최대 요구로 데이터 보호와 프라이버시(37%)와 보안과 통제(36%)를 꼽았으며, 퍼블릭 클라우드의 1순위 우려가 보안에서 비용으로 바뀌었다고 보고합니다. 검증과 확장 단계에서 데이터 주권, 비용, 통제 압력이 커진다는 본 가이드 7.1절의 논지와 같은 방향을 가리키는 외부 신호입니다. 다만 벤더가 발간한 설문이므로 절대 수치보다 방향성의 참고 자료로 보시기 바랍니다. (원문: [Understand what's driving shifts in AI demands](https://www.linkedin.com/pulse/understand-whats-driving-shifts-ai-demands-vmware-1odje/))
- **시장 신호: 온프렘 회귀는 넓게 계획되고 좁게 실행된다**(9.3절) — 조사들이 방향은 같되 폭은 다르게 보고합니다. Barclays의 CIO 설문(2024년 하반기분)에서는 CIO의 86%가 "일부 워크로드"를 퍼블릭 클라우드에서 되돌릴 계획이라고 답해 조사 사상 최고치를 기록했지만, IDC 조사에서 워크로드 전반의 전면 회귀를 계획한 곳은 8–9%에 그칩니다. 즉 온프렘 회귀는 전면 철수가 아니라 선별적 재배치로 나타나며, 자산을 가르고 패턴이 예측 가능해진 워크로드부터 하나씩 옮긴다는 9.3절의 규율과 같은 방향입니다. 두 수치의 모수가 다르다는 점 — "일부 회귀를 계획한 CIO 비율" 대 "전면 이동을 실행한 기업 비율" — 에 유의하십시오. (Barclays 원자료는 비공개라 2차 인용으로 유통됩니다: [86% 수치와 모수 해설](https://www.digital-chiefs.de/en/cloud-repatriation-2026-statistical-illusion/), [앞선 조사분(83%)의 해설](https://www.channelnomics.com/insights/breaking-down-the-83-public-cloud-repatriation-number), [IDC 블로그 원문](https://blogs.idc.com/2024/10/28/storm-clouds-ahead-missed-expectations-in-cloud-computing/))
- **업계 관점: 외주(FDE)에서 내부 AI Engineer로**(5.8절) — Andrew Ng, *Forward Deployed Engineers and the Future of AI Engineering*, The Batch / Letters from Andrew Ng(2026-05-29). 고객사에 상주하며 솔루션을 맞추고 정착시키는 Forward Deployed Engineer(FDE)가 부상하고 있으나, 기업은 소수의 외부 FDE보다 자기 조직에서 AI를 만들고 운영할 인력(AI Engineer)을 훨씬 더 많이 필요로 하고, 한 벤더에 깊게 묶이면 선택지(optionality)를 잃기 때문에 AI Engineer 수요가 더 커진다는 논지입니다. AI Engineer 역할이 LLMOps, Evals, AI Data, Harness 엔지니어 등으로 분화하리라는 전망도 함께 제시합니다. 외주로 시작하되 내부 운영 역량과 벤더 선택지를 종착점으로 둔다는 본 가이드 5.8절과 같은 방향의 외부 근거입니다. 다만 (가) 수요 차이는 "훨씬 많다"는 정성적 표현이며 배수와 수치로 제시되지 않았고, (나) 원문은 FDE를 부정하지 않고 FDE와 AI Engineer를 모두 새로 생기는 일자리로 보며(외주의 깊은 통합은 도입 속도와 완성도에서 단기 이점), (다) 선택지 보존에는 추상화와 운영 비용과 벤더 고유 기능 포기라는 트레이드오프가 따른다는 점을 함께 보시기 바랍니다. (원문: [Forward Deployed Engineers and the Future of AI Engineering](https://www.deeplearning.ai/the-batch/forward-deployed-engineers-and-the-future-of-ai-engineering))
- **실패율과 손익 괴리의 외부 실증**(1.2.3절, 8.2절) — 2025–2026년의 여러 조사가 "파일럿은 많은데 손익은 움직이지 않는다"는 같은 그림을 서로 다른 각도에서 보여 줍니다. S&P Global Market Intelligence(451 Research) 설문에서는 AI 이니셔티브 대부분을 폐기했다는 기업이 42%(전년 17%)로 늘었고 PoC의 46%가 프로덕션 도달 전에 접혔으며([보도](https://www.ciodive.com/news/AI-project-fail-data-SPGlobal/742590/)), IDC 조사는 PoC의 88%가 대규모 배포에 이르지 못한다고 보고했습니다([보도](https://www.cio.com/article/3850763/88-of-ai-pilots-fail-to-reach-production-but-thats-not-all-on-it.html)). McKinsey의 2026년 State of AI 조사에서는 AI 사용자의 80%가 개인 생산성 향상을 체감하는데도, EBIT의 5% 이상을 AI에 귀속시키는 고성과 기업은 6%에 그쳤습니다([원문](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai)). 널리 인용되는 MIT Project NANDA의 "95%가 측정 가능한 손익 기여 없음"(*The GenAI Divide: State of AI in Business 2025*, 2025-07)은 동료평가 없는 예비 연구라는 한계가 있어 방향성 참고로만 보시기 바랍니다([보도](https://finance.yahoo.com/news/mit-report-95-generative-ai-105412686.html)). **주의: 이 수치들은 모수가 전부 다릅니다** — 각각 '대부분을 폐기한 기업 비율', '프로덕션 미도달 PoC 비율', '손익 귀속 고성과 기업 비율', '손익 기여가 확인되지 않은 조직 비율'입니다. 단일 "AI 실패율"로 합산 인용하지 말고, 병목이 도입과 활동이 아니라 손익 연결과 역량 축적에 있다는 방향성의 근거로만 쓰는 것이 정직합니다.
- **에이전트 거버넌스: 실패 예측과 보안 리스트**(10.3절) — Gartner는 에이전틱(agentic, 도구를 호출해 스스로 행동하는) AI 프로젝트의 40% 이상이 2027년 말까지 취소될 것으로 예측했습니다(2025-06 보도자료; 사유는 비용 증가, 불명확한 사업 가치, 리스크 통제 부재). 실측이 아닌 예측치이고 표본도 자사 웨비나 참석자라는 한계가 있으나, 실패 원인을 기술이 아니라 거버넌스에서 찾는다는 점에서 10.3절과 같은 방향입니다. OWASP는 LLM 애플리케이션 Top 10(2026)에서 과잉 권한(Excessive Agency)을 상위 리스크로 올렸고, 별도의 에이전틱 애플리케이션 Top 10(2026)에서 신원과 권한 남용과 인간-에이전트 신뢰 악용을 주요 항목으로 다뤘습니다 — 에이전트별 고유 신원, 최소 권한, 민감 행위 확인이라는 10.3절의 통제와 같은 원리입니다. (원문: [Gartner 보도자료](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027), [OWASP GenAI Security Project](https://genai.owasp.org/))
- **섀도 AI의 규모와 비용**(10.4절) — 세 조사가 서로 다른 각도에서 같은 그림을 보여 줍니다. Microsoft와 LinkedIn의 *2024 Work Trend Index*(31개국 31,000명 설문)에서는 직장에서 AI를 쓰는 사람의 78%가 회사가 제공하지 않은 자기 도구를 가져와 쓴다고 답했습니다. PagerDuty의 섀도 AI 설문(2026-06, 미국, 영국, 호주, 일본의 사무직 1,250명)에서는 66%가 회사 정책에 어긋난다고 알면서도 AI 도구를 썼다고 답했고, AI를 업무에 써 본 응답자의 89%는 그 도구를 개인 생활에서 먼저 접했다고 답했습니다. IBM의 *2025 Cost of a Data Breach Report*(Ponemon Institute 조사, 600개 조직)는 섀도 AI가 관여한 침해가 전 세계 평균 침해 비용에 67만 달러를 더했고, 조직의 63%가 섀도 AI를 다룰 AI 거버넌스 정책이 없으며, AI 관련 보안 사고를 겪은 침해 조직의 97%가 적절한 AI 접근 통제가 없었다고 보고합니다. **주의: 모수가 전부 다릅니다** — 첫째는 'AI 사용자 중 비율', 둘째는 '사무직 응답자 중 비율', 셋째는 '침해를 겪은 조직 기준의 비용과 비율'입니다. 하나의 "섀도 AI 비율"로 합산하지 말고, 수요는 넓고 정책은 비어 있으며 비용은 실재한다는 10.4.2절 방향성의 근거로만 쓰시기 바랍니다. 셋 다 벤더가 발간한 조사라는 점도 함께 보십시오. (원문: [Microsoft 2024 Work Trend Index](https://blogs.microsoft.com/blog/2024/05/08/microsoft-and-linkedin-release-the-2024-work-trend-index-on-the-state-of-ai-at-work/), [PagerDuty 보도자료](https://www.pagerduty.com/newsroom/shadow-ai-workplace-survey-2026/), [IBM 2025 Cost of a Data Breach](https://www.ibm.com/think/x-force/2025-cost-of-a-data-breach-navigating-ai))
- **법정 의무: 한국 AI 기본법**(5.5절과 워크시트 B-0) — 「인공지능 발전과 신뢰 기반 조성 등에 관한 기본법」, 2026-01-22 법과 시행령 동시 시행. 고영향 AI 사업자에게 위험관리방안, 설명 방안, 사람의 관리, 감독, 문서 작성 의무를, 고영향과 생성형 AI에 이용 사실 고지와 생성물 표시 의무를 부과하며, 시행 후 최소 1년의 계도기간을 운영합니다. 본 가이드의 비례적 거버넌스, 휴먼인더루프, 게이트 기록이 이 법정 의무와 같은 방향이므로, 별도 대응 체계 없이 기존 게이트에 연계하는 것이 합리적입니다. (원문: [법제처 국가법령정보센터](https://www.law.go.kr/lsSc.do?query=인공지능+발전과+신뢰+기반+조성) — 법령명으로 검색, 적용 전 시행령과 고시 최신본 확인)
- **업계 프레임워크: Platform Engineering 2.0**(6절, 6.7절) — Broadcom, PlatformEngineering.org 공동 백서, *Platform Engineering 2.0: An Evolution for the AI Era*. 개발자 중심의 기존 플랫폼(Platform Engineering 1.0)이 AI 네이티브 플랫폼, 다중 페르소나, 내장 FinOps, 보안의 기반 계층 내장, 컴포저블(조합형) 아키텍처의 다섯 축으로 확장되어야 한다는 프레임워크로, 06의 진화형 아키텍처(6.2절), 골든 패스(6.3절), 비용 규율(6.7절) 논지와 같은 방향입니다. 백서가 인용한 두 제3자 통계는 1차 출처로 직접 확인했습니다 — 조직의 90%가 하나 이상의 (내부 개발자) 플랫폼을 도입(Google DORA, [2025 State of AI-assisted Software Development](https://dora.dev/dora-report-2025/)), 기업이 평균적으로 필요량보다 약 35% 더 많은 클라우드 자원에 지출(KPMG, [As cloud over-spending rises, look to cost optimization](https://kpmg.com/xx/en/our-insights/transformation/cloud-cost-optimization.html)). 후자는 '지출의 35%가 낭비'가 아니라 '필요량 대비 약 35% 초과 지출'이라는 점에 유의해 6.7절에 그대로 반영했습니다. (백서 원문: [The Time for Platform Engineering 2.0 Is Now](https://www.linkedin.com/pulse/time-platform-engineering-20-now-vmwarevcf-m3yfc/))
- **업계 프레임워크: FinOps 관리 범위(Scopes)**(6.7절) — FinOps Foundation, *FinOps Framework*. 2025년 프레임워크 갱신에서 관리 범위를 퍼블릭 클라우드에서 기술 지출 전반으로 넓히는 Scopes 개념을 도입해, SaaS, 데이터센터, 데이터 플랫폼, AI, 라이선스를 기술 범주(Technology Categories)로 공식화했습니다. 재단의 사명도 "클라우드의 가치"에서 "기술의 가치"를 관리하는 사람들로 바뀌었습니다. 6.7절의 "2025년부터 SaaS, 데이터센터, AI 지출까지 공식 관리 범위" 서술의 출처입니다. (원문: [FinOps Framework Overview](https://www.finops.org/framework/))
- Private AI 구현의 구체 경로는 다음 시리즈를 참조하시기 바랍니다.
  - [VCF Private AI 가이드 시리즈 허브](https://github.com/JaeHoYun/vcf-private-ai)
  - [① 인프라와 운영](https://github.com/JaeHoYun/vcf-private-ai/tree/main/01-infra) | [② 벡터 DB](https://github.com/JaeHoYun/vcf-private-ai/tree/main/02-vectordb) | [③ 서빙 API](https://github.com/JaeHoYun/vcf-private-ai/tree/main/03-serving-api) | [④ RAG 아키텍처](https://github.com/JaeHoYun/vcf-private-ai/tree/main/04-rag) | [⑤ 보안과 거버넌스](https://github.com/JaeHoYun/vcf-private-ai/tree/main/05-security) | [⑥ 사이징과 비용](https://github.com/JaeHoYun/vcf-private-ai/tree/main/06-sizing-cost) | [⑦ 통합 설계](https://github.com/JaeHoYun/vcf-private-ai/tree/main/07-design)

---

[← 상위 README](../README.md) | [← 이전: 10 AI 거버넌스](../docs/10-governance.md) | [다음: A2 한국 규제와 정책 타임라인 →](A2-kr-regulatory-timeline.md)
