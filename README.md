# GIGAette Mongolia Heating Simulator

> 몽골 체체를렉 IsoTES 난방 사업성 인터랙티브 시뮬레이터
> Mongolia Tsetserleg IsoTES Heating Business Viability Interactive Simulator

**라이브 데모 / Live demo**: https://ikjejang-gigaette.github.io/heating-simulator/

---

## 개요 (Korean)

GIGAette의 IsoTES(Isobaric Thermal Energy Storage) 시스템을 몽골 체체를렉 신도시 난방에 적용했을 때의 경제성을, 4가지 기술(갈탄 보일러, IsoTES + 그리드 전기, 태양광 PV + IsoTES, 태양열 ETC + IsoTES)로 비교 시뮬레이션하는 단일 HTML 파일입니다.

### 주요 기능

- **Tier 1/2/3 슬라이더** (총 36개): 심야할인·탄소가격·할인율·CAPEX 세부 등 실시간 조작
- **4기술 비교**: LCOH·NPV·회수기간·CO₂ 절감을 표·차트로 동시 비교
- **14개 시나리오 프리셋**: PoC 기본·스케일업 100/500MWh·탄소 $15~$150·ETC 보수/낙관 등
- **2개 운영 모드**: PoC (1.5 MWh 시범) / 스케일업 (50~500 MWh 상업화)
- **3개 통화 토글**: USD / MNT / KRW
- **2개 언어 토글**: 한국어 / English
- **검증 모드**: Excel SSoT(`heating_business_model_v1.xlsx` v1.3, 127 수식)와 5% 허용 오차 내 일치 자동 검증
- **PDF 출력**: 브라우저 인쇄 → IR/ODA용 한 페이지 자료

### 사용법

1. **온라인**: 위 라이브 데모 URL 접속
2. **오프라인**: `index.html` 다운로드 후 더블클릭 (Chart.js·Alpine.js는 CDN 로드, 인터넷 필요)
3. **완전 오프라인**: CDN 두 줄을 같은 폴더에 다운로드 후 HTML의 `script src` 경로 변경

### 기술 스택

- **Frontend**: Vanilla HTML + CSS Grid + Alpine.js 3.x (인라인 ~15KB) + Chart.js 4.x (CDN)
- **계산 엔진**: 순수 JS, USD 기준 내부 계산 → 표시 직전 환율 적용
- **데이터 SSoT**: Excel 모델 (사내 보관)

---

## Overview (English)

A single-file HTML simulator comparing the economic viability of GIGAette's IsoTES (Isobaric Thermal Energy Storage) system applied to district heating in Tsetserleg, Mongolia, against three alternatives: lignite coal boiler, Solar PV + IsoTES, and Solar ETC + IsoTES.

### Features

- **36 sliders across 3 tiers**: night discount, carbon price, discount rate, CAPEX components
- **4-technology comparison**: LCOH, NPV, payback, CO₂ savings shown side-by-side
- **14 scenario presets**: PoC baseline, scale-up 100/500MWh, carbon $15~$150, ETC conservative/optimistic
- **2 operating modes**: PoC (1.5 MWh pilot) / Scale-up (50~500 MWh commercial)
- **3 currency toggles**: USD / MNT / KRW
- **Bilingual UI**: Korean / English
- **Verification mode**: validates JS computation against Excel SSoT within 5% tolerance
- **PDF export**: browser print → one-page IR/ODA collateral

### Usage

1. **Online**: visit live demo URL above
2. **Offline**: download `index.html` and double-click (Chart.js/Alpine.js loaded via CDN)
3. **Fully offline**: download both CDN files locally and update `<script src>` paths

---

## 데이터 출처 / Data Sources

- KOICA CTS Seed 1 모니터링 보고서 (2025)
- KOICA CTS Seed 1 탄소배출량 감소율 모니터링 보고서 (2024)
- USEA 2020 (갈탄 보일러 효율)
- IRENA (시스템 수명)
- World Bank 사회할인율 (6%)
- UNESCAP (운송 단가)

## 라이선스 / License

© 2026 GIGAette Co., Ltd. All rights reserved.
See [LICENSE](LICENSE) for details.

## 문의 / Contact

기술 문의·버그 리포트: GIGAette 기술팀
For technical inquiries and bug reports: GIGAette technical team
