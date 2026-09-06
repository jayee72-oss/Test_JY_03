# 크루즈야 마린지점 공식 반응형 홈페이지 & 랜딩페이지 운영 가이드

**크루즈야 마린지점(담당자: 전재의 지사장)**의 공식 1:1 맞춤 상담 반응형 웹사이트입니다.  
로열캐리비안, 크루즈예약.com, 크루즈여행닷컴의 우수한 UI/UX(대형 선박 감성 히어로, 빠른 조건 검색 바, 지역별 카테고리 탭 탐색)를 결합하여 설계되었습니다.

---

## 1. 🌐 실시간 공식 배포 주소 (Production Live)

누구나 스마트폰, PC에서 바로 접속할 수 있는 공식 배포 링크입니다:

* 🚀 **공식 운영 주소:** **[https://cruiseya-marine.vercel.app](https://cruiseya-marine.vercel.app)**
* 💻 **로컬 테스트 주소:** [http://localhost:3456](http://localhost:3456)

---

## 2. 향후 수정 사항 재배포 방법 (원클릭)

`index.html`에서 문구나 연락처, 이미지를 수정한 뒤 터미널에서 다음 명령어를 실행하면 5초 만에 실시간 웹사이트에 반영됩니다:

```bash
vercel --prod --yes
```

---

## 3. 운영자 정보 수정 방법 (`SITE_CONFIG`)

`index.html` 내 `<script>` 태그 상단의 `SITE_CONFIG` 값을 수정하여 손쉽게 관리할 수 있습니다.

```javascript
const SITE_CONFIG = {
  brandName: "크루즈야 마린지점",
  managerName: "전재의",
  branchRole: "지사장",
  region: "부산",

  phoneNumber: "010-0000-0000", // 전화번호 입력 시 원클릭 통화 활성화
  kakaoChannelUrl: "https://pf.kakao.com/_xxxxxx", // 카카오톡 채널 링크
  email: "contact@cruiseya-marine.com",

  webhookUrl: "" // Google Sheets Apps Script 배포 URL (연동 시 입력)
};
```
