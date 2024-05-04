# homework
테킷 프론트앤드 스쿨 10기 과제 저장소

접속상태는 구현하지 못했습니다

#### 초기화 값 
마진과 패딩값을 0으로 주어 디자인에 영향이 가지 않도록 하였습니다

#### avatars 클래스

- **width/heigth 값**
avatars 클래스에는 사진 4장(각 64px/총 256px)과 이미지 간격(각 20px/ 총 60px)을 더해 width값을 316px으로 지정해주었고 사진 2장 (각 64px/총 128px)과 이미지 간격(각 20px/ 총 20px)을 더해 height값을 148px으로 지정해주었습니다.

- **화면 가운데 정렬**
position속성을 absolute로 지정하였고 top과 left을 50%로 지정하여 가운데 정렬하였으며 width값과 height값을 transform: translate 속성으로 정중앙으로 가게끔 하였습니다

#### float 속성
- 사진 각각의 클래스인 woman과 man클래스에 float: left 속성을 넣어 좌측 부터 순서대로 컨테이너 (avatars)안에 들어가게 하였습니다. ~~사실 완벽히 이해한 상태로 사용한건 아니고 이렇게도 해보고 저렇게도 해보다가 되었습니다~~ 

- woman클래스에는 margin-bottom을 주어 man클래스와의 간격을 20px만큼 띄웠습니다

#### nth-child 가상선택자
nth-child 가상선택자를 사용하여 woman클래스와 man클래스의 두번째 선택자부터 margin-left속성이 들어가게 하여 두번째-네번째 사진 왼쪽에만 여백이 20px이 들어가게끔 하였습니다 

#### supports 
- supports를 사용하여 flex속성을 지원하는 브라우저에서는
각사진의 상위 클래스인 woman-group과 man-group에 display:flex속성을 주어 woman클래스 컨텐츠와 man클래스 컨텐츠  row방향으로 나열되도록 하였습니다
- justify-content: space-between 속성을 주어 양끝에는 여백이 없고 가운데에만 균등하게 여백이 들어가게 하였습니다
- float속성을 사용하였을때 사진과 사진사이에 여백을 주기 위해 필요했던 margin-left속성은 justify-content: space-between으로 대체하여 0px로 변경하였습니다 

