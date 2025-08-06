# Mini Trackball Keyboard

PWM3610 트랙볼, EC11 인코더, 스위치 2개로 구성된 간단한 커스텀 키보드입니다.

## 하드웨어 구성

- **MCU**: Nice!nano v2
- **트랙볼**: PWM3610 (SPI)
- **인코더**: EC11 (회전 + 푸시)
- **스위치**: 2개 (MX 호환)
- **연결**: Bluetooth LE + USB-C

## 기능

- **트랙볼**: 마우스 커서 제어
- **스위치 1**: 왼쪽 클릭
- **스위치 2**: 오른쪽 클릭
- **인코더**: 위/아래 스크롤
- **인코더 푸시**: 추가 기능 (설정 가능)
- 무선 연결
- RGB 백라이트 (선택사항)

## 키맵

### 기본 레이어

- 스위치 1: 왼쪽 클릭
- 스위치 2: 오른쪽 클릭
- 인코더 CW: 스크롤 위
- 인코더 CCW: 스크롤 아래

### 레이어 1 (함수 레이어)

- 스위치 1: Bluetooth 프로필 0 선택
- 스위치 2: Bluetooth 프로필 1 선택

## 파일 구조

```
mini-trackball-keyboard/
├── README.md
├── config/
│   ├── mini-trackball.zmk.yml
│   ├── mini-trackball.keymap
│   ├── mini-trackball.overlay
│   └── west.yml
├── pcb/
│   ├── mini-trackball.kicad_pcb
│   ├── mini-trackball.kicad_sch
│   └── gerber/
├── case/
│   ├── top.stl
│   ├── bottom.stl
│   └── trackball_holder.stl
└── bom/
    └── components.csv
```

## 빌드 및 플래시

1. ZMK 설정을 GitHub에 푸시
2. GitHub Actions를 통해 펌웨어 자동 빌드
3. 다운로드한 펌웨어를 키보드에 플래시

## 라이센스

MIT License
