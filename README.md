# CommandX

<p align="center">
    <img src="assets/AppIcon.svg" width="128" height="128" alt="CommandX 앱 아이콘">
</p>

<h3 align="center">Mac에서도 파일 이동은 Command-X, Command-V.</h3>

<p align="center">
    CommandX는 macOS Finder에 익숙한 잘라내기와 붙여넣기 흐름을 더해주는 작은 메뉴 막대 앱입니다.<br>
    파일을 선택하고 <code>Command-X</code>, 이동할 폴더에서 <code>Command-V</code>. 이제 세 개의 키를 누르지 않아도 됩니다.
</p>

<p align="center">
    <strong><a href="https://github.com/dongkkase/CommandX/releases/latest">최신 버전 다운로드</a></strong>
    ·
    <a href="#설치">설치 방법</a>
    ·
    <a href="https://github.com/dongkkase/CommandX/issues/new/choose">문제 신고</a>
</p>

> 이 저장소는 CommandX의 소개, 사용자 안내, 지원 및 Release 다운로드를 위한 공개 저장소입니다. 실제 앱 소스 코드는 포함하지 않습니다. GitHub가 자동으로 표시하는 `Source code (zip)`과 `Source code (tar.gz)`는 설치 파일이 아닙니다. Release의 Assets에서 `CommandX-<버전>-macOS.zip`을 다운로드하세요.

## Finder의 방식은 그대로, 단축키만 익숙하게

macOS에서 파일을 이동하려면 보통 복사한 뒤 `Option-Command-V`를 눌러야 합니다. CommandX는 이 동작을 Windows와 여러 파일 관리자에서 익숙한 `Command-X`, `Command-V` 흐름으로 바꿔줍니다.

- **바로 익숙해지는 단축키**: 파일이나 폴더를 `Command-X`로 잘라내고 `Command-V`로 이동합니다.
- **붙여넣기 전까지 원본 유지**: 잘라내는 순간에는 파일을 삭제하거나 이동하지 않습니다.
- **Finder가 직접 이동 처리**: 붙여넣을 때 Finder의 기본 이동 명령을 사용합니다.
- **텍스트 편집은 그대로**: Finder에서 파일명을 바꾸거나 검색어를 입력할 때는 원래의 텍스트 잘라내기가 동작합니다.
- **필요한 곳에서만 동작**: Finder가 전면에 있을 때만 파일 이동 단축키를 처리합니다.

이름 충돌, 이동 진행률, 외장 디스크, 클라우드 파일과 실행 취소는 기존과 같이 Finder가 담당합니다. CommandX는 Finder를 대신하는 파일 관리자가 아니라, 자주 쓰는 이동 동작을 더 간결하게 만드는 도구입니다.

## 사용법

1. Finder에서 이동할 파일 또는 폴더를 선택합니다.
2. `Command-X`를 눌러 이동 대기 상태로 만듭니다.
3. 대상 폴더를 엽니다.
4. `Command-V`를 누르면 Finder가 파일을 이동합니다.

`Esc`를 누르면 이동 대기를 취소할 수 있습니다. 다른 복사 동작으로 클립보드가 바뀐 경우에도 이전 파일이 잘못 이동하지 않도록 대기 상태가 자동으로 취소됩니다.

## 이런 분에게 잘 맞습니다

- Windows에서 Mac으로 옮겨와 파일 잘라내기 단축키가 아쉬운 분
- Finder에서 파일과 폴더를 자주 정리하는 분
- `Option-Command-V` 대신 더 단순하고 기억하기 쉬운 흐름을 원하는 분
- Finder의 기본 동작을 유지하면서 단축키만 바꾸고 싶은 분

## 핵심 설정

- **로그인 시 실행**: Mac을 켤 때 CommandX를 자동으로 시작합니다.
- **메뉴 막대 아이콘 숨기기**: 설정을 마친 뒤 메뉴 막대를 더 간결하게 유지합니다.
- **Command-X 안정 처리 모드**: Finder 복사 후 클립보드 변경이 잠시 안정된 뒤 이동 대기 상태로 전환합니다.

메뉴 막대 아이콘을 숨긴 뒤에는 CommandX를 다시 실행하거나 `Option-Command-X`를 눌러 설정을 열 수 있습니다.

## 시스템 요구 사항

- macOS 13 Ventura 이상
- Apple Silicon 또는 Intel Mac
- 손쉬운 사용 및 단축키 전송 권한

## 설치

