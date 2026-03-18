# HWPX 파일 병합 도구 (PyQt5)

이 프로그램은 여러 개의 HWPX 파일을 선택하여 하나의 파일로 병합해주는 도구입니다.

## 주요 기능
- **여러 파일 선택**: 병합할 HWPX 파일을 한꺼번에 선택할 수 있습니다.
- **순서 변경**: 리스트에서 드래그 앤 드롭으로 병합 순서를 바꿀 수 있습니다.
- **자동 병합**: 한컴오피스 Automation API를 사용하여 서식과 내용을 정확하게 병합합니다.

## 실행 환경 및 주의사항
- **한컴오피스 필수**: 이 프로그램은 한컴오피스(HWP)의 기능을 직접 제어하므로, **실행하는 PC에 한컴오피스가 설치되어 있어야 합니다.**
- **Windows 전용**: 한컴오피스 API(win32com)를 사용하므로 Windows 환경에서만 작동합니다.

## GitHub Actions 빌드 (PyInstaller)
이 프로젝트는 GitHub Actions를 통해 자동으로 실행 파일(`.exe`)을 생성하도록 설정되어 있습니다.

1. 이 저장소를 GitHub에 푸시합니다.
2. GitHub 저장소의 **Actions** 탭으로 이동합니다.
3. 가장 최근의 워크플로우 실행을 클릭합니다.
4. 하단의 **Artifacts** 섹션에서 `HwpxMerger-Executable`을 다운로드합니다.
5. 압축을 풀고 `HwpxMerger.exe`를 실행합니다.

## 로컬에서 실행하기 (Python)
1. 의존성 설치:
   ```bash
   pip install -r requirements.txt
   ```
2. 프로그램 실행:
   ```bash
   python main.py
   ```
