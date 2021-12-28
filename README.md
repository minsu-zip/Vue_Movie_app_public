## 📌 프로젝트 설명 <!-- 어떤 걸 만들었는지 대략적으로 설명해주세요 -->
프로그래머스 데브코스에서 진행한 프로젝트로 일부 기록이 노출되면 안 되는 상황으로 인해 commit 기록이 없음
<br>
[Vue3를 활용한 간단한 영화 검색 사이트](https://angry-albattani-9bdfaf.netlify.app/)

이벤트 흐름 :
- Home 컴포넌트 생성 시 기본 data값("frozen")으로 API 요청
- 영화 검색 시  value값으로 API 요청
- More 버튼 클릭 시 기존 data + nextPage 값으로 API 요청
- 영화 상세 보기(detail) 클릭시 Modal 기능으로 영화 상세 정보 출력
  - Modal 컴포넌트에 클릭된 영화 id값을 넘겨주고 받은 id값 기준으로 API 요청
- 잘못된 경로 입력 시 NotFound 처리

## 👩‍💻 구현 내용

- [x] 검색어를 입력해 영화를 검색할 수 있어야 합니다.
- [x] 검색된 결과를 통해 영화의 상세 정보를 볼 수 있어야 합니다.
- [x] 클라이언트에서 API Key가 노출되지 않아야 합니다.
- [x] 실제 서비스로 배포하고 접근 가능한 링크를 추가해야 합니다.
- [x] API 요청(Request)에 대한 로딩 애니메이션을 추가해 보세요.
- [x] 영화 상세 검색으로 출력할 영화 포스터를 더 높은 해상도 사용해 보세요.
  - [x] 영화 포스터 주소에 포함된 `SX300`를 `SX700`과 같이 더 큰 숫자로 수정해 요청하세요.
- [x] 더보기 기능을 통해 추가 데이터 가져오기
  - 검색 결과가 바뀌면 이전 데이터 초기화
- [x] 잘못된 경로 처리

대략적인 컴포넌트 구조
<img src='https://user-images.githubusercontent.com/52727782/136580213-ff3fa144-f739-44ae-9415-320690c66467.jpg' style="height:80%";/>
<!-- ![컴포넌트 구조](https://user-images.githubusercontent.com/52727782/136580213-ff3fa144-f739-44ae-9415-320690c66467.jpg) -->

시연영상

https://user-images.githubusercontent.com/52727782/136582907-6ce83545-e7a6-42da-9bf6-e483894933e1.mp4
