# DOOM HTML (Pure HTML5 Canvas Raycaster)

"냉장고에서도 돌아가는 전설의 게임" **DOOM(1993)** 스타일의 3D 레이캐스팅 FPS 게임을 **순수 단일 HTML 파일(HTML5 + Vanilla JavaScript + CSS)** 로 구현했습니다.

외부 라이브러리(Three.js 등)나 이미지 파일 로딩 없이, 100% 브라우저 자체 캔버스와 Web Audio API로 구현되어 있어 GitHub Pages에 올리면 즉시 웹에서 실행됩니다.

---

## 🎮 주요 특징

- **단일 파일 실행 (`index.html`)**: 설치나 복잡한 빌드 과정 없이 더블 클릭만으로 바로 실행 가능
- **정통 레이캐스팅(Raycasting) 3D 엔진**: 울펜슈타인 3D 및 둠 방식의 DDA 레이캐스팅 알고리즘 적용
- **절차적 픽셀 텍스처 (Procedural Textures)**: 외부 이미지 파일 없이 코드로 직접 생성하는 레트로 벽면 텍스처 (벽돌, 돌, 악마 문양)
- **절차적 스프라이트 렌더링**: 원거리/근거리 정렬 및 카코데몬(Cacodemon) 스타일 외눈박이 악마 몬스터
- **둠 특유의 클래식 HUD**: 탄약수, 체력, 방어력, 데미지 상태에 반응하는 페이스 이모지 상태창
- **효과음 내장**: Web Audio API 신시사이저로 발사음, 타격음, 피격음 재생
- **마우스 룩(Pointer Lock) & 키보드 조작 완벽 지원**

---

## 🕹️ 조작법 (Controls)

| 키 / 동작 | 기능 |
| :--- | :--- |
| **W, S** | 앞 / 뒤로 이동 |
| **A, D** | 좌 / 우 평행이동 (스트레이프) |
| **←, →** 또는 **마우스 이동** | 시점 회전 |
| **마우스 좌클릭** 또는 **SPACE** | 샷건 발사 |
| **화면 클릭** | 마우스 조준 활성화 (Pointer Lock) |

---

## 🚀 GitHub Pages로 바로 배포하는 방법

1. GitHub에서 새로운 저장소(Repository)를 만듭니다 (예: `doom-html`).
2. 이 폴더의 `index.html` 파일을 해당 저장소에 커밋 & 푸시합니다:
   ```bash
   git init
   git add index.html README.md
   git commit -m "Initial commit: Doom HTML"
   git branch -M main
   git remote add origin https://github.com/사용자아이디/저장소이름.git
   git push -u origin main
   ```
3. GitHub 저장소의 **Settings** -> **Pages** 탭으로 이동합니다.
4. **Branch**를 `main`으로 선택하고 **Save**를 누릅니다.
5. 1~2분 뒤 생성되는 `https://<아이디>.github.io/<저장소이름>/` 주소로 접속하면 브라우저나 모바일 어디서든 바로 플레이할 수 있습니다!
