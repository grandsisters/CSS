## CSS 테두리 너비

***
### CSS 테두리 너비
이 border-width속성은 네 개의 테두리 너비를 지정합니다.

너비는 특정 크기(px, pt, cm, em 등)로 설정하거나 미리 정의된 세 가지 값(얇음, 중간 또는 두껍게) 중 하나를 사용하여 설정할 수 있습니다.

    예시
    다양한 테두리 너비 시연:

    p.one {
    border-style: solid;
    border-width: 5px;
    }

    p.two {
    border-style: solid;
    border-width: medium;
    }

    p.three {
    border-style: dotted;
    border-width: 2px;
    }

    p.four {
    border-style: dotted;
    border-width: thick;
    }

***
### 특정 측면 너비
border-width 속성은 하나에서 (상단 테두리 오른쪽 테두리, 아래쪽 테두리, 왼쪽 테두리) 네 개의 값을 가질 수 있습니다 :

    예시
    p.one {
    border-style: solid;
    border-width: 5px 20px; /* 5px top and bottom, 20px on the sides */
    }

    p.two {
    border-style: solid;
    border-width: 20px 5px; /* 20px top and bottom, 5px on the sides */
    }

    p.three {
    border-style: solid;
    border-width: 25px 10px 4px 35px; /* 25px top, 10px right, 4px bottom and 35px left */

설정값이 두개라면 위,아래 

설정값이 네개라면 시계방향으로 위,오른쪽,아래,왼쪽 순이다.