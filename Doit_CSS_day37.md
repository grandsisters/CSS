### 미디어 쿼리 적용하기

<br>

미디어 쿼리가 어떻게 구성되는지 알았으니 웹 문서에 적용해 보자.

적용하는 방법은 크게 외부 CSS 파일로 연결하는 방법과 웹 문서에 직접 정의하는 방법이 있다.

***
### 외부 CSS 파일 연결하기

<br>

외부 CSS 파일을 따로 저장해서 웹 문서에 연결하는 방법을 알아보자.

이 방법은 각 조건별로 CSS 파일을 따로 저장한 뒤 link태그나 @import문을 사용해서 연결한다.

먼저 외부 CSS 파일을 연결할 때 가장 많이 사용하는 link태그를 알아보자.

link태그는 head태그 사이에 넣는다.

    - 기본형 
    <link rel='stylesheet' media='미디어 쿼리 조건' href='css 파일 경로'>

위 기본형의 의미는 미디어 쿼리 조건이 맞다면 지정한 CSS 파일을 가져와서 적용하라는 것이다.

속성의 순서는 상관없다.

예를 들어 인쇄용 CSS를 정의한 css/print.css 파일을 만들어 놓았다면 다음과 같은 코드를 작성하여 웹 문서와 연결하면 된다.

    - 예시
    <link rel='stylesheet' media='print' href='css/print.css>


외부 CSS 파일을 연결하는 또 다른 방법으로 link태그 대신 @import문을 사용할 수 있다.

@import문은 CSS를 정의하는 style태그 사이에서 다음과 같이 사용한다.

    - 기본형
    @import url(css 파일 경로) 미디어 쿼리 조건

예를 들어 태블릿용 CSS를 정의한 css/tablet.css 파일을 만들고, 너빗값이 321px 이상이면서 768px 이하일 때에 미디어 쿼리를 적용하려면 다음과 같이 지정할 수 있다.

    - 예시
    @import url('css/tablet.css') only screen and (min-width: 321px) and (max-width: 768px);

***
### link태그와 @import문의 차이점

<br>

link태그와 @import 문은 모두 외부에서 CSS 파일을 가져와 사용하는 방법이다.

CSS 파일이 한두개 밖에 없다면 속도나 처리 면에서는 큰 차이가 없다.

그런데 인터넷 익스플로러의 경우 @import 문과 자바스크립트가 함께 있을 경우 자바스크립트를 먼저 내려받은 후에 @import 문에 있는 CSS를 다운로드 한다.

그로인해 자바스크립트에서 스타일과 관련된 정보를 처리해야 할 경우 오류가 날 수도 있다.

그래서 CSS 파일이 많고 규모가 큰 사이트를 개발한다면 @import 문보다 link태그를 주로 사용한다.
***
### 웹 문서에 직접 정의하기

<br>

이번에는 외부 CSS 파일을 만들지 않고 웹 문서에서 미디어 쿼리를 직접 지정하는 방법을 알아보자.

웹 문서에 미디어 쿼리를 직접 정의하는 방법은 2가지이다.

첫 번째 방법은 style 태그 안에서 media 속성을 사용하여 조건을 지정하고, 그 조건에 맞는 스타일 규칙을 정의하는 것이다.

    - 기본형
    <style media='<조건>'> {
        <스타일 규칙>
    }
    </style>


예를 들어 다음은 media 속성을 사용해 화면 너비가 320px 이하일 때 배경색을 주황색으로 바꾸는 미디어 쿼리이다.

    - 예시
    <style media='screen and (max-width:320px)'>
        body {
            background-color: orange;
        }
    </style>

두 번째 방법은 스타일을 선언할 때 @media 문을 사용해 각 조건별로 스타일을 지정해 놓고 스타일을 선택해서 적용하는 것이다.

@media 문을 사용하는 기본형은 다음과 같다.

    - 기본형
    <style>
        @media <조건> {
            <스타일 규칙>
        }
    </style>

예를 들어 @media 문을 사용해 화면 너비가 320px 이하일 경우 배경색을 주황색으로 바꾸는 미디어 쿼리는 다음과 같이 사용한다.

    - 예시 
    <style>
        @media screen and (max-width: 320px) {
            body {
                background-color: orange;
            }
        }
    </style>

첫 번째 방법은 하나의 style 태그 안에서 하나의 조건을 지정하지만, 두 번째 방법은 style 태그 안에 여러 개의 조건에 따른 스타일을 모두 나열해 놓고 그중에서 선택해서 사용한다.

