# CommandX 개인정보 보호 안내

최종 수정일: 2026-08-30

CommandX는 Finder의 파일 이동 단축키를 제공하기 위해 필요한 정보만 기기 안에서 처리합니다.

## 수집하거나 전송하지 않는 정보

- 사용자 계정 또는 식별자
- 분석, 광고 또는 사용 통계
- 파일명과 파일 경로
- 클립보드 내용
- 키 입력 기록
- 충돌 보고서 또는 진단 정보

CommandX 앱 자체는 서버에 네트워크 요청을 보내지 않습니다. 설정 화면의 Release 또는 Issue 링크를 선택하면 사용자의 기본 웹 브라우저가 GitHub를 엽니다.

## 기기 안에서 처리하는 정보

- Finder가 전면에 있는지 확인합니다.
- `Command-X`, `Command-V`, `Esc`와 설정 복구 단축키를 구분하기 위해 키보드 이벤트를 메모리에서 평가합니다.
- Finder가 복사한 파일 URL과 Finder pasteboard 정보를 짧은 이동 대기 시간 동안 메모리에서 검증합니다.
- 로그인 실행, 메뉴 막대 아이콘, 안정 처리 모드와 같은 설정값만 macOS UserDefaults에 저장합니다.

키보드 이벤트, 파일 URL과 클립보드 내용은 디스크에 기록하거나 외부로 전송하지 않습니다.

## 권한

CommandX는 Finder 단축키를 감지하고 Finder에 기본 복사·이동 명령을 전달하기 위해 macOS의 손쉬운 사용 및 단축키 전송 권한을 사용합니다. 권한은 `시스템 설정 > 개인정보 보호 및 보안`에서 언제든지 철회할 수 있습니다.

## 문의

개인정보 관련 문의는 [공개 Issue](https://github.com/dongkkase/CommandX/issues/new/choose)로 접수할 수 있습니다. Issue에 개인 파일명이나 전체 파일 경로를 첨부하지 마세요.

## English summary

CommandX does not collect analytics, account data, file paths, clipboard contents, or keystroke logs, and it does not transmit app data over the network. Shortcut and Finder pasteboard information is evaluated in memory only. The app persists only its user settings in macOS UserDefaults.
