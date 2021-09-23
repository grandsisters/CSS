## CSS 배경 이미지 반복

***
### CSS 배경 반복
기본적으로 background-image속성은 이미지를 가로 및 세로로 반복합니다.

일부 이미지는 가로 또는 세로로만 반복되어야 합니다. 그렇지 않으면 다음과 같이 이상하게 보일 것입니다.

    예시
    body {
    background-image: url("gradient_bg.png");
    }

위의 이미지를 가로로만( background-repeat: repeat-x;) 반복 하면 배경이 더 잘 보입니다.

    예시
    body {
    background-image: url("gradient_bg.png");
    background-repeat: repeat-x;
    }

팁: 이미지를 세로로 반복하려면 background-repeat: repeat-y;

***
### CSS 배경 반복: 반복 없음
배경 이미지를 한 번만 표시하는 것도 background-repeat속성에 의해 지정됩니다 .

    예시
    배경 이미지를 한 번만 표시:

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    }

위의 예에서 배경 이미지는 텍스트와 같은 위치에 배치됩니다. 

텍스트를 너무 방해하지 않도록 이미지의 위치를 ​​변경하고 싶습니다.

***
### CSS 배경 위치
background-position속성은 배경 이미지의 위치를 지정하는 데 사용됩니다.

    예시
    오른쪽 상단 모서리에 배경 이미지 배치: 

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    }