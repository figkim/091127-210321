### Repository for the online wedding invitation card.

#### TO-DO
- [ ] 메인 이미지의 ratio 는 유지하면서, width 는 device-agnostic 하도록 변경
  - 현재는 device screen 에 맞춰 ratio 가 변하다 보니, 일반적인 가로 모니터의 경우 이미지 height 가 잘림.
- [ ] 주요 사진 선정 및 작문
  - 전체 사진 최종본으로 변경
  - Milestone 4 개로 줄이기
  - 메인 27
  - 중앙 14
  - 엔딩 33
  - 갤러리 (16-12-25-20-10-3-13-34-35-7-18-31)
- [ ] Embed image 화질 낮추기
- [ ] Tmap, Kakao navi 길 안내 invoke 기능 추가 ([참조](https://community.openapi.sk.com/t/tmap/9170/2))
- [ ] Apple cal, Google cal 일정 추가 기능 추가
- [ ] Facebook event 생성 및 댓글 링크 추가

#### 참고사항
- Social media thumbnail image 의 경우, 한 번 이미지를 불러오고 난 뒤로는 지속하여 캐시 데이터를 활용함.
  - 카카오톡: Open graph cache flush 를 활용 (https://developers.kakao.com/tool/clear/og)
  - 슬랙: [Reddit](https://www.reddit.com/r/Slack/comments/hhbald/how_to_clear_unfurl_cache/) 에 따르면 manually flush 기능은 없어보이고, 24시간 뒤 renewal 된다고 하니 확인 
