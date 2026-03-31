# Glacier Utility

브라우저에서 바로 이미지를 리사이즈, 변환, 압축할 수 있는 정적 웹 앱입니다.  
서버 업로드 없이 모든 처리가 클라이언트(Canvas API)에서 이루어집니다.

🔗 **[https://blackwood1987.github.io/ImageResizely/](https://blackwood1987.github.io/ImageResizely/)**

## 주요 기능

- **리사이즈** — 가로/세로 픽셀 직접 입력, 비율 고정 토글
- **포맷 변환** — WebP, PNG, JPG, AVIF 지원
- **품질 조절** — 슬라이더로 출력 품질 설정 (PNG 무손실 자동 처리)
- **드래그 앤 드롭** — 파일 드롭 또는 클릭 업로드
- **결과 비교** — 원본 vs 처리 결과 나란히 표시, 용량 절감률 표시

## 파일 구조

```
index.html   # 데스크톱 레이아웃
mobile.html  # 모바일 레이아웃
```

## 기술 스택

- Tailwind CSS (CDN)
- Google Fonts — Inter, Material Symbols Outlined
- Canvas API / File API / Blob URL
- GitHub Pages 배포 (빌드 단계 없음)
