# Kokoa Clone 2023 Update

## 1. login-page

- 레이아웃 나누기 : status-bar / header / form
- styles.css에 관련된 css파일 모두 import하기 (styles.css에는 공통된 부분만 남긴다)
- :root로 색상이나 폰트사이즈를 지정해 변수명으로 가져다 쓸 수 있다
- :not으로 예외로하고 싶은 부분만 따로 스타일을 지정할 수 있다
- input[type="submit"] : input의 type이 submit인 속성만 스타일을 지정할 수 있다

## 2. Friends-page

- components 폴더 : 반복되는 스타일을 컴포넌트 화
- screens 폴더 : 해당 페이지에서만 사용할 스타일
- 레이아웃 나누기 : status-bar(스타일 반복) / header(chat, find랑 같은 스타일) / nav(4개 페이지 스타일 반복)
- nav-chat icon위에 넘버링 : 부모에 position: relative, 해당 요소에 position: absolute, top, left값 설정하기

## 3. Chats-page

- chat-page : 채팅 아이콘이 채워짐, friends-page : 사람 아이콘이 채워짐
- header부분에 아이콘 추가
- user-component__column의 레이아웃 수정
- 개수를 나타내는 숫자 뱃지부분 css 분리

## 4. Find-page

- 설정 아이콘의 빨간 알림 뱃지 추가
- 반복되는 border 스타일 변수로 설정
- position: absolute, relative 설정 반복하면서 많이 익숙해짐

## 5. more, setting, chat page

- 아이콘이나 영역을 눌렀을 때 페이지로 연결되도록 a태그 활용
- 아이콘을 양쪽으로 배치할 때 margin-right: auto, margin-left: auto를 쓰면 아주 간단하고 예쁘게 배치됨..!
- chat-page: 상태바, 채팅 상단바를 모두 position: fixed로 하여 하단으로 스크롤해도 위치고정 할 수 있고 z-index로 레이어의 순서를 지정할 수 있다
- 반복되는 부분은 무조건 component로 빼서 활용도를 높인다
- 채팅 말풍선 모양을 css로 하기 어려워 모서리 부분을 각지게 표현하는 것으로 변경
- 요소의 순서를 바꾸는 방법
  1) order : 숫자 => flex children에게만 적용됨
  2) flex-direction : row-reverse