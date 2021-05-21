### 트랜지션의 속도 곡선을 지정하는 transition-timing-function 속성

<br>

transition-timing-function 속성을 사용하면 트랜지션 효과의 시작, 중간, 끝에서 속도를 지정해 전체 속도 곡선을 만들 수 있다.

속도 곡선은 미리 정해진 키워드나 베지에 곡선을 이용해 표현한다.

    - 기본형 transition-timing-function: linear | ease | ease-in | ease-out | ease-in-out | cubic-bezier(n, n, n, n)

|종류|설명|
|----|----|
|ease|처음에는 천천히 시작하고 점점 빨라지다가 마지막엔 천천히 끝낸다. 기본값|
|linear|시작부터 끝까지 똑같은 속도로 진행한다.|
|ease-in|느리게 시작한다.|
|ease-out|느리게 끝낸다.|
|ease-in-out|느리게 시작하고 느리게 끝낸다.|
|cubic-bezier(n, n, n, n)|베지에 함수를 정의해서 사용한다. 이때 n값은 0~1 사이만 사용할 수 있다.|

***
***

- 트랜지션의 지연 시간을 설정하는 transition-delay 속성

    transition-delay 속성은 트랜지션 효과를 언제부터 시작할 것인지 설정한다. 
    
    이 속성을 사용하면 지정한 시간만큼 기다렸다가 트랜지션이 시작된다.

    사용할 수 있는 값은 초(s)나 밀리초(ms)이며, 기본값은 0이다.

        기본형 transition-delay: <시간>

- 트랜지션의 속성을 한꺼번에 표기하는 transition 속성

    트랜지션의 적용 대산이 전체이고 각각의 진행 시간이 같다면 transition 속성으로 한꺼번에 지정하는 것이 편리하다.

        -기본형 transition: <transition-property값> | <transition-duration값> | <transition-timing-function값> | <transition-delay값> 

    속성값을 작성하는 순서는 상관이 없다. 다만 시간값을 사용하는 속성이 2개(진행 시간, 지연 시간)이므로 시간값이 2개 있다면 앞에 오는 시간값을 transition-duration 속성으로, 뒤에 오는 시간값은 transition-delay 속성으로 간주한다.  