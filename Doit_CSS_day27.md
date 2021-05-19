### 요소를 회전시키는 rotate() 함수

<br>

2차원 rotate() 함수

요소를 회전시키는 rotate() 함수는 2차원 회전과 3차원 회전에서 모두 사용할 수 있다.

rotate() 함수를 2차원에서 사용할 때는 각도만 지정하면 된다.

함수는 웹 요소를 지정한 각도만큼 오른쪽(시계 방향)이나 왼쪽(시계 반대 방향)으로 회전시킨다.

    - 기본형 transform: rotate(각도)

rotate() 함수에서 지정할 수 있는 각도의 값은 일반적인 각도(degree)나 래디안(radian)을 사용하는데, 이때 1래디안은 180도/𝝅를 의미한다.

<br>

3차원 rotate() 함수

3차원 rotate()함수는 다음과 같이 x축이나 y축, z축을 기준으로 회전시킵니다.

    - 기본형 transform: rotate(rx, ry, 각도)
             transform: rotate3d(rx, ry, rz, 각도)
             transform: rotateX(각도)
             transform: rotateY(각도)
             transform: rotateZ(각도)

이때 perspective 속성을 함께 사용해서 원근감을 추가해 주면 회전 형태를 입체적으로 표현 할 수 있다.

perspective 속성은 3차원 변형에서 사용하는데, 원래 있던 위치에서 사용자가 있는 방향이나 혹은 반대 방향으로 잡아당기거나 밀어내어 원금감을 표현한다.

perspective 속성에서 사용하는 값은 0보다 커야 하며, 원래 있던 위치에서 사용자가 있는 쪽으로 얼마나 이동 하는지를 픽셀 크기로 나타낸다. 값이 클수록 사용자로부터 멀어진다.

이때 주의할 점은 perspective 속성은 변형하는 요소가 아니라 변형하는 요소의 부모 요소에 정의해아 한다는 것이다.

***
### 요소를 비틀어 왜곡하는 skew() 함수

<br>

skew() 함수는 지정한 각도만큼 요소를 비틀어 왜곡한다. 이때 양쪽 방향으로 비틀거나 한쪽 방향으로만 비틀 수도 있다.

    - 기본형 transform: skew(x각도, y각도)
             transform: skewX(x각도)
             transform: skewY(y각도)


1) transform: skew(x각도, y각도)
:첫 번째 값은 x축을 기준으로 비트는 각도이고, 두 번째 값은 y축을 기준으로 비트는 각도이다. 두 번째 값이 주어지지 않으면 y축 각도를 0으로 간주한다.

2) transform: skewX(x각도)
:x축을 기준으로 주어진 각도만큼 비튼다.

3) transform: skewY(y각도)
:y축을 기준으로 주어진 각도만큼 비튼다.