<h1 align="center">DO-ST</h1>

<p align="center">
  Flutter 기반 크로스플랫폼 앱 프로젝트
</p>

<p align="center">
  <img alt="Flutter" src="https://img.shields.io/badge/Flutter-stable-02569B?style=flat-square&logo=flutter&logoColor=white&labelColor=24292F" />
  <img alt="Dart" src="https://img.shields.io/badge/Dart-%5E3.7.2-0175C2?style=flat-square&logo=dart&logoColor=white&labelColor=24292F" />
  <img alt="Platforms" src="https://img.shields.io/badge/Platforms-Android_·_iOS_·_Web_·_Desktop-6B7280?style=flat-square&labelColor=24292F" />
  <img alt="Status" src="https://img.shields.io/badge/Status-Initial_setup-F59E0B?style=flat-square&labelColor=24292F" />
</p>

<br />

> [!NOTE]
> 지금은 `flutter create`로 만든 **초기 세팅 단계**입니다.
> `lib/main.dart`에는 Flutter 기본 카운터 예제만 있고, 앱 기능은 아직 구현 전입니다.

<br />

## 지원 플랫폼

모든 플랫폼 폴더가 생성되어 있어, 한 코드베이스로 아래 타깃을 빌드할 수 있습니다.

| Android | iOS | Web | macOS | Windows | Linux |
| :-: | :-: | :-: | :-: | :-: | :-: |
| ✓ | ✓ | ✓ | ✓ | ✓ | ✓ |

<br />

## 프로젝트 구조

Flutter 프로젝트는 저장소 루트가 아닌 `ourapp/` 폴더에 있습니다.

```
DO-ST
└── ourapp/
    ├── lib/
    │   └── main.dart          # 앱 진입점 (현재 기본 카운터 예제)
    ├── test/
    │   └── widget_test.dart   # 기본 위젯 테스트
    ├── android/  ios/  web/   # 모바일 · 웹 플랫폼 설정
    ├── macos/  windows/  linux/
    ├── analysis_options.yaml  # flutter_lints 규칙
    └── pubspec.yaml           # 패키지 · SDK 설정
```

<br />

## 시작하기

**요구 사항:** Dart 3.7.2 이상(4.0 미만)을 포함한 Flutter SDK

```bash
cd ourapp
flutter pub get
flutter run            # 연결된 기기 또는 에뮬레이터에서 실행
```

```bash
flutter run -d chrome  # 웹으로 실행
flutter test           # 테스트 실행
```

<br />

## 개발 환경

| 항목 | 값 |
| :-- | :-- |
| Dart SDK | `^3.7.2` |
| 린트 | `flutter_lints ^5.0.0` |
| Android | AGP 8.7.0 · Kotlin 1.8.22 · Gradle 8.10.2 · Java 11 |
| iOS / macOS | 최소 iOS 12.0 · macOS 10.14 |
| 패키지 ID | `com.example.ourapp` |

<br />

## 다음 단계

- [ ] 앱 이름과 패키지 ID(`com.example.ourapp`)를 고유한 값으로 변경
- [ ] Android 릴리스 서명 설정 (현재 debug 키로 서명)
- [ ] 기본 카운터 화면을 실제 서비스 화면으로 교체
- [ ] 서비스 소개와 화면 구성을 README에 추가
