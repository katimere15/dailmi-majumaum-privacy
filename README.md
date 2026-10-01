# 마주마음 개인정보처리방침

마주마음 `com.dailmi.majumaum`의 공개 개인정보처리방침과 배포 파일은 이 디렉터리에서만 관리한다.

- 공개 문서: `index.html`
- 공개 저장소: https://github.com/katimere15/dailmi-majumaum-privacy
- 공개 주소: https://katimere15.github.io/dailmi-majumaum-privacy/
- 운영자: Dailmi
- 개인정보 문의: `chyou960118@gmail.com`
- 기준일: 2026-10-01
- 언어: 한국어 전체 본문과 영문 전체 번역

현재 문서는 다음 실제 구현을 기준으로 작성했다.

- Google 로그인과 Firebase Authentication
- 서울 `asia-northeast3`의 Cloud Firestore·Cloud Functions
- Local-first 개인 배려카드와 기기 로컬 알림
- 2인 연결, 마음카드, 날짜 합의, 공유 캘린더와 준비 체크리스트
- FCM 푸시, Firebase App Check와 Play Integrity
- 마음카드 수신 중지, 차단·연결 해제, 데이터 내보내기와 계정 삭제
- 연결 종료 뒤 공유 데이터 접근 즉시 차단과 7일 삭제 대기
- Firebase Analytics, Crashlytics와 광고 SDK 미사용
- 종단간 암호화는 아직 적용하지 않음

## 공개 전 필수 확인

1. 앱 또는 스토어 등록정보에서 공개 정책 URL로 쉽게 이동할 수 있게 한다.
2. Android 자동 백업을 유지할지 또는 민감한 로컬 카드 데이터를 백업에서 제외할지 결정한다. 현재 앱은 자동 백업을 명시적으로 차단하지 않으므로 본문도 이를 그대로 안내한다.
3. 만료·사용된 초대 레코드의 자동 삭제를 구현할지 결정한다. 현재는 24시간 뒤 사용할 수 없지만 레코드는 생성자 계정 삭제 때까지 보관되므로 본문도 이를 그대로 안내한다.
4. App Check, 계정 삭제, 7일 예약 삭제와 데이터 내보내기를 실기기에서 검증한다.
5. Google Play 데이터 보안 양식의 수집·공유·삭제 답변이 이 문서 및 실제 SDK 동작과 일치하는지 검토한다.

기능, SDK, 저장 위치, 수탁자, 보유 기간 또는 삭제 동작이 바뀌면 앱 코드·백엔드 문서·이 처리방침을 같은 변경에서 함께 갱신한다.

