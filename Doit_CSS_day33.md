### 뷰포트 지정하기

<br>

뷰포트는 meta태그를 이용해 head태그 사이에 작성한다.

    - 기본형 <meta name='viewport' content='속성1=값1', '속성2=값2', ...>

이와 같이 content 속성을 이용해 뷰포트 속성과 속성값을 지정하면 되는데, content 안에서 사용하는 뷰포트의 속성은 다음과 같다.

|종류|설명|사용 가능한 값|기본값|
|----|----|--------------|------|
|width|뷰포트 너비|device-width 또는 크기|브라우저 기본값|
|height|뷰포트 높이|device-height 또는 크기|브라우저 기본값|
|user-scalable|확대,축소 가능 여부|yes 또는 no(yes는 1로, device-width와 device-height값은 10으로 간주)|yes|
|initial-scale|초기 확대,축소 값|1~10|1|

다음은 가장 많이 사용하는 뷰포트 속성으로 웹 페이지 뷰포트의 너비를 스마트폰 화면 너비에 맞추고 초기 화면 배율을 1로 지정한다.

    <meta name='viewport' content='width=device-width, initial-scale=1'>

***
### 뷰포트 단위

<br>

뷰표트 개념이 등장하기 전까지는 CSS에서 크기를 지정할 때 주로 px, %의 단위를 사용했지만 이제는 다음과 같이 뷰포트를 기준으로 하는 단위를 사용할 수도 있다.

- vw(viewprot width): 1vw는 뷰포트 너비의 1%와 같다.
- vh(viewport height): 1vh는 뷰포트 높이의 1%와 같다.
- vmin(viewport minimum): 뷰포트의 너비와 높이 중에서 작은 값의 1%와 같다.
- vmax(viewport maximum): 뷰포트의 너비와 높이 중에서 큰 값의 1%와 같다.

예를 들어 뷰포트의 너비가 1000px, 높이가 800px일 경우 1vw는 10px, 1vh는 8px가 된다.

1vmin은 너빗값과ㅏ 높잇값 중 작은 값인 800px의 1%인 8px가 되고 vmax는 10px가 된다.

만일 화면을 돌리게 되면 어떻게 될까?

방향이 바뀌므로 1vw는 8px, 1vh는 10px가 된다.

하지만 작은 값과 큰 값의 변화가 없으므로 vmin은 8px, vmax는 10px가 그대로 유지된다.