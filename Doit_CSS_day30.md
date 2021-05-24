## 애니메이션 알아보기

<br>

CSS3의 animation 속성을 이용하면 트랜지션보다 더 쉽게 애니메이션을 만들 수 있다.

***
### CSS 애니메이션에서 사용하는 속성

<br>

animation 속성을 사용하면 자바스크립트를 사용하지 않고도 웹 요소에 애니메이션을 추가할 수 있다.

animation 속성은 특정 지점에서 스타일을 바꾸면서 애니메이션을 만드는데, 이렇게 애니메이션 중간에 스타일이 바뀌는 지점을 키프레임(keyframe)이라고 한다.

키프레임은 @keyframes 속성으로 정의하고, animation 속성과 그 하위 속성을 이용해서 애니메이션의 실행 시간이나 반복 여부 들을 지정한다.

|종류|설명|
|----|----|
|@keyframes|애니메이션이 바뀌는 지점을 지정한다.|
|animation-delay|애니메이션의 시작 시간을 지정한다.|
|animation-direction|애니메이션을 종료한 뒤 처음부터 시작할지, 역방향으로 진행할지 지정한다.|
|animation-duration|애니메이션의 실행 시간을 지정한다.|
|animation-iteration-count|애니메이션의 반복 횟수를 지정한다.|
|animation-name|@keyframes로 설절해 놓은 중간 상태를 지정한다.|
|animation-timing-function|키프레임의 전환 형태를 지정한다.|
|animation|animation 속성을 한꺼번에 묶어서 지정한다.|

***
***
<br>

- 애니메이션의 지점과 이름을 설정하는 @keyframes 속성, animation-name 속성

    애니메이션의 시작과 끝을 비롯하여 상태가 바뀌는 부분이 있다면 @keyframes 속성을 이용해 바뀌는 지점을 설정한다.

        - 기본형 @keyframes <이름> {
            <선택자> { <스타일> }
        } 
        
    또한 웹 문서에서는 애니메이션을 여러 개 정의할 수 있으므로 이름을 이용해 애니메이션을 구별해야 한다.

    이때 animation-name 속성으로 어떤 애니메이션을 사용할지 이름으로 구분한다.

        - 기본형 animation-name: <키프레임 이름> | none

    @keyframes 속성에서 사용하는 선택자는 스타일 속성값이 바뀌는 지점을 가리킨다.

    예를 들어 애니메이션의 중간 지점을 추가하려면 시작 위치를 0%, 끝 위치를 100%로 놓고 50% 위치에 키프레임을 추가하면 된다. 

    시작과 끝 위치만 사용하려면 0%, 100%와 같은 값 대신 from과 to라는 키워드를 사용해도 된다.

- 애니메이션의 실행 시간을 지정하는 animation-duration속성 

    animation-duration 속성은 애니메이션을 얼마 동안 재생할 것인지 설정한다.

    - 기본형 animation-duration: <시간>

    animation-duration 속성에서 사용할 수 있는 값은 초(s)나 밀리초(ms)와 같은 시간 단위이다.

    기본값은 0이므로 animation-duration 속성값을 정하지 않으면 애니메이션은 실행되지 않는다.
