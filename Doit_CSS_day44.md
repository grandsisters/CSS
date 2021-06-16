## 한눈에 정리하기

***
### 미디어 쿼리의 속성

<br>

|종류|설명|
|----|----|
|width, height|웹 페이지의 가로 너비, 세로 높이|
|min-width, min-height|웹 페이지의 최소 너비, 최소 높이|
|max-width, max-height|웹 페이지의 최대 너비, 최대 높이|
|device-width, device-height|단말기의 가로 너비, 세로 높이|
|min-device-width, min-device-height|단말기의 최소 너비, 최소 높이|
|max-device-width, max-device-height|단말기의 최대 너비, 최대 높이|
|orientation: portrait|단말기의 세로 모드|
|orientation: landscape|단말기의 가로 모드|

***
### 플렉스 박스 레이아웃의 속성

<br>

|종류|설명|속성값|
|----|----|------|
|display|플렉스 컨테이너를 지정한다.|flex, inline-flex|
|flex-direction|플렉스 항목에서 주축과 방향을 지정한다.|row, row-reverse, column, column-revers|
|flex-wrap|컨테이너 너비보다 항목이 많을 경우 줄 바꿈 여부를 지정한다.|nowrap, wrap, wrap-reverse|
|flex-flow|배치 방향과 줄 바꿈을 한번에 지정한다.|flex-direction 속성값과 flex-wrap 속성값 사용|
|justify-content|주축에서 플렉스 항목 정렬 방법을 지정한다.|flex-start, flex-end, center, space-between, space-around|
|align-items|교차축에서 플렉스 항목 정렬 방법을 지정한다.|flex-start, flex-end, center, baseline, stretch|
|align-self|특정 플렉스 항목의 정렬 방법을 지정한다.|flex-start, flex-end, center, baseline, stretch|
|align-content|여러 줄일 때 교차축 정렬 방법을 지정한다.|flex-start, flex-end, center, space-between, space-around, stretch|
|flex|플렉스 항목의 너비를 줄이거나 늘린다.|1개에서 3개까지의 값, auto, initial|

***
### CSS 그리드 레이아웃의 속성과 함수

<br>

|종류|설명|속성값|
|----|----|------|
|display|그리드 컨테이너를 지정한다.|grid, inline-grid|
|grid-template-columns|칼럼을 지정한다.|크깃값|
|grid-template-rows|줄 높이를 지정한다.|크깃값|
|grid-column-gap|칼럼과 칼럼 사이의 간격을 지정한다.|크깃값|
|grid-row-gap|줄과 줄 사이의 간격을 지정한다.|크깃값|
|grid-gap|칼럼과 줄 사이의 간격을 한꺼번에 지정한다.|크깃값|
|grid-column-start|칼럼 시작의 라인 번호를 지정한다.|숫자|
|grid-column-end|칼럼 마지막의 라인 번호를 지정한다.|숫자|
|grid-column|칼럼 시작 번호와 끝 번호 사이에 슬래시(/)를 넣어 사용한다.|숫자|
|grid-row-start|줄 시작의 라인 번호를 지정한다.|숫자|
|grid-row-end|줄 마지막으 ㅣ라인 번호를 지정한다.|숫자|
|grid-row|줄 시작 번호와 줄 끝 번호 사이에 슬래시(/)를 넣어 사용한다.|숫자|
|grid-area|템플릿 이름을 지정한다.||
|grid-template-areas|grid-area를 사용해 템플릿 그리드를 만든다.||
|minmax()|최솟값과 최댓값을 지정하는 함수이다.|크깃값, auto|
|repeat()|같은 값을 여러 번 반복할 때 사용하는 함수다.|크깃값, auto-fill, auto-fit|

