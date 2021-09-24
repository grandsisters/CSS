## CSS 테두리 색상

***
### CSS 테두리 색상
border-color속성은 네 테두리의 색상을 설정하는 데 사용됩니다.

색상은 다음과 같이 설정할 수 있습니다.

- 이름 - "빨간색"과 같은 색상 이름을 지정합니다.
- HEX - "#ff0000"과 같은 HEX 값을 지정합니다.
- RGB - "rgb(255,0,0)"과 같은 RGB 값 지정
- HSL - "hsl(0, 100%, 50%)"와 같은 HSL 값을 지정합니다.
- 투명한(transparent)

참고 : 경우 border-color는 요소의 색상을 상속 설정되어 있지 않습니다.

    예시
    다양한 테두리 색상 시연:

    p.one {
    border-style: solid;
    border-color: red;
    }

    p.two {
    border-style: solid;
    border-color: green;
    }

    p.three {
    border-style: dotted;
    border-color: blue;
    }

***
### 특정 측면 색상
border-color속성은 네가지 값 중의 하나 (상단 테두리 오른쪽 테두리, 아래쪽 테두리, 왼쪽 테두리) 할 수 있습니다. 

    예시
    p.one {
    border-style: solid;
    border-color: red green blue yellow; /* red top, green right, blue bottom and yellow left */
    }

***
### 16진수 값
테두리 색상은 16진수 값(HEX)을 사용하여 지정할 수도 있습니다.

    예시
    p.one {
    border-style: solid;
    border-color: #ff0000; /* red */
    }

***
### RGB 값
또는 RGB 값을 사용하여:

    예시
    p.one {
    border-style: solid;
    border-color: rgb(255, 0, 0); /* red */
    }

***
### HSL 값
HSL 값을 사용할 수도 있습니다.

    예시
    p.one {
    border-style: solid;
    border-color: hsl(0, 100%, 50%); /* red */
    }
