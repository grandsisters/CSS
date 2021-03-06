### 플렉스 컨테이너를 지정하는 display 속성

<br>

플렉스 박스 레이아웃을 만들려면 먼저 웹 콘텐츠를 플렉스 컨테이너로 묶어 주어야 한다.

배치할 웹 요소가 있다면 그 요소를 감싸는 부모 요소를 만들고, 그 부모 요소를 플렉스 컨테이너로 만들어야 한다.

이때 특정 요소가 플렉스 컨테이너로 동작하려면 display 속성을 이용해 이 부분에 플렉스 박스 레이아웃을 적용하겠다고 지정해야 한다.

플렉스 컨테이너를 지정하는 display의 속성값은 다음과 같다.

|종류|설명|
|----|----|
|flex|컨테이너 안의 플렉스 항목을 블록 레벨 요소로 배치한다.|
|inline-flex|컨테이너 안의 플렉스 항목을 인라인 레벨 요소로 배치한다.|

***
### 플렉스 방향을 지정하는 flex-direction 속성

<br>

플렉스 컨테이너 안에서 플렉스 항목을 배치하는 주축과 방향을 지정하는 속성이다.

<br>

|종류|설명|
|----|----|
|row|주축을 가로로 지정하고 왼쪽에서 오른쪽으로 배치한다. 기본값|
|row-reverse|주축을 가로로 지정하고 반대로 오른쪽에서 왼쪽으로 배치한다.|
|column|주축을 세로로 지정하고 위쪽에서 아래쪽으로 배치한다.|
|column-reverse|주축을 세로로 지정하고 아래쪽에서 위쪽으로 배치한다.|

***
### 플렉스 항목의 줄을 바꾸는 flex-wrap 속성

<br>

flex-wrap 속성을 플렉스 컨테이너 너비보다 많은 플렉스 항목이 있을 경우 줄을 바꿀지 여부를 지정한다.

속성값으로 wrap이나 wrap-reverse로 지정한 후 웹 브라우저 화면의 너비를 늘리거나 줄여 보면 플렉스 컨테이너의 너비에 따라 여러 줄로 표시되는 것을 볼 수 있다.

|종류|설명|
|----|----|
|nowrap|플렉스 항목을 한 줄에 표시한다. 기본값|
|wrap|플렉스 항목을 여러 줄에 표시한다.|
|wrap-reverse|플렉스 항목을 여러 줄에 표시하되, 시작점과 끝점이 바뀐다.|

***
### 배치 방향과 줄 바꿈을 한꺼번에 지정하는 flex-flow 속성

<br>

flex-flow 속성은 flex-direction 속성과 flex-wrap 속성을 한꺼번에 지정하여 플렉스 항목의 배치 방향을 결정거나 줄을 바꾼다.

기본값은 row nowrap이다.

***
### 주축 정령 방법을 지정하는 justify-content 속성

<br>

justify-content 속성을 주축에서 플렉스 항목 간의 정렬 방법을 지정한다.

사용할 수 있는 justify-content의 속성값은 다음과 같다.

|종류|설명|
|----|----|
|flex-start|주축의 시작점에 맞춰 배치한다.|
|flex-end|주축의 끝점에 맞춰 배치한다.|
|center|주축의 중앙에 맞춰 배치한다.|
|space-between|첫 번째 항목과 끝 항목을 주춫ㄱ의 시작점과 끝점에 배치한 후 나머지 항목은 그 사이에 같은 간격으로 배치한다.|
|space-around|모든 항목을 주축에 같은 간격으로 배치한다.|

***
### 교차축 정렬 방법을 지정하는 align-items 속성

<br>

justify-content 속성이 주축에서 항목을 정렬하는 방법이라면, align-items 속성은 교차축을 기준으로 플렉스 항목을 정렬한다.

|종류|설명|
|----|----|
|flex-start|교차축의 시작점에 맞춰 배치한다.|
|flex-end|교차축의 끝점에 맞춰 배치한다.|
|center|교차축의 중앙에 배치한다.|
|baseline|교차축의 문자 기준선에 맞춰 배치한다.|
|stretch|플렉스 항목을 늘려 교차축에 가득 차게 배치한다.|

***
### 특정 항목만 정렬 방법을 지정하는 align-self 속성

<br>

align-item 속성은 교차축을 기준으로 플렉스 항목의 정렬 방법을 결정하지만 그중에서 특정 항목만 지정하고 싶다면 align-self 속성을 사용한다.

그래서 align-item 속성은 플렉스 컨테이너를 지정하는 선택자에서 사용하지만 align-self 속성은 플렉스 항목 선택자에서 사용한다.

align-self 속성에서 사용하는 값은 align-items 속성에서 사용하는 값과 같다.

***
### 여러 줄일 때 교차축 정렬 방법을 지정하는 align-content 속성

<br>

주축에서 줄 바꿈이 생겨서 플렉스 항목을 여러 줄로 표시할 때 align-content 속성을 사용하면 교차축에서 플렉스 항목 간의 간격을 지정할 수 있다.

한 줄일 경우에는 align-items 속성을 사용한다.

|종류|설명|
|----|----|
|flex-start|교차축의 시작점에 맞춰 배치한다.|
|flex-end|교차축의 끝점에 맞춰 배치한다.|
|center|교차축의 중앙에 맞춰 배치한다.|
|space-between|첫 번째 항목과 끝 항목을 교차차구의 시작점과 끝점에 맞추고 나머지 항목은 그 사이에 같은 간격으로 배치한다.|
|space-around|모든 항목을 교차축에 같은 간격으로 배치한다.|
|stretch|플렉스 항목을 늘려서 교차축에 가득 차게 배치한다.|