1. [CommandX Releases](https://github.com/dongkkase/CommandX/releases)에서 최신 `CommandX-<버전>-macOS.zip`을 다운로드합니다.
2. ZIP의 압축을 풉니다.
3. `CommandX.app`을 `/Applications` 폴더로 옮깁니다.
4. `/Applications/CommandX.app`을 실행합니다.
5. 앱의 안내에 따라 손쉬운 사용 및 단축키 전송 권한을 허용합니다.

Release의 macOS ZIP은 Apple Silicon과 Intel Mac을 모두 지원하는 Universal 앱으로 제공됩니다. 공식 ZIP을 설치했는데도 macOS가 개발자를 확인할 수 없다고 표시하면 보안 설정을 우회하지 말고 파일을 다시 다운로드하거나 [Issue를 등록](https://github.com/dongkkase/CommandX/issues/new/choose)해 주세요.

권한과 파일 이동 테스트에는 Release Assets의 Developer ID 서명·공증 ZIP만 사용하세요. 소스에서 직접 만든 Debug, Local Release 또는 Unsigned Test 빌드는 정식 앱과 다른 식별자를 사용하며 `/Applications` 설치용이 아닙니다.

**[CommandX 최신 버전 다운로드](https://github.com/dongkkase/CommandX/releases/latest)**

## 권한 문제 해결

CommandX는 Finder의 단축키를 감지하고 Finder에 이동 명령을 전달하기 위해 macOS의 손쉬운 사용 권한이 필요합니다. 단축키가 동작하지 않으면 다음 순서로 확인해 주세요.

1. CommandX 설정에서 현재 권한 안내를 확인합니다.
2. 손쉬운 사용을 허용하면 단축키 전송 권한 요청이 이어집니다. 별도 안내가 남아 있으면 `권한 적용 완료`를 누릅니다.
3. `시스템 설정 > 개인정보 보호 및 보안 > 손쉬운 사용`에서 CommandX를 껐다가 다시 켭니다.
4. 계속 동작하지 않으면 기존 CommandX 항목을 제거하고 `/Applications/CommandX.app`을 다시 추가합니다.
5. CommandX를 완전히 종료한 뒤 `/Applications/CommandX.app`을 다시 실행합니다.

여러 위치에 CommandX를 복사해 실행하면 macOS가 서로 다른 앱으로 인식할 수 있습니다. `/Applications/CommandX.app` 한 복사본만 사용하는 것을 권장합니다.

## 업데이트와 삭제

현재 자동 업데이트는 제공하지 않습니다. 설정 화면의 `릴리즈 확인` 또는 [Releases 페이지](https://github.com/dongkkase/CommandX/releases)에서 새 버전을 다운로드한 뒤 기존 `/Applications/CommandX.app`을 교체해 주세요.

앱을 삭제하려면 먼저 `로그인 시 실행`을 끄고 CommandX를 종료한 다음 `/Applications/CommandX.app`을 삭제합니다.

## 개인정보 보호와 알려진 제한

- 계정, 광고, 분석 도구 또는 앱 자체의 네트워크 전송 기능이 없습니다.
- 파일명, 파일 경로, 클립보드 내용 및 키 입력을 디스크에 저장하거나 외부로 전송하지 않습니다.
- Finder가 전면에 있고 텍스트를 편집하지 않을 때만 파일 이동 단축키를 변환합니다.
- 파일명 변경 또는 Finder 검색 입력 중에는 원래 텍스트 잘라내기가 동작합니다.
- 외장 디스크, 네트워크 볼륨 또는 클라우드 간 이동은 Finder가 처리하므로 시간이 걸리거나 Finder 오류가 나타날 수 있습니다.
- 다른 클립보드 앱이 복사 내용을 변경하면 이동 대기가 취소됩니다.

자세한 내용은 [개인정보 보호 안내](PRIVACY.md)를 확인하세요.

## 지원

문제가 있으면 [지원 안내](SUPPORT.md)를 먼저 확인해 주세요. 해결되지 않으면 공개 저장소에 [Issue를 등록](https://github.com/dongkkase/CommandX/issues/new/choose)할 수 있습니다.

문제를 제보할 때는 macOS 버전, Mac 종류와 재현 순서를 알려주시면 확인에 도움이 됩니다. 개인 파일명이나 전체 파일 경로는 포함하지 마세요.

## English

**Cut and move files on your Mac with the shortcuts you already know.**

CommandX is a lightweight macOS 13+ menu bar app that brings the familiar `Command-X`, `Command-V` file-moving flow to Finder. Cutting does not delete or move anything immediately. When you paste, CommandX asks Finder to perform its native move operation, so Finder continues to handle progress, name conflicts, external drives, cloud files, and Undo.

CommandX only handles file shortcuts when Finder is active and leaves normal text cutting intact while renaming files or typing in Finder search. You can cancel a pending move with `Esc`, launch the app at login, hide its menu bar icon, and enable reliable handling that waits for Finder to confirm the copy operation.

Download `CommandX-<version>-macOS.zip` from the [latest Release](https://github.com/dongkkase/CommandX/releases/latest), extract it, move `CommandX.app` to `/Applications`, and grant the requested Accessibility and shortcut delivery permissions.

This public repository contains product documentation, support, and release downloads only. It does not contain the app source code. GitHub's automatically generated source archives are not the macOS app; download the macOS ZIP from the Release Assets section.
