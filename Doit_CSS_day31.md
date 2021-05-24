- 애니메이션의 방향을 지정하는 animation-direction 속성

    애니메이션은 한 번 실행하고 나면 처음 상태로 되돌아간다.

    이때 animation-direction 속성을 사용하면 원래 상태로 돌아가거나 애니메이션을 반대 방향으로 한 번 더 실행하도록 할 수도 있다.

        - 기본형 animation-direction: normal | alternate

    |종류|설명|
    |----|----|
    |normal|애니메이션을 끝까지 실해하면 원래 위치로 돌아간다. 기본값|
    |alternate|애니메이션을 끝까지 실행하면 왔던 방향으로 되돌아가면서 애니메이션을 실행한다.|

- 반복 횟수를 지정하는 animation-iteration-count 속성

    상황에 따라 애니메이션을 반복해서 보여 줘야 할 때는 animation-iteration-count 속성을 사용해 반복 횟수를 정한다.

        - 기본형 animation-iteration-count: <숫자> | infinite
    
    |종류|설명|
    |----|----|
    |숫자|애니메이션의 반복 횟수를 정한다.|
    |infinite|애니메이션을 무한 반복한다.|

- 애니메이션의 속도 곡선을 지정하는 animation-timing-function 속성

    트랜지션과 마찬가지로 animation에서도 애니메이션의 시작, 중간, 끝에서 속도를 지정하여 전체 속도 곡선을 만들 수 있다.

        - 기본형 animation-timing-function: linear | ease | ease-in | ease-out | ease-in-out | cubic-bezier(n, n, n, n)

- 애니메이션의 속성을 한꺼번에 표기하는 animation 속성

    animation 관련 속성을 한 줄씩 따로따로 작성하지 않고 한꺼번에 표기하는 방법을 알아보자.

    주의할 점은 애니메이션 속성을 사용할 때 animation-duration 속성을 반드시 표기해야 한다는 것이다.

    애니메이션 실행 시간을 지정하지 않으면 기본값으로 0이 적용되어 애니메이션 효과를 볼 수 없기 때문이다.

        - 기본형 animation: <animation-name> | <animation-duration> |
                            <animation-timing-function> | <animation-delay> |
                            <animation-iteration-count> | <animation-direction>

