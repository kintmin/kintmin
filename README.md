## 안녕하세요, Android 개발자 권오민입니다

**실기기에서 생기는 문제를 로그로 재현하고, 근본 원인까지 추적합니다.**

결제 단말(키오스크, 무인수납기) 앱, 저성능 태블릿에서 도는 병원 차팅 앱, 100시간 이상 상주하는 포그라운드 서비스를 가진 MAU 30만 헬스케어 앱을 운영해 왔습니다.<br>
전능아이티(주) 개발2팀 모바일 파트장 (2025.04 ~)

<br>

### 숫자로 보는 작업

| 항목 | 결과 | 프로젝트 |
|---|---|---|
| 사용자 인식 비정상 종료율 | **4.10% -> 0.05%**, 6개월 이상 유지 | 캐시닥 (MAU 30만 헬스케어) |
| 사용자 인식 ANR | **1.09% -> 0.02%**, 6개월 이상 유지 | 캐시닥 |
| 걸음수 누락 CS | **0건**, 로그 17종으로 원인 2가지 확인 | 캐시닥 |
| 콜드스타트 TTID | **860.5ms -> 412ms**, Macrobenchmark 측정 기반 | 캐시닥 |
| 저성능 태블릿 OOM | **메모리 peak 2곳 제거** | 스마트차트 (1,150개 병원) |
| 레거시 통신 전환 | TCP -> REST API, **배포 후 통신 관련 CS 없음** | 스마트차트 |

회사 프로젝트 코드는 비공개입니다. 문제, 원인, 해결 과정은 [포트폴리오](https://www.notion.so/35ef472e19cb809eb5f9f3c74694dbb1)에 정리해 두었습니다.

<br>

### 공개 프로젝트

| 프로젝트 | 내용 | 기술 |
|---|---|---|
| [JellyTube](https://github.com/kintmin/JellyTube) | yt-dlp 기반 음원 다운로드 및 재생 Android 앱. Python-Android 브릿지, WorkManager 연속 다운로드, KMP Desktop과 NSD 로컬 통신 | Kotlin, Compose, KMP, Ktor |
| [ibeacon_plugin](https://github.com/p-cube-plus/ibeacon_plugin) | BLE 비콘 Flutter 플러그인. Android, iOS 네이티브 코드 직접 구현 | Kotlin, Swift, Flutter |
| [Pcube+](https://github.com/p-cube-plus/p-cube-plus-application) | 동아리 출석체크 및 회비 관리 iOS/Android 앱 | Flutter |
| [Project-MetaDogs](https://github.com/kintmin/Project-MetaDogs) | 2023 제15회 창의설계경진대회 대상 (1등상). Oculus VR 손동작 전처리와 제스처 인식, ML Agent 강화학습 | Unity, C# |

<br>

### 기술

![Kotlin](https://img.shields.io/badge/Kotlin-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Android](https://img.shields.io/badge/Android-34A853?style=flat-square&logo=android&logoColor=white)
![Coroutines](https://img.shields.io/badge/Coroutines-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Jetpack Compose](https://img.shields.io/badge/Jetpack%20Compose-4285F4?style=flat-square&logo=jetpackcompose&logoColor=white)
![KMP](https://img.shields.io/badge/Kotlin%20Multiplatform-7F52FF?style=flat-square&logo=kotlin&logoColor=white)
![Flutter](https://img.shields.io/badge/Flutter-02569B?style=flat-square&logo=flutter&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub%20Actions-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Firebase](https://img.shields.io/badge/Crashlytics-DD2C00?style=flat-square&logo=firebase&logoColor=white)
![BigQuery](https://img.shields.io/badge/BigQuery-669DF6?style=flat-square&logo=googlebigquery&logoColor=white)

- 디버깅 도구: LeakCanary, Android Studio Memory Profiler, Macrobenchmark, Play Console Android Vitals
- 관심 분야: AOSP, Android Framework, HAL

<br>

### 연락

- Email: kintmin4@gmail.com
- Portfolio: [Notion](https://www.notion.so/35ef472e19cb809eb5f9f3c74694dbb1)
