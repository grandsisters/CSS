### 웹 요소를 이동시키는 translate() 함수

<br>

translate() 함수는 x축이나 y축 또는 양쪽 방향으로 이동할 거리를 지정하면 해당 요소가 지정한 크기만큼 이동한다.

translate()함수에서 사용하는 형식은 다음과 같다.

    - 기본형 transform: translate(tx, ty)
             transform: translate3d(tx, ty, tz)
             transform: translateX(tx)
             transform: translateY(ty)
             transform: translateZ(tz) 


1) transform: translate(tx, ty)
:x축으로 tz만큼, y축으로 ty만큼 이동한다. tx와 ty 2가지 값을 사용하지만 ty값이 주어지지 않으면 0으로 간주한다.

2) transform: translate3d(tx, ty, tz)
:x축으로 tx만큼, y축으로 ty만큼, 그리고 z축(앞뒤)으로 tz만큼 이동한다.

3) transform: translateX(tx)
:x축으로 tx만큼 이동한다.

4) transform: translateY(ty)
:y축으로 ty만큼 이동한다.

5) transform: translateZ(tz)
:z축으로 tz만큼 이동한다.

***
### 요소를 확대, 축소하는 scale()함수

<br>

scale() 함수는 웹 요소를 지정한 크기만큼 확대하거나 축소한다.

scale() 함수를 사용하는 형식은 다음과 같다. 괄호 안의 값(sx, sy, sz)이 1보다 크면 확대되고 1보다 작으면 축소된다.

    - 기본형 transform: scale(sx, sy)
             transform: scale3d(sx, sy, sz)
             transform: scaleX(sx)
             transform: scaleY(sy)
             transform: scaleZ(sz)

1) transform: scale(sx, sy)
:x축으로 sx만큼, y축으로 sy만큼 확대합니다. 값이 하나뿐일 경우에는 x, y에 같은 값을 적용한다. 예를 들어 scale(2)는 scale(2, 2)와 같은 함수이며, 요소를 2배로 확대한다.

2) transform: scale3d(sx, sy, sz)
:x축으로 sx만큼, y축으로 sy만큼, 그리고 z축으로 sz만큼 확대한다.

3) transform: scaleX(sx)
:x축으로 sx만큼 확대한다.

4) transform: scaleY(sy)
:y축으로 sy만큼 확대한다.

5) transform: scaleZ(sz)
:z축으로 sz만큼 확대한다.