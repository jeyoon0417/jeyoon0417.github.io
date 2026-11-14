# JamesWorks 메인 사이트

게임 목록 페이지. 여기에 도메인을 연결하면 다른 게임 저장소들이 자동으로 `도메인/저장소이름/` 주소가 된다.

## 올리는 곳

저장소 이름을 **정확히 `jeyoon0417.github.io`** 로 만들어야 한다 (사용자 사이트 저장소). 이 폴더의 파일을 전부 최상위에 올리고, Settings → Pages에서 `main` / `(root)`를 켠다.

- `index.html` 메인 페이지
- `privacy.html` 개인정보처리방침 (모든 게임 공통)
- `icon-192.png`, `icon-512.png` JamesWorks 로고
- `orak-icon.png` 오르락내리락 카드 아이콘
- `ic-game.png`, `ic-group.png`, `ic-wrench.png` 픽셀 아이콘

## 도메인 연결 (예: jamesworks.kr)

1. 도메인을 산다.
2. **먼저** 이 저장소 Settings → Pages → Custom domain에 도메인을 입력하고 Save.
3. 도메인 업체 DNS 설정에 아래를 추가한다.
   - A 레코드 `@` → `185.199.108.153`, `185.199.109.153`, `185.199.110.153`, `185.199.111.153` (4줄)
   - CNAME 레코드 `www` → `jeyoon0417.github.io`
4. DNS가 반영되면(보통 몇 분~몇 시간) Custom domain 옆에 체크 표시가 뜬다. 그다음 **Enforce HTTPS**를 켠다.
5. 결과:
   - `jamesworks.kr` → 이 메인 페이지
   - `jamesworks.kr/Orak/` → 오르락내리락 (Orak 저장소는 아무것도 안 바꿔도 됨)

## 게임을 추가할 때

새 저장소를 만들고 Pages만 켜면 `jamesworks.kr/저장소이름/` 으로 열린다. `index.html`의 게임 목록에 카드 하나만 추가하면 끝.
같은 도메인의 게임들은 브라우저 저장 공간을 같이 쓰므로, 저장 이름 앞에 게임 이름을 붙인다 (오르락내리락은 `orak_`).

## 애드센스

사이트 등록은 **도메인(jamesworks.kr) 하나**로 한다. 승인되면 `ads.txt`를 **이 저장소 최상위**에 올린다 (게임 저장소가 아니라 여기).
