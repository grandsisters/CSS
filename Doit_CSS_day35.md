***
### 웹 문서의 가로 너비와 세로 높이 속성

<br>

실제 웹 문서 내용이 화면에 나타나는 영역을 뷰포트라고 하는데 뷰포트의 너비와 높이를 미디어의 쿼리 조건으로 사용할 수 있다.

이때 높잇값은 미디어에 따라 달라지므로 주의해야 한다.

screen이 아닌 미디어에서는 스크롤을 포함한 전체 문서를 height로 지정해야 하며, print에서는 한 페이지 높이를 기준으로 한다.


|종류|설명|
|----|----|
|width, height|웹 페이지의 가로 너비, 세로 높이를 지정한다.|
|min-width, min-height|웹 페이지의 최소 너비, 최소 높이를 지정한다.|
|max-width, max-height|웹 페이지의 최대 너비, 최대 높이를 지정한다.|

    - 예시
    @media screen and (min-width: 1440px) { 너비가 최소 1440px인 화면용 스타일
        ...
    }

    너비가 1440px 이상일 때 미디어 쿼리

***
### 단말기의 가로 너비와 세로 높이 속성

<br>

이번에는 단말기에서 기본으로 제공하는 물리적인 가로 너비와 세로 높이의 크기를 체크해 보자.

단말기의 너비와 높이는 단말기 브라우저 창의 너비와 높이를 말한다.

이때 주의할 점을 대부분의 단말기 해상도와 실제 브라우저의 너비가 다르다는 것이다.

단말기 너비나 높이를 고려해 미디어 쿼리를 작성해야 한다면 다음과 같은 속성을 사용한다.

|종류|설명|
|----|----|
|device-width, device-height|단말기의 가로 너비, 세로 높이를 지정한다.|
|min-device-width, min-device-height|단말기의 최소 너비, 최소 높이를 지정한다.|
|max-device-width, max-device-height|단말기의 최대 너비, 최대 높이를 지정한다.|

    - 예시
    @media screen and (min-device-width: 375px) and (min-device-height:812px) {
        ...
    }

    iphone X일 경우에 미디어 쿼리

***
### 화면 회전 속성

<br>

미디어 쿼리에서 orientation 속성을 사용하면 기기의 방향을 확인할 수 있고, 그에 따라서 웹 사이트의 레이아웃을 바꿀 수 있다.

orientation 속성으로는 portrait와 landscape가 있다.

가로 모드는 landscape, 세로 모드는 portrait 이며, 기본값은 landscape이다.

|종류|설명|
|----|----|
|orientation: portrait|단말기의 세로 모드를 지정한다.|
|orientation: landscape|단말기의 가로 모드를 지정한다.|

    - 예시
    @media screen and (min-device-width: 812px) and (orientation: landscape) {
        ...
    }

    iphone X를 가로로 돌릴 경우에 미디어 쿼리

이 외에도 화면 비율이나 단말기 화면 비율, 색상당 비트 수 같은 여러 가지 미디어 쿼리 조건이 있다.