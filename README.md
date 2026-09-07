# py_nesting
A Python-based 2D sheet nesting algorithm to minimize material loss in furniture manufacturing.
가구 설계를 위한 표준 판재(4×8) 2D Nesting 및 자재 로스율 최적화 파이썬 스크립트

`py_nesting`은 가구 설계 과정에서 발생할 수 있는 원목 및 합판 자재의 버림 비율(Loss Rate)을 줄이고, 표준 판재 재단 배치를 최적화하기 위해 독학 및 연구 중인 파이썬 프로젝트입니다.

---

## 📌 프로젝트 배경 (Motivation)

가구 설계 실무에서는 제작 비용 절감과 자재 효율성이 중요합니다.  
본 프로젝트는 **2D/3D CAD 도면 작성 단계에서 산출된 부품 치수를 바탕으로 판재(4×8, 1220×2440mm) 재단 효율성을 사전에 검증하고, HTML/SVG 리포트를 통해 직관적으로 시각화하는 자동화 알고리즘**을 구현하는 것을 목표로 합니다.

---

## 🛠 주요 기능 및 학습 목표 (Features & Goals)

- [x] **표준 판재 및 부품 규격 설정**: 4×8 판재 및 각 부품의 2D 가로·세로 치수 데이터 구조화
- [ ] **2D Nesting 배치 알고리즘 구현**: 자재 효율성을 극대화하는 부품 정렬 및 배치 시도 (학습 진행 중)
- [ ] **HTML/SVG 기반 결과 시각화**: 웹 브라우저에서 확인할 수 있는 2D 자재 배치 리포트(`.html`) 자동 생성
- [ ] **목취율 및 로스율 자동 산출**: 전체 자재 대비 실제 사용 면적 계산 및 리포트 상단 표시
- [ ] **CAD 데이터 연동 (향후 목표)**: `.dxf` 파일 내 치수 데이터 추출 및 BOM(부품명세서) 자동 연동 연구

---

## 💻 기술 스택 (Tech Stack)

- **Language:** Python 3.x
- **IDE:** Visual Studio Code
- **Visualization:** HTML5, CSS3, SVG (웹 브라우저 기반 인터랙티브 배치도 시각화)
- **Libraries (예정):** `ezdxf` (CAD 연동 검토), `Jinja2` (HTML 리포트 템플릿 생성 검토)

---

## 📂 프로젝트 구조 (Project Structure)

```text
py_nesting/
├── README.md
├── main.py              # 메인 실행 파일
├── nesting_calc.py      # 목취율 및 로스율 계산 알고리즘 모듈
├── html_render.py       # HTML/SVG 시각화 리포트 생성 모듈
├── data/
│   └── sample_parts.json # 가구 부품 치수 샘플 데이터
└── output/
    └── result.html      # 생성된 시각화 결과 파일 (웹 브라우저 실행)
