## 변형 함수

|종류|설명|
|----|----|
|translate( )함수: 요소 이동하기|
|transform: translate(tx, ty)|지정한 크기만큼 x축과 y축으로 이동한다.|
|transform: translate(tx, ty, rz)|지정한 크기만큼 x축, y축, z축으로 이동한다.|
|transform: translate(tx)|지정한 크기만큼 x축으로 이동한다.|
|transform: translate(ty)|지정한 크기만큼 y축으로 이동한다.|
|transform: translate(tz)|지정한 크기만큼 z축으로 이동한다.|


***
<br>

|종류|설명|
|----|----|
|translate( )함수: 요소 확대,축소하기|
|transform: scale(sx, sy)|지정한 크기만큼 x축, y축으로 확대,축소 한다.|
|transform: scale(sx, sy, sz)|지정한 크기만큼 x축, y축으로 확대,축소 한다.|
|transform: scaleX(sx)|지정한 크기만큼 x축으로 확대,축소 한다.|
|transform: scaleY(sy)|지정한 크기만큼 y축으로 확대,축소 한다.|
|transform: scaleZ(sz)|지정한 크기만큼 z축으로 확대,축소 한다.|


***
<br>

|종류|설명|
|----|----|
|rotate( )함수 :요소 회전하기|
|transform: rotate(각도)|지정한 각도만큼 회전한다.|
|transform: rotateX(각도)|x축을 기준으로 지정한 각도만큼 회전한다.|
|transform: rotateY(각도)|y축을 기준으로 지정한 각도만큼 회전한다.|
|transform: rotateZ(각도)|z축을 기준으로 지정한 각도만큼 회전한다.|
|transform: rotate3d(rx, ry, rz, 각도)|x축과 y축, z축을 기준으로 지정한 각도만큼 회전한다.|


***
<br>

|종류|설명|
|----|----|
|skew( )함수: 요소 비틀기|
|transform: skew(ax, ay)|지정한 각도만큼 x축과 y축으로 비튼다.|
|transform: skewX(ax)|지정한 각도만큼 x축으로 비튼다.|
|transform: skewY(ay)|지정한 각도만큼 y축으로 비튼다.|

***
## 트랜지션 속성

|종류|설명|
|----|----|
|transition-property|트랜지션 적용 대상을 지정한다. 기본값은 all이다.|
|transition-duration|트랜지션의 실행 시간을 지정한다. 단위는 s(초)이고 기본값은 0이다.|
|transition-timing-function|트랜지션의 실행 형태를 지정한다.|
|transition-delay|트랜지션의 지연 시간을 지정한다. 단위는 s(초)이고 기본값은 0이다.|
|transition|transition-property, transition-duration, transition-timing-function, transition-delay 속성을 한꺼번에 지정한다.|

***
## 애니메이션 속성

|종류|설명|
|----|----|
|@keyframes|애니메이션이 바뀌는 지점을 설정한다.|
|animation-delay|애니메이션의 시작 시간을 지정한다.|
|animation-direction|애니메이션을 종료한 뒤 처음부터 시작할지, 반대 방향으로 진행할지 지정한다.|
|animation-duration|애니메이션의 실행 시간을 지정한다. 단위는 s(초)이다.|
|animation-iteration-count|애니메이션의 반복 횟수를 지정한다.|
|animation-name|@ketsframe로 설정해 놓은 중간 상태를 지정한다.|
|animation-timing-function|키프레임의 전화 형태를 지정한다.|
|animation|animation 속성을 한꺼번에 묶어서 지정한다.|