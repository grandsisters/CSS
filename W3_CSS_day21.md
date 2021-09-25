## CSS Margins

여백은 정의된 테두리 외부의 요소 주위에 공간을 만드는 데 사용됩니다.

***
### CSS 여백
CSS margin속성은 정의된 테두리 외부의 요소 주위에 공간을 만드는 데 사용됩니다.

CSS를 사용하면 여백을 완전히 제어할 수 있습니다. 요소의 각 측면(위, 오른쪽, 아래, 왼쪽)에 대한 여백을 설정하는 속성이 있습니다.

***
### 여백 - 개별 측면
CSS에는 요소의 각 측면에 대한 여백을 지정하는 속성이 있습니다.

- margin-top
- margin-right
- margin-bottom
- margin-left

모든 여백 속성은 다음 값을 가질 수 있습니다.

- auto - 브라우저가 여백을 계산합니다.
- 길이 - 여백을 px, pt, cm 등으로 지정합니다.
- % - 포함하는 요소 너비의 %로 여백을 지정합니다.
- 상속 - 여백이 부모 요소에서 상속되어야 함을 지정합니다.

팁: 음수 값이 허용됩니다.

    예시
    <p> 요소의 네 면 모두에 대해 다른 여백을 설정합니다.

    p {
    margin-top: 100px;
    margin-bottom: 100px;
    margin-right: 150px;
    margin-left: 80px;
    }

***
### 여백 - 약식 속성
코드를 줄이려면 하나의 속성에 모든 여백 속성을 지정할 수 있습니다.

margin속성은 다음 각 마진 특성에 대한 약식 속성이다 :

- margin-top
- margin-right
- margin-bottom
- margin-left

작동 방식은 다음과 같습니다.

4개의 margin 속성 값이 있는 경우:

- 여백: 25px 50px 75px 100px;
    - 상단 여백은 25px입니다.
    - 오른쪽 여백은 50px입니다.
    - 하단 여백은 75px입니다.
    - 왼쪽 여백은 100px입니다.


    예시
    4개의 값과 함께 margin 속기 속성을 사용합니다.

    p {
    margin: 25px 50px 75px 100px;
    }

3개의 margin 속성 값이 있는 경우:

- 여백: 25px 50px 75px;
    - 상단 여백은 25px입니다.
    - 좌우 여백은 50px
    - 하단 여백은 75px입니다.


    예시
    다음 세 가지 값과 함께 margin 속기 속성을 사용합니다. 

    p {
    margin: 25px 50px 75px;
    }


2개의 margin 속성 값이 있는 경우:

- 여백: 25px 50px;
    - 상단 및 하단 여백은 25px입니다.
    - 좌우 여백은 50px


    예시
    다음 두 값과 함께 margin 속기 속성을 사용합니다. 

    p {
    margin: 25px 50px;
    }


1개의 margin 속성 값이 있는 경우:

- 여백: 25px;
- 네 여백은 모두 25px입니다.


    예시
    하나의 값과 함께 margin 속기 속성을 사용합니다. 

    p {
    margin: 25px;
    }

***
### 자동 값
여백 속성을 auto로 설정하여 컨테이너 내에서 요소를 가로로 가운데에 맞출 수 있습니다 .

그러면 요소가 지정된 너비를 차지하고 나머지 공간이 왼쪽과 오른쪽 여백 사이에 균등하게 분할됩니다.

    예시
    여백 사용: 자동:

    div {
    width: 300px;
    margin: auto;
    border: 1px solid red;
    }

***
### 상속 가치
이 예에서는 \<p class="ex1"> 요소의 왼쪽 여백이 상위 요소(\<div>)에서 상속되도록 합니다.

    예시
    상속 값의 사용:

    div {
    border: 1px solid red;
    margin-left: 100px;
    }

    p.ex1 {
    margin-left: inherit;
    }