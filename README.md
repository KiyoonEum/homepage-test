# Kiyoon Eum — Aqua 홈페이지

HTML과 CSS만으로 동작하는 GitHub Pages용 홈페이지입니다. 설치·빌드 과정은 필요 없습니다.

## GitHub에 적용

1. ZIP 압축을 풉니다.
2. `kiyooneum.github.io-main` 폴더 **안의 내용**을 기존 `kiyooneum.github.io` 저장소의 루트에 올립니다. 폴더 자체를 한 단계 더 중첩하지 않습니다.
3. 같은 이름의 `index.html`, `style.css`, `README.md`를 교체하고 새 배경·아이콘 파일을 `assets`에 추가합니다.
4. 기존 `misc` PDF, 프로필 사진, 사이트맵, Google 인증 파일도 포함되어 있습니다.

기존 GitHub Pages 설정을 그대로 사용하면 됩니다. PC에서 `index.html`을 열어도 확인할 수 있습니다.

## 수정 위치

| 내용 | 파일 / 표시 |
| --- | --- |
| 제목·검색 소개 | `index.html`의 `[EDIT 01]` |
| 이름·메뉴 | `[EDIT 02]` |
| 첫 화면 문구·버튼 | `[EDIT 03]` |
| 소개·사진 | `[EDIT 04]` |
| 연구 관심사 | `[EDIT 05]` |
| 논문 | `[EDIT 06]` — `li.publication` 한 개가 한 편 |
| 학력·강의 경력 | `[EDIT 07]` |
| 발표·초록 | `[EDIT 08]` — `details.talk` 한 개가 한 발표 |
| 노트·PDF 경로 | `[EDIT 09]` |
| 하단 연락처·갱신일 | `[EDIT 10]` |
| 색·폰트·폭·여백·배경 | `style.css`의 `:root` |
| 카드·접기/펼치기·모바일 | `style.css`의 07–08번 구역 |

이메일은 헤더·소개·하단 세 곳에 있습니다. 주소를 바꿀 때 세 곳을 함께 변경하세요.
논문·발표·노트는 각각의 HTML 블록을 복사해 추가할 수 있습니다. 논문을 추가하면 `paper-number`의 표시 번호도 함께 갱신하세요.
CV를 처음부터 펼쳐 두려면 `<details class="cv">`에 `open`을 추가하세요.

## 기존 파일에서 정리한 부분

- 기존 인적 사항, 논문 5편, 학력 2개, 강의 경력 7개, 발표 5개 및 초록, PDF 노트 3개를 반영했습니다.
- 하단 인용문과 BANG 장식은 넣지 않았습니다.
- 잘못 연결된 이메일 버튼을 `kyeum@kaist.ac.kr`로 고쳤습니다.
- 첨부에 `CV.pdf`가 없어 CV 버튼은 페이지 안의 CV로 연결했습니다. PDF를 추가한 뒤 원하는 위치에 `<a href="CV.pdf">Download CV (PDF)</a>`를 넣으면 됩니다.
- `[doi]`, `XXXX.XXXXX`, 빈 Slides 등 임시 링크는 제거했습니다. 실제 주소가 생기면 해당 논문·발표 블록에 링크를 추가하세요.
- `#top`, `#about`, `#papers`, `#cv`, `#talks`, `#misc` 앵커와 기존 PDF 경로를 유지했습니다.
- 원본에 있던 출판 상태와 연도는 유지했습니다.

## 구성

- `index.html`: 모든 문구·목록·링크
- `style.css`: 디자인과 모바일 대응
- `assets`: 원본 프로필 사진, Aqua 배경, SVG 아이콘
- `misc`: 원본 노트 PDF
- `sitemap.xml`, `google00ef7af9e22e08ee.html`: 기존 검색 관련 파일

외부 폰트나 JavaScript에 의존하지 않습니다. CV와 발표는 브라우저 기본 접기/펼치기 기능으로 동작합니다.
