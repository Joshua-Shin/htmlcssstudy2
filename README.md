- pseudo-element, 애니메이션, shadow dom 이런건 일단 생략.
- 기본 태그, form, 레이아웃은 기본이고, 조금 더 추가하면 fontAwesome, bootstrap 활용하는것까지만 선 그어놓자.

#### 핵심 문법
- css 맨 위에 두면 좋은거
  - body {margin: 0px;}
  - div {box-sizing: border-box;}

- form에서 input 이외의 태그
  - <button type="submit">전송</button> 
  - <textarea cols="30" rows="10"></textarea> // 여러줄 입력

- display
  - display: flex;
  - justify-content: center; // 좌우 정렬
  - flex-wrap : wrap; // 넘치면 아래로 내려감. 이거 안해주면 한줄에 자식요소들이 최대한으로 차지하면서 버팀.
  - align-items: center; // 상하 정렬
  - flex-direction : row; // row가 기본값, 반응형 웹 만들때 row만 column으로 바꾸면 쉽게 적용되겠네.
  - flex-grow:2; // flex 박스의 남은 여백을 얼마나 차지 할것이냐, 형제 div들의 grow 값의 합에서 2만큼 차지함. 얘만 자식요소에 직접 선언

- background
  - background-image : url(../img/shoes.jpg);
  - background-image: linear-gradient( rgba(0,0,0,0.5), rgba(0,0,0,0.5) ), url(이미지경로); // 배경 사진 어둡게 해서 글씨 잘 보이게
  - background-size : cover; // 배경사진 짤려도 상관 없으니 div의 빈 공간 없이 배경으로 채워라.
  - background-repeat : no-repeat; // 배경사진 반복하지 마라
  - background-position : center; // 배경사진 위치 조절
  - padding : 1px; // 배경으로 지정한 div 내에 padding 없이 div 또 선언하면, margin collapse effect 현상 생길 수 있는데 이를 해결해줌.
  
- position
  - position 부여하면 생기는 효과 2가지
    - 1_ 좌표이동가능 ex) top:10px; bottom:10px; left:0; right:0;
    - 2_ 공중에 뜸
  - position: relative; // 내 원래 위치를 기준으로 이동하세요.
  - position: static; // 좌표 이동 하지 않음
  - position: fixed; / 뷰 포트 기준으로 고정
    - 스크롤 올리고 내려도 계속 화면에 고정되는 상단바 라든가, 왼쪽 세로로 긴 매뉴바라든가, 오른쪽 하단에 '상담하기' '구매하기' '스크롤한번에위로올리기' 버튼 같은거 만들떄 좋음
    - sticky는 스크롤을 내리면 그 기준부터 같이 붙어서 고정됨.
  - position: absolute;
    - 내 부모 태그 중 relative가 선언된 부모를 기준으로 좌표 이동 가능
- 애니메이션
  - one-way 애니메이션 혼자 알아서 만드는 법
    - 1_ 시작스타일 정하기
    - 2_ 최종스타일 정하기
    - 3_ 언제 최종스타일로 변할지 트리거 주기 (대부분 마우스 올렸을 때임)
    - 4_ transition 으로 서서히 동작하게 만들기 
- 시작 스타일에 transition : all 1s;

- fontawesome은 cdn 주소 따로 구글링해서 복붙해야되고, bootstrap은 공식사이트에 가이드 나와있음

#### 최종 미션
- form & display 연습
<img width="500" src="https://user-images.githubusercontent.com/93418349/229077955-64b92094-b038-4108-a5cf-9b0f20d491e9.png">
- 배경 & Position 연습 
<img width="600" src="https://user-images.githubusercontent.com/93418349/229390060-f1e83a8b-513e-405a-9c96-d27b3994f9bf.png">
- 애니메이션 연습
<img width="400" src="https://user-images.githubusercontent.com/93418349/229078484-988b14aa-4ee4-48de-864e-5ef0bac9ba9b.gif">

------------


<!--
- Landing Page 만들기 <br>
  - PC화면 <br>
<img width="600" src="https://user-images.githubusercontent.com/93418349/229078422-48425c7f-f451-44a4-b718-ef66287518ac.png">
  - 모바일 <br>
<img width="300" src="https://user-images.githubusercontent.com/93418349/229078436-73c51459-80ad-4d7e-89cf-d1d1a0679e05.png">
  - 애니메이션 <br>
<img width="300" src="https://user-images.githubusercontent.com/93418349/229078484-988b14aa-4ee4-48de-864e-5ef0bac9ba9b.gif">
-->
