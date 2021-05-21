## 트랜지션 알아보기

<br>

트랜지션은 하나의 스타일을 완전히 다른 스타일로 바꾼다.

스타일이 바뀌는 시간을 조절하여 자바스크립트를 사용하지 않고도 애니메이션 효과를 낼 수 있다.

***
### 트랜지션이란

<br>

트랜지션은 웹 요소의 배경색을 바꾸거나 도형의 테두리를 사각형에서 원형으로 바꾸는 것처럼 스타일 속성이 바뀌는 것을 말한다.

웹 요소의 스타일 속성이 시간에 따라 바뀌는 것을 트랜지션이라고 한다.

***
### 트랜지션과 속성

|종류|설명|
|----|----|
|transition-property|트랜지션의 대상을 지정한다.|
|transition-duration|트랜지션을 실행할 시간을 지정한다.|
|transition-timing-function|트랜지션의 실행 형태를 지정한다.|
|transition-delay|트랜지션의 지연 시간을 지정한다.|
|transition|transition-property, transition-duration, transition-timing-function, transition-delay 속성을 한꺼번에 정한다.|

***
***

<br>

- 트랜지션의 대상을 지정하는 transition-property속성

    트랜지션을 만들려면 맨 먼저 transition-property속성을 사용하여 어떤 속성에 트랜지션을 적용할 것인지 대상을 지정해야 한다.

        - 기본형 transition-property: all | none | <속성 이름>


    |종류|설명|
    |----|----|
    |all|all값을 사용하거나 transition-property를 생략할 경우 요소의 모든 속성이 트랜지션 대상이 된다. 기본값|
    |none|트랜지션을 하는 동안 아무 속성도 바뀌지 않는다.|
    |속성 이름|트랜지션 효과를 적용할 속성을 지정한다. 예를 들어 배경색만 바꿀 것인지, width값을 바꿀 것인지 원하는 대상만 골라 지정할 수 있다. 속성이 여럿일 경우 쉼표(,)로 구분하여 나열한다.|

- 트랜지현의 진행 시간을 지정하는 transition-duration속성

    transition-property에서 트랜지션 대상을 지정했다면 다음으로 진행 시간을 지정해야 속성이 자연스럽게 바뀌는 애니메이션 효과를 만들 수 있다. 
    
    진행 시간을 transition-duration속성으로 지정할 수 있다. 

    지정할 수 있는 시간 단위는 초(second) 또는 밀리초(millisecond) 이다.

    트랜지션의 대상 속성이 여러 개라면 진행 시간도 쉼표(,)로 구분해서 여러 개를 지정할 수 있다.

    음숫값을 지정하면 0으로 간주한다.

        - 기본형 transition-duration: <시간>
