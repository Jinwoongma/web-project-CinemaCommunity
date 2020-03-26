# Web project2

## 어려웠던 부분

### 1. nav, footer 구현

* navbar를 화면 창 크기에 따라 동적으로 바뀌게 하는것이 힘들었음

  * navbar-collapse와 navbar-toggle을 통해 해결
  * 화면너비가 넓으면 navbar-collapse이 표시되고, navbar-toggle은 숨겨짐
  * 화면너비가 작으면 navbar-collapse은 숨겨지고, navbar-toggle은 표시됨

* 햄버거 버튼을 만드는 과정이 힘들었음

  * navbar-toggler와 navbar-toggler-icon 클래스를 통해 만들 수 있었음

* 화면 너비가 넓을 때 ul 태그를 오른쪽으로 정렬하는 것이 힘들었음

  * ul tag에 ml-auto 속성을 추가하여 해결

* login 버튼을 눌렀을 떄 화면 전체가  Fade가 되고 로그인 창이 클릭되지 않는 현상 발생

  * modal 태그를 nav 태그 밖으로 옮기니 해결됨

    

### 2. Home 구현

* header의 carousel에 넣는 그림이 잘려서 나오는 현상이 발생함
  * img 태그에 d-block w-100 클래스를 추가하여 해결함
* section에서 영화 포스터들 사이에 margin을 넣는 과정이 힘들었음. container 기준으로 col-md-4를 적용하면 margin 없이 3개의 구역으로만 빽빽하게 나뉘어졌음
  * row 클래스 안에 inner라는 div 태그를 추가하고 row 에 padding을 넣어주니 해결됨
  * https://stackoverflow.com/questions/18738712/how-do-i-add-spacing-between-columns-in-bootstrap 

### 4. Community 구현

* 창 크기에 따라 table과 article을 보여주고 숨기는것이 어려웠음
  * table과 artice을 div 태그로 각각 감싸고, 그 div 태그에 visible 클래스를 추가하여 해결함
