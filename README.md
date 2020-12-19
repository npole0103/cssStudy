# StudyCSS
CSS SUMMARY

---
## Tag & Code

style CSS 코드 내용을 담음 : `<style>내용</style>`

HTML 태그 내에서 속성으로 사용 : `style="color:black"`

선택자 Selector : `a { }`

효과 declaration 선택자 내에서 사용 : `{      }`  
괄호 내에 있는 것을 선언(효과)라고 지칭함.

`color:black;`에서 color는 속성, red는 value라고 부름.

링크에 존재하는 언더라인 삭제 : `text-decoration: none;`

언더라인 생성 : `text-decoration: underline;`

글자 폰트 : `font-size: 60px;`

글자 정렬 : `text-align: center;`

class : `class="클래스이름"`

style 태그 내에서 class 사용 : `.클래스이름 { }`

id : `id="아이디이름"`

style 태그 내에서 id 사용 : `#아이디이름 { }`

선택자 서열 : id > class > 태그  
(같은 서열 내에선 가장 밑에 있는 선택자가 우선 순위)

암묵적 규칙 : id 선택자는 단 한번만 등장해야한다 id는 중복돼서는 안된다.

---
## Box Model

**border** : 테두리를 뜻함  
    `border-width: 5px;`  테두리 두께
    `border-color: red;`  테두리 색
    `border-style: solid;` 테두리 스타일 단선(solid)

Block level element : 화면 전체를 크기로 쓰는 태그 ex) h1

inline element : 자기 자신의 크기만큼만 크기로 갖는 태그 ex) a

display 속성을 추가해서 block과 inline을 전환할 수 있음  
    `display:inline;` inline level로 설정  
    `display:bloack;` block level로 설정
    `display:none;` 화면에서 보이지 않게 설정

중복의 제거 : `border: 5px red solid;`로 5px red solide 모두 설정 가능

**padding** : content와 border 사이에 여백을 주는 속성

**margin** : border와 또 다른 border 사이에 여백을 주는 속성

content 폭과 높이 : width와 height 속성으로 크기 조절  
`width:100px`  
`height:40px`

---
## Grid

div : 나누기 위해 쓰이는 아무런 의미 없는 태그. Block level element이다.  
`<div>내용</div>`

span : 나누기 위해 쓰이는 아무런 의미 없는 태그 Inline level element이다.  
`<span>내용</span>`

grid-templete-colums : 열로 나누게 됨.  
`grid-template-columns: 150px 1fr;` 여기서 1fr은 자동으로 나머지를 할당하는 것인데 만약 2fr 1fr로 쓰면 첫 열은 전체의 2만큼 두번째 열은 전체의 1만큼 총 3의 크기로 나뉘어 할당된다. px값을 넣으면 고정된다.

`#idname ol { }` 이라는 id 이름 뒤에 나온 태그 이름은
그 아이디 내에 있는 하위 ol 태그들에 대한 내용을 적용할 때 사용.

## Media Query

`@media(조건식) { }` : 조건이 맞다면 { }안에 해당하는 코드가 실행됨.

`min-width: 800px` : 화면의 크기 최소값이 800px이다  
(screenWidth > 800px )

`max-width: 800px` : 화면의 크기가 최대값이 800px이다  
(screenWidth < 800px )

미디어 쿼리를 활용하면 조건문처럼 특정 조건이 되었을 때 웹브라우저에 나타나는 화면을 제어할 수 있다.

Link 문서간 연결 혹은 외부 리소스 연결 시 사용 : `<link rel="stylesheet" type="text/css" href="theme.css">`  
link 태그 사용시 웹브라우저에서 해당 문서를 다운받아서 적용하게 됨.

속성
- href 연결 문서 위치
- rel 연결 문서와의 관계
- type 연결 문서의 타입
(예제에선 type 사용 안함)

Link 태그는 근시안적으로 보면 문서 다운을 받게 되면 트래픽을 사용하게 되어 비효율적이라고 생각할 수 있다. 하지만 원시안적으로 보면
캐싱이라는 기술을 사용해서 한번 다운한 파일을 다시 읽기 때문에
엄청난 효율을 낼 수 있다.

---
## etc

코딩은 중복의 제거가 중요하다.

CSS로 HTML을 디자인 하는 것이 훨씬 효율적이다.

style 태그 말고 속성을 통해서도 CSS를 사용할 수 있다.

같은 선택자일 때 보다 밑에 있는 선택자가 더 우선 순위이다.

태그 서열이 id > class > 태그인 이유는 포괄적인 것 일수록
그것을 전체적으로 변화시키고 특수하고 예외적인 것들만 우선적으로 변경시키는 것이 효율적이기 때문이다.

**개발자도구 F12** 혹은 **마우스 우클릭 검사**를 이용하면 HTML 문서를 볼 수 있으며 각 컨텐츠의 CSS 부분이 어떻게 작성되었는지 볼 수 있다.

[CanIUse.com](https://caniuse.com/) : HTML CSS JAVASCRIPT 기술 등을 인터넷 브라우저가 채택하고 있는 통계를 보여주는 사이트

선택자와 속성이 CSS에서 가장 중요함.

속성을 많이 알 수록 표현이 풍부하고 선택자를 많이 알 수록 속성을 잘 활용할 수 있음. 



---