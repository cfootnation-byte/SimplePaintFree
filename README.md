<p align="center">
  <img src="https://simplepaint.pages.dev/favicon.ico" width="80" />
</p>

<h1 align="center">SimplePaint</h1>

<p align="center">
  AI 기반 일러스트 & 웹툰 어시스턴트 툴
</p>

<p align="center">
  <img src="https://img.shields.io/badge/version-1.0.0-blue" alt="Version" />
  <img src="https://img.shields.io/badge/platform-Windows%2010%2B-0078D6?logo=windows" alt="Platform" />
  <img src="https://img.shields.io/badge/license-Proprietary-red" alt="License" />
  <img src="https://img.shields.io/badge/Qt-6.7-41CD52?logo=qt" alt="Qt" />
</p>

<p align="center">
  <b>한국어</b> | <a href="docs/README_en.md">English</a> | <a href="docs/README_ja.md">日本語</a>
</p>

---

<p align="center">
  <video src="media/demo.mp4" width="720" controls></video>
</p>

## 소개

SimplePaint는 선화부터 채색, 명암까지 AI가 자동화하는 일러스트 & 웹툰 제작 도구입니다.
사용자 본인의 API 키(Gemini, Flux)를 사용하여 AI 기능을 무료로 이용할 수 있습니다.

---

## AI 기능

### 1. 명암 생성 (AI Shading)

선화 레이어에서 자동으로 셀셰이딩을 생성합니다. 광원 방향과 강도를 자동으로 분석하여 자연스러운 명암을 만들어냅니다.

**사용 방법:**
1. 선화 레이어 선택
2. 상단 메뉴에서 [AI] → [명암 생성] 클릭
3. 옵션 선택: 하드 셀셰이딩 / 소프트 셰이딩 / 3톤 셀셰이딩
4. 생성 버튼 클릭

### 2. 밑색 생성 (AI Colorize)

선화에 자동으로 플랫 컬러링을 적용합니다. 캐릭터 시트를 참조하여 일관된 색상을 유지할 수 있습니다.

**사용 방법:**
1. 선화 레이어 선택
2. [AI] → [밑색 생성] 선택
3. (선택사항) 캐릭터 시트 파일 지정
4. 자동 채색 실행

### 3. 캐릭터 시트 생성

참조 이미지로부터 턴어라운드 캐릭터 시트를 자동 생성합니다. 정면, 측면, 후면, 클로즈업 4가지 뷰를 제공합니다.

**사용 방법:**
1. [AI] → [캐릭터 시트 생성] 선택
2. 참조 이미지 업로드 (정면 또는 3/4 앵글 권장)
3. 생성할 뷰 선택 (정면/측면/후면/클로즈업)
4. 생성 실행

### 4. 선화 생성 (AI Line Art)

캐릭터 시트를 기반으로 새로운 포즈의 선화를 생성합니다. 클린 선화, 자연스러운 펜선, 스케치풍 중 선택 가능합니다.

**사용 방법:**
1. 캐릭터 시트 로드
2. [AI] → [선화 생성] 선택
3. 원하는 포즈 프롬프트 입력 (예: "앉아있는 포즈")
4. 선화 스타일 선택
5. 생성 실행

### 5. 영역 분리 (AI Segmentation)

이미지를 의미 있는 단위로 자동 분리하여 각각 별도의 레이어로 만듭니다.

**사용 방법:**
1. 분리할 레이어 선택
2. [AI] → [영역 분리] 선택
3. 분리할 요소 입력 (예: "인물, 배경, 소품")
4. 자동 분리 실행

### 6. 명암색 변환 (Shading Color Swap)

회색 톤의 명암을 원하는 컬러로 변환하여 다양한 분위기를 연출할 수 있습니다. AI가 아닌 내부 변환이므로 API 키가 필요하지 않습니다.

**사용 방법:**
1. 명암 레이어 선택
2. [AI] → [명암색 변환] 선택
3. 변환할 색상 선택 (컬러 피커)
4. 적용 버튼 클릭

---

## 인터페이스 & 기본 기능

### 메뉴 바

**File 메뉴**
- **Save Project (Ctrl+S):** 현재 작업을 프로젝트 파일로 저장합니다. 레이어 구조가 그대로 유지됩니다.
- **Open Project (Ctrl+O):** 저장된 프로젝트 파일을 불러옵니다.
- **Export Image (Ctrl+E):** 현재 캔버스를 이미지 파일(PNG 등)로 내보냅니다.
- **Import Image to Layer:** 외부 이미지 파일을 새 레이어로 가져옵니다.
- **Import PSD (Ctrl+Shift+O):** Photoshop PSD 파일을 레이어 구조 그대로 불러옵니다.
- **Export as PSD (Ctrl+Shift+S):** 현재 작업을 PSD 파일로 내보냅니다.
- **Exit (Ctrl+Q):** 프로그램을 종료합니다.

