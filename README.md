# POLIS 2.0 — 세계 총선 시뮬레이터

GitHub Pages에서 별도 서버 없이 실행하는 의회·총선 가상 게임입니다.

플레이: https://saucepark060323-creator.github.io/polis-election-simulator/

## 메뉴
- **홈:** 국가 선택, 바로 개표, 공약·선거운동, 가상 개표 결과
- **역대 선거:** 한국 1988/2004/2016/2024, 영국 2024, 독일 2021
- **정치 샌드박스:** 정당 합당·분당, 가상 지지 기반 이동, 이벤트, 4년 뒤 다음 총선
- **공약·선거운동·의회:** 기존 정책 질문, 8턴 캠페인, 득표·의석 계산 및 연립정부

'고급 설정 및 데이터 관리'에서 정당·지역·제도 편집, JSON 가져오기·내보내기를 사용할 수 있습니다.

## 역사 자료와 모델 한계

실제 선거 결과는 정당별 확정 의석을 보여주는 역사 자료입니다. **당시 지지율·선거구·정책·선거법을 정확히 복원하지 않습니다.** 초기 정당 지지 강도는 실제 의석 비율을 바탕으로 만든 게임용 수치이고, 사용자가 개표한 결과는 현실의 예측이 아닌 독립적 가상 계산입니다.

- 한국 1988: [국사편찬위원회 한국사DB](https://db.history.go.kr/id/tcct_1988_04_26_0010)
- 한국 2004: [국사편찬위원회 한국사DB](https://db.history.go.kr/id/tcct_2004_04_15_0010)
- 한국 2016: [국토지리정보원 국가지도집](https://nationalatlas.ngii.go.kr/pages/page_1846.php)
- 한국 2024: [국제의회연맹 IPU](https://data.ipu.org/parliament/KR/KR-LC01/election/KR-LC01-E20240410/) — 민주당·국민의힘의 위성정당 의석을 묶어 표시
- 영국 2024: [영국 하원 도서관](https://commonslibrary.parliament.uk/research-briefings/cbp-10009/)
- 독일 2021: [독일 연방선거관리청 2021년 최초 확정 결과](https://www.bundeswahlleiterin.de/info/presse/mitteilungen/bundestagswahl-2021/52_21_endgueltiges-ergebnis.html)

## GitHub Pages 배포

`index.html` 단일 파일로 작동합니다. 저장소 Settings → Pages → Deploy from a branch → `main` → `/(root)`.

브라우저의 localStorage에 자동 저장됩니다. 브라우저 캐시를 삭제하면 기록이 사라질 수 있으므로 장기 저장하려면 JSON으로 백업하세요.