# ReviewU
- [ReviewU Install](https://github.com/apps/reviewu)
- [ReviewU Example](https://github.com/boboc-app/ReviewU-examples)

### Features
- [x] PR 기반 내용 축약
- [x] 요약 내용 포맷 개선 및 커스터마이즈 기능 (2025-02-24)
- [ ] 영문 지원
- [ ] ...

### Custom Summarize Format 
1. Root 디렉토리 경로에 `./review_u` 디렉토리 생성
2. `./review_u` 디렉토리 내부에 `SUMMARIZER_FORMAT.md`를 생성 (`.review_u/SUMMARIZER_FORMAT.md`)
3. 표현하고자 하는 형식의 포맷을 만들고, 주석 (`<!---->`)을 통해서 각 섹션에 대한 설명을 기술
4. PR을 통해서 반영된 포맷을 확인합니다. ( [예시](https://github.com/boboc-app/ReviewU-examples/blob/Customized-Review/.review_u/SUMMARIZER_FORMAT.md?plain=1)  /  [PR 요약 결과](https://github.com/boboc-app/ReviewU-examples/pull/2) )
-  [기본 포맷 예시](https://github.com/boboc-app/ReviewU-examples/pull/1)

<hr/>
## 📌 ReviewU – 자동으로 Pull Request 변경 사항 요약
ReviewU는 Pull Request의 Commit Diff와 Commit Message를 분석하여 주요 변경 사항을 자동으로 요약하는 GitHub App입니다.

### 🚀 주요 기능
자동 요약 생성: Commit Diff와 Message를 기반으로 핵심 변경 사항을 간결하게 정리 <br/>
PR 리뷰 효율화: 리뷰어가 변경 내용을 빠르게 파악할 수 있도록 요약 제공 <br/>
개발 흐름 개선: 불필요한 커밋 로그 탐색 없이, 중요한 변경 사항만 집중적으로 확인 <br/>

### 🎯 이런 분들께 추천합니다!
✔️ 여러 개의 커밋이 포함된 PR을 한눈에 파악하고 싶은 리뷰어 <br/>
✔️ 변경 사항 요약을 문서화하는 번거로움을 줄이고 싶은 개발자 <br/>
✔️ 코드 리뷰 프로세스를 효율적으로 개선하고 싶은 팀

지금 ReviewU 를 사용하여 코드 리뷰 속도를 높이고, 더 나은 협업 환경을 만들어보세요! 🚀