**Edit 메뉴**
- **Undo (Ctrl+Z):** 마지막 작업을 되돌립니다.
- **Redo (Ctrl+Y):** 되돌린 작업을 다시 실행합니다.
- **Free Transform (Ctrl+T):** 선택된 레이어를 자유 변형합니다. 크기 조절, 회전, 이동이 가능합니다.
- **Canvas Size:** 캔버스의 크기를 변경합니다.
- **AI Variations:** AI를 사용하여 현재 이미지의 변형(배리에이션)을 생성합니다.
- **Clear Layer:** 현재 선택된 레이어의 내용을 전부 지웁니다.

**View 메뉴**
- **Zoom In (Ctrl++):** 캔버스를 확대합니다.
- **Zoom Out (Ctrl+-):** 캔버스를 축소합니다.
- **Reset Zoom (Ctrl+0):** 캔버스를 기본 배율(100%)로 초기화합니다.
- **Show Grid:** 캔버스에 그리드를 표시하거나 숨깁니다.

### 도구 바 (Toolbar)

- **Undo / Redo (Ctrl+Z / Ctrl+Y):** 작업을 되돌리거나 다시 실행합니다.
- **Save / Load:** 현재 캔버스를 이미지 파일로 저장하거나, 이미지 파일을 불러옵니다.
- **Color:** 그리기에 사용할 색상을 선택합니다. 기본 4색이 제공되며, 클릭하여 커스텀 색상을 선택할 수 있습니다.
- **Eraser:** 지우개 모드를 켜거나 끕니다.
- **Clear:** 현재 선택된 레이어의 내용을 전부 지웁니다.
- **Brush Size:** 브러시(펜/지우개)의 크기를 조절합니다.
- **Zoom:** 캔버스의 확대/축소 비율을 조절합니다.

### 레이어 시스템

**레이어 설정**
- **블렌드 모드:** 레이어 패널 상단의 드롭다운에서 블렌드 모드를 선택할 수 있습니다. 14종 지원.
- **불투명도 (Opacity):** 슬라이더로 레이어의 불투명도를 0%~100% 사이에서 조절합니다.

**레이어 관리**
- **+Layer:** 새로운 빈 레이어를 추가합니다.
- **+Folder:** 레이어를 그룹으로 묶을 수 있는 폴더를 추가합니다.
- **Delete:** 선택된 레이어 또는 폴더를 삭제합니다.
- **Up / Down:** 선택된 레이어의 순서를 한 단계 위 또는 아래로 이동시킵니다.
- **Show / Hide:** 선택된 레이어를 숨기거나 다시 표시합니다.

**고급 기능**
- **+Mask:** 선택된 레이어에 마스크를 추가합니다.
- **-Mask:** 선택된 레이어의 마스크를 삭제합니다.
- **Edit Mask:** 마스크 편집 모드에 진입합니다. 지우개로 영역을 지우면 해당 부분이 마스킹됩니다. 편집이 끝나면 Edit Mask 버튼을 다시 눌러 비활성화합니다.
- **Clip:** 선택된 레이어를 아래 레이어에 클리핑합니다. 아래 레이어에서 색칠된 영역 안에서만 현재 레이어가 보이게 됩니다.

### 블렌드 모드 (14종)

| 그룹 | 모드 |
|------|------|
| 어둡게 | Normal, Darken, Multiply, Color Burn, Linear Burn |
| 밝게 | Lighten, Screen, Color Dodge, Add (Linear Dodge) |
| 대비 | Overlay, Soft Light, Hard Light |
| 차이 | Difference, Exclusion |

---

## API 키 설정

SimplePaint Free는 사용자 본인의 API 키를 사용합니다. AI 기능을 사용하려면 다음 API 키가 필요합니다:

| API | 용도 | 발급처 |
|-----|------|--------|
| Flux (BFL) | 명암 생성, 밑색 생성, 선화 생성 | [Black Forest Labs](https://api.bfl.ml/) |
| Gemini (Google) | 캐릭터 시트 생성, 영역 분리, 색상 분석 | [Google AI Studio](https://aistudio.google.com/) |

앱 실행 후 **설정 → API Settings**에서 키를 입력하면 됩니다.

---

## 시스템 요구사항

| | 최소 사양 | 권장 사양 |
|---|----------|----------|
| OS | Windows 10 (64-bit) | Windows 11 (64-bit) |
| CPU | Intel i5 | Intel i7 |
| RAM | 8GB | 16GB+ |
| GPU | 2GB VRAM | 4GB VRAM (NVIDIA) |
| Storage | 5GB | 10GB |

---

## 설치

1. [Releases](../../releases) 페이지에서 최신 인스톨러를 다운로드합니다.
2. 다운로드한 설치 파일을 실행합니다.
3. 설치 마법사의 안내를 따라 설치를 완료합니다.
4. SimplePaint를 실행하고 API 키를 설정합니다.

---

## 라이선스

Copyright (c) 2026 SimplePaint. All rights reserved.

이 소프트웨어는 독점 소프트웨어(Proprietary Software)입니다.
소스 코드는 공개되지 않으며, 인스톨러를 통한 사용만 허가됩니다.
무단 복제, 수정 및 재배포는 금지됩니다.
