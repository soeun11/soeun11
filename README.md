## 안녕하세요, iOS 개발자 임소은입니다 👋

혼자 잘하는 개발보다 팀이 함께 만들어 가는 개발을 중요하게 생각합니다. 단과학생회에서 학우들의 의견을 모으고 조율하며 소통하는 법을 배웠고, 이 경험을 바탕으로 대외 동아리에서는 팀원으로, 졸업프로젝트 pawrest에서는 개발 리드로 참여했습니다. 기획자·디자이너와 이야기하며 서비스를 만들어 왔고, 대외 동아리 데모데이에서 두 차례 수상했습니다. pawrest에서는 개발 리드로서 팀원 모두가 같은 기준으로 일할 수 있도록 컨벤션과 구조를 맞추는 데 힘썼고, 5인 팀과 함께 기획부터 App Store 출시까지 하나의 서비스를 끝까지 완성했습니다. 현재는 오류를 수정하고 기능을 보완하며 유지보수를 이어가고 있습니다.

📧 sillioud@naver.com

---

## 🛠 Tech Stack

![Swift](https://img.shields.io/badge/Swift-F05138?style=for-the-badge&logo=swift&logoColor=white)
![SwiftUI](https://img.shields.io/badge/SwiftUI-0A84FF?style=for-the-badge&logo=swift&logoColor=white)
![UIKit](https://img.shields.io/badge/UIKit-2396F3?style=for-the-badge&logo=apple&logoColor=white)
![TCA](https://img.shields.io/badge/TCA-000000?style=for-the-badge)
![Combine](https://img.shields.io/badge/Combine-5E5CE6?style=for-the-badge)
![Moya](https://img.shields.io/badge/Moya-FF6B35?style=for-the-badge)
![SnapKit](https://img.shields.io/badge/SnapKit-7B61FF?style=for-the-badge)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=for-the-badge&logo=firebase&logoColor=black)
![SwiftData](https://img.shields.io/badge/SwiftData-F05138?style=for-the-badge)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Figma](https://img.shields.io/badge/Figma-F24E1E?style=for-the-badge&logo=figma&logoColor=white)
![Photoshop](https://img.shields.io/badge/Photoshop-31A8FF?style=for-the-badge&logo=adobephotoshop&logoColor=white)
![Illustrator](https://img.shields.io/badge/Illustrator-FF9A00?style=for-the-badge&logo=adobeillustrator&logoColor=white)

- **Language**: Swift
- **UI**: SwiftUI, UIKit, SnapKit, Then
- **Architecture**: Clean Architecture, MVVM, TCA(The Composable Architecture), 모듈화
- **Data·Network**: Combine, Moya, Firebase, SwiftData, Gemini API
- **Tools**: Git, Figma, Photoshop, Illustrator

---

## 📱 Projects

### pawrest — 졸업프로젝트, 심리 상태 기록·진단 앱
`2026.02 - 현재 (출시 후 유지보수 중)` · SwiftUI · TCA · Firebase · SwiftData · Gemini · 5인 팀 · [App Store](https://apps.apple.com/kr/app/id6791101641)

- SwiftUI와 TCA 기반 App / Core / Features 구조를 설계하고, Feature별로 View·Reducer·UseCase·Service를 나눈 경량 Clean Architecture로 단방향 데이터 흐름 구성
- Service를 Firebase(Auth·Firestore·Storage) 원격 구현과 SwiftData 로컬 구현으로 분리하고 UseCase에서 통합해 로컬 캐시·오프라인·임시 저장 지원
- FactChat 게이트웨이를 통해 Gemini(Flash-Lite)를 URLSession async/await로 연동하고, 감정 기록·자가진단 기록 기반 AI 리포트와 요일별·시간대별 인사이트 생성 기능 구현
- 기록 건수에 따라 프롬프트를 분기하고 진단·단정 표현 금지, JSON 출력 형식 등 규칙을 지정했으며, 응답 파싱 실패·기록 없음에는 기본 문구로 대체하는 예외 처리 구현
- Swift Charts로 감정 변화와 리포트를 시각화하고, Lottie로 추모 화면 구성
- 공통 컴포넌트와 컬러 토큰·타이포그래피 modifier를 정리해 디자인 일관성 확보
- 이슈·브랜치·PR·커밋 컨벤션을 정리하고 xcconfig로 팀 ID 설정을 분리해 5인 팀의 Git 충돌 감소

### FLINT — SOPT 대외동아리 iOS 앱 개발
`2025.09 - 진행중` · Swift · UIKit · SnapKit · Then · Moya · Combine · 앱스토어 출시 예정 · **SOPT 데모데이 우수상**

- Clean Architecture를 Presentation / Domain / Data / Core 계층으로 구성하고, Domain의 Interface를 Data의 Repository가 구현하는 구조로 의존성 분리
- 화면(Home 등)과 공통(Components·Extensions) 단위로 Presentation을 모듈화해, 여러 기능을 오가며 작업해도 충돌하지 않는 구조에 맞춰 개발
- Moya로 네트워크 레이어(API·DTO·Error)를 추상화하고 Combine으로 비동기 처리 구성, AppDIContainer로 의존성 주입
- SnapKit과 Then으로 Auto Layout과 초기화 코드의 가독성을 확보하고, 팀 컨벤션을 준수해 협업
- 디자이너와 협의해 iOS 기본 컴포넌트를 활용하는 UI 구현 방식 조율

### Catchy — UMC 7기 iOS 파트 프로젝트
`2024.09 - 2025.02` · Swift · SwiftUI · Moya · Combine · **UMC 7th 데모데이 최우수상**

- iOS 파트로 참여해 SwiftUI로 모임 투표·일정 조율 앱의 그룹 페이지 제작
- Moya 기반 네트워크 레이어로 서버 API를 연동하고 Combine으로 그룹 관련 화면의 데이터 흐름 구현
- GitHub Issues, 브랜치 전략(main / develop / feat), PR·커밋 컨벤션에 따라 협업

---

## 🏆 Awards · Paper · Certificate

- **논문 제출** `2026.11` 펫로스 증후군 완화를 돕는 감정 기록 기반 애도 지원 모바일 앱 'Pawrest' 개발 — 한국멀티미디어학회, 공저(7인 중 3번째 저자), 심사 중
- **프로그램 저작권 등록** `2026.11` Pawrest — 컴퓨터프로그램저작물(응용프로그램), 공동저작자(5인), 등록번호 C-2026-056464, 한국저작권위원회
- **UMC 7th 데모데이 최우수상** — Catchy 프로젝트 (iOS 파트)
- **SOPT 데모데이 우수상** — FLINT 프로젝트 (iOS 개발)
- **GTQ 그래픽기술자격 1급** `2022.04` 한국생산성본부

---

## 🎓 Education & Activity

- **서울여자대학교 디지털미디어학과** (제2전공 디지털융합경영) `2022.02 - 재학 중 (2027 졸업 예정)`
- **미래산업융합대학 단과학생회 정보국원** `2022.02 - 2023.01`
