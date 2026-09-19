# A1. FAQ와 참고

> 자주 묻는 질문과 본문이 인용한 외부 자료의 출처를 모았습니다. 용어는 각 장에서 처음 나오는 곳에 풀어 썼습니다.

---

## A1.1 자주 묻는 질문

**Q. 전사 AX 전략과 로드맵을 먼저 그려야 하지 않나요?**
방향과 목표는 먼저 정해야 합니다. 목표가 없다면 [01장](../docs/01-starting-point.md)의 유형 (가)에 해당하고, 사업 목표에서 내려오는 작업이 첫걸음입니다. 다만 상세한 전사 로드맵을 확정한 뒤에 착수하면 확인되지 않은 가설 위에 큰 계획을 세우게 됩니다. 큰 방향은 가볍게 정하고, 첫 문제는 구체적으로 정의합니다([03장](../docs/03-problem-definition.md)).

**Q. 작은 파일럿만 되풀이하면 전사 차원의 큰 가치는 얻지 못하는 것 아닌가요?**
그럴 위험이 있습니다. 그래서 첫 검증 단위는 큰 목표로 가는 경로 위에서 고릅니다([03장 3.5절](../docs/03-problem-definition.md)). 가치가 부서 사이의 흐름에서 나오는 과제는 좁은 파일럿으로 잡히지 않으므로 범위를 달리 잡습니다([04장 4.8절](../docs/04-validation.md)).

**Q. ROI를 사전에 제시하지 않으면 예산 승인이 어렵습니다.**
단일 숫자 대신 효과의 범위, 손익분기 시점, 민감도, 대안 비교, 회수되지 않는 조건을 제시하고, 파일럿의 비용 상한을 밝힙니다([04장 4.6절](../docs/04-validation.md)).

**Q. 처음부터 사내에 AI 인프라를 갖춰야 하나요?**
과제마다 다릅니다. 민감한 데이터가 없으면 외부 서비스로 빠르게 확인할 수 있고, 규제로 외부 전송이 불가능하면 처음부터 사내 환경이 필요합니다. 어느 쪽도 기본값이 아닙니다([06장](../docs/06-execution-environment.md)).

**Q. AI 보조 도구를 도입했는데 왜 효과가 없나요?**
도구의 도입과 업무의 변화는 다른 일입니다. 어떤 문제를 풀려는 것이었는지가 정의되지 않았거나([03장](../docs/03-problem-definition.md)), 업무 흐름 안에 들어가지 않았을 가능성이 큽니다([07장 7.2절](../docs/07-organization-and-control.md)).

**Q. 문제가 AI 없이도 풀릴 것 같습니다. 그래도 AX 과제로 진행해야 하나요?**
아닙니다. 프로세스 개선, 규칙 기반 자동화, 기존 시스템 개선으로 풀리는 문제라면 그쪽이 대개 더 싸고 확실합니다([03장 3.4절](../docs/03-problem-definition.md)).

**Q. 빠르게 실패하라고 하는데, 실패하면 누가 책임지나요?**
잘해 보려다 생긴 실패와 규정을 어긴 행위는 다르게 다룹니다. 앞의 것은 비용과 기간의 상한을 둔 게이트 안에서 일어나는 정상적인 결과이고, 게이트의 중단은 처벌이 아닙니다([07장 7.3절](../docs/07-organization-and-control.md)).

**Q. 직원들이 개인 AI 도구를 몰래 쓰고 있는 것을 발견했습니다. 금지해야 하나요?**
금지는 사용을 없애지 않고 더 깊이 숨깁니다. 먼저 등록하고, 넣는 데이터의 등급으로 위험을 판정한 뒤, 저위험은 승인된 경로로 옮기고 고위험은 대체 수단을 먼저 준 다음 중단합니다. 발견된 사용은 문제를 찾는 단서이기도 합니다([07장 7.6절](../docs/07-organization-and-control.md), [02장 2.6절](../docs/02-lenses.md)).

**Q. 외부 전문가나 FDE에게 맡기면 빠르지 않나요?**
빠릅니다. 다만 문제와 해법의 윤곽이 있고 사내에 받을 사람이 있을 때 그렇습니다. 구조 문제가 남아 있는 과제는 누가 만들어도 같은 자리에서 멈춥니다([05장](../docs/05-solve-path.md)).

**Q. 이 가이드는 특정 벤더 제품을 전제하나요?**
전제하지 않습니다. 사내 구축을 선택한 경우의 구현 경로 한 예를 [06장](../docs/06-execution-environment.md) 끝과 [README](../README.md)의 관련 가이드에서 안내할 뿐입니다.

## A1.2 참고

- 본문의 검증 방식(결정의 되돌림 가능성 구분, 최소 관통 파일럿, 가치 가설과 게이트)은 제품 개발, 린 방법론, 전환 관리 분야에서 널리 통용되는 사고를 AX 맥락에 맞춰 정리한 것입니다. 되돌림 가능성의 구분은 아마존이 의사결정을 두 유형으로 나눌 때 쓴 two-way door 비유에서 왔습니다.
- **심리적 안전감**(07장 7.3절). Amy C. Edmondson, *The Fearless Organization* (2018). 심리적 안전감을 처벌과 창피 없이 아이디어, 질문, 우려, 실수를 말할 수 있다는 믿음으로 정의하며, 성과가 높은 팀일수록 오류를 더 솔직히 드러낸다는 연구를 제시합니다.
- **자동화와 증강의 분류**(02장 2.8.2절). Anthropic Economic Index. 실제 AI 사용 데이터에서 증강(augmentation)이 완전 자동화보다 우세하게 나타나며, 직무와 사용 방식에 따라 양상이 크게 다릅니다. 회차마다 수치가 갱신되므로 인용할 때는 해당 회차와 발간 시점을 함께 적으시기 바랍니다. (원문: [Anthropic Economic Index](https://www.anthropic.com/economic-index))
- **온프렘 회귀는 넓게 계획되고 좁게 실행된다**(06장 6.5절). 조사들이 방향은 같되 폭은 다르게 보고합니다. Barclays의 CIO 설문(2024년 하반기분)에서는 CIO의 86%가 일부 워크로드를 퍼블릭 클라우드에서 되돌릴 계획이라고 답해 조사 사상 최고치를 기록했지만, IDC 조사에서 워크로드 전반의 전면 회귀를 계획한 곳은 8-9%에 그칩니다. 온프렘 회귀가 전면 철수가 아니라 선별적 재배치로 나타난다는 뜻입니다. 두 수치는 모수가 다릅니다. 앞의 것은 일부 회귀를 계획한 CIO의 비율이고, 뒤의 것은 전면 이동을 계획한 기업의 비율입니다. (Barclays 원자료는 비공개라 2차 인용으로 유통됩니다: [86% 수치와 모수 해설](https://www.digital-chiefs.de/en/cloud-repatriation-2026-statistical-illusion/), [앞선 조사분(83%)의 해설](https://www.channelnomics.com/insights/breaking-down-the-83-public-cloud-repatriation-number), [IDC 블로그 원문](https://blogs.idc.com/2024/10/28/storm-clouds-ahead-missed-expectations-in-cloud-computing/))
- **FDE와 내부 AI Engineer**(05장 5.3절, 5.4절). Andrew Ng, *Forward Deployed Engineers and the Future of AI Engineering*, The Batch(2026-05-29). 고객사에 들어가 솔루션을 맞추고 정착시키는 FDE가 부상하고 있으나, 기업은 소수의 외부 FDE보다 자기 조직에서 AI를 만들고 운영할 인력을 훨씬 더 많이 필요로 하고, 한 벤더에 깊게 묶이면 선택지(optionality)를 잃는다는 논지입니다. 다만 수요 차이는 정성적 표현이며 수치로 제시되지 않았고, 원문은 FDE를 부정하지 않으며, 선택지를 지키는 데에도 비용과 벤더 고유 기능의 포기가 따른다는 점을 함께 보시기 바랍니다. (원문: [Forward Deployed Engineers and the Future of AI Engineering](https://www.deeplearning.ai/the-batch/forward-deployed-engineers-and-the-future-of-ai-engineering))
- **FDE는 팀의 일**(05장 5.3.3절). Palantir 공식 블로그, *A Day in the Life of a Palantir Deployment Strategist*(2022-03-08). 일반적인 프로젝트에 Deployment Strategist와 Forward Deployed Engineer가 함께 투입되고, 앞의 역할은 고객의 운영을 이해해 적용할 곳을 찾고 고객과의 관계와 일정을 맡으며, 두 역할의 경계는 실제로는 자주 흐려진다고 설명합니다. 회사가 채용 홍보 목적으로 쓴 글이라는 점을 감안해, 역할 구성에 관한 사실의 출처로만 씁니다. (원문: [A Day in the Life of a Palantir Deployment Strategist](https://blog.palantir.com/a-day-in-the-life-of-a-palantir-deployment-strategist-951cb59a5a96))
- **FDE의 기대와 위험**(05장 5.3.1절, 5.3.2절). Larry Dignan, *Forward deployed engineers: The promise, peril in AI deployments*, Constellation Research(2026-02-01). FDE가 고객 환경에 들어가 가치 실현을 앞당긴다는 기대와 함께, 현장 인력이 미완성 제품을 가릴 수 있고, 넓은 의미의 벤더 의존 전략일 수 있으며, 소프트웨어 벤더가 서비스 회사처럼 변해 간다는 신호일 수 있다는 위험을 짚습니다. FDE 모델의 출발점으로 Palantir를 듭니다. 분석 기관의 논평이며 실측 조사가 아닙니다. 본문 5.3.4절의 이해관계 서술은 이 글의 인용이 아니라 이 가이드의 추론입니다. (원문: [Constellation Research](https://www.constellationr.com/insights/news/forward-deployed-engineers-promise-peril-ai-deployments))
- **실패율과 손익 괴리의 외부 조사**(A3 3번, 08장 8.4절). 2025-2026년의 여러 조사가 파일럿은 많은데 손익은 움직이지 않는다는 같은 그림을 서로 다른 각도에서 보여 줍니다. S&P Global Market Intelligence(451 Research) 설문에서는 AI 이니셔티브 대부분을 폐기했다는 기업이 42%(전년 17%)로 늘었고 PoC의 46%가 프로덕션 도달 전에 접혔으며([보도](https://www.ciodive.com/news/AI-project-fail-data-SPGlobal/742590/)), IDC 조사는 PoC의 88%가 대규모 배포에 이르지 못한다고 보고했습니다([보도](https://www.cio.com/article/3850763/88-of-ai-pilots-fail-to-reach-production-but-thats-not-all-on-it.html)). McKinsey의 2026년 State of AI 조사에서는 AI 사용자의 80%가 개인 생산성 향상을 체감하는데도, EBIT의 5% 이상을 AI에 귀속시키는 고성과 기업은 6%에 그쳤습니다([원문](https://www.mckinsey.com/capabilities/quantumblack/our-insights/the-state-of-ai)). 널리 인용되는 MIT Project NANDA의 95% 수치(*The GenAI Divide: State of AI in Business 2025*, 2025-07)는 동료평가 없는 예비 연구라는 한계가 있어 방향성 참고로만 보시기 바랍니다([보도](https://finance.yahoo.com/news/mit-report-95-generative-ai-105412686.html)). **주의: 이 수치들은 모수가 전부 다릅니다.** 각각 대부분을 폐기한 기업의 비율, 프로덕션에 이르지 못한 PoC의 비율, 손익 귀속이 확인된 고성과 기업의 비율, 손익 기여가 확인되지 않은 조직의 비율입니다. 단일 AI 실패율로 합산해 인용하지 말고, 병목이 도입과 활동이 아니라 손익과의 연결에 있다는 방향성의 근거로만 쓰는 것이 정직합니다.
- **에이전트 거버넌스**(07장 7.7절). Gartner는 에이전틱(agentic) AI 프로젝트의 40% 이상이 2027년 말까지 취소될 것으로 예측했습니다(2025-06 보도자료. 사유는 비용 증가, 불명확한 사업 가치, 위험 통제의 부재). 실측이 아닌 예측치이고 표본도 자사 웨비나 참석자라는 한계가 있습니다. OWASP는 LLM 애플리케이션 Top 10에서 과잉 권한(Excessive Agency)을 상위 위험으로 올렸고, 별도의 에이전틱 애플리케이션 Top 10에서 신원과 권한의 남용을 주요 항목으로 다뤘습니다. (원문: [Gartner 보도자료](https://www.gartner.com/en/newsroom/press-releases/2025-06-25-gartner-predicts-over-40-percent-of-agentic-ai-projects-will-be-canceled-by-end-of-2027), [OWASP GenAI Security Project](https://genai.owasp.org/))
- **섀도 AI의 규모와 비용**(02장 2.6절, 07장 7.6절). 세 조사가 서로 다른 각도에서 같은 그림을 보여 줍니다. Microsoft와 LinkedIn의 *2024 Work Trend Index*(31개국 31,000명 설문)에서는 직장에서 AI를 쓰는 사람의 78%가 회사가 제공하지 않은 자기 도구를 가져와 쓴다고 답했습니다. PagerDuty의 섀도 AI 설문(2026-06, 미국, 영국, 호주, 일본의 사무직 1,250명)에서는 66%가 회사 정책에 어긋난다고 알면서도 AI 도구를 썼다고 답했습니다. IBM의 *2025 Cost of a Data Breach Report*(Ponemon Institute 조사, 600개 조직)는 섀도 AI가 관여한 침해가 전 세계 평균 침해 비용에 67만 달러를 더했고, 조직의 63%가 섀도 AI를 다룰 정책이 없다고 보고합니다. **주의: 모수가 전부 다릅니다.** 첫째는 AI 사용자 중 비율, 둘째는 사무직 응답자 중 비율, 셋째는 침해를 겪은 조직 기준의 비용과 비율입니다. 하나의 섀도 AI 비율로 합산하지 말고, 수요는 넓고 정책은 비어 있다는 방향성의 근거로만 쓰시기 바랍니다. 셋 다 벤더가 발간한 조사입니다. (원문: [Microsoft 2024 Work Trend Index](https://blogs.microsoft.com/blog/2024/05/08/microsoft-and-linkedin-release-the-2024-work-trend-index-on-the-state-of-ai-at-work/), [PagerDuty 보도자료](https://www.pagerduty.com/newsroom/shadow-ai-workplace-survey-2026/), [IBM 2025 Cost of a Data Breach](https://www.ibm.com/think/x-force/2025-cost-of-a-data-breach-navigating-ai))
- **한국 AI 기본법**(07장 7.8절). 「인공지능 발전과 신뢰 기반 조성 등에 관한 기본법」, 2026-01-22 법과 시행령 동시 시행. 고영향 AI 사업자에게 위험관리방안, 설명 방안, 사람의 관리와 감독, 문서 작성 의무를, 고영향과 생성형 AI에 이용 사실 고지와 생성물 표시 의무를 부과하며, 시행 후 최소 1년의 계도기간을 운영합니다. 일정은 [부록 A2](A2-kr-regulatory-timeline.md)를 참고하시기 바랍니다. (원문: [법제처 국가법령정보센터](https://www.law.go.kr/lsSc.do?query=인공지능+발전과+신뢰+기반+조성). 법령명으로 검색하고, 적용 전 시행령과 고시의 최신본을 확인하시기 바랍니다.)

---

[← 이전: 08 확장과 다음 단계](../docs/08-scale-and-next.md) | [목차](../README.md) | [다음: A2 한국 규제와 정책 타임라인 →](A2-kr-regulatory-timeline.md)
