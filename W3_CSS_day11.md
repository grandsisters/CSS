## CSS 배경 이미지

***
### CSS 배경 이미지
background-image속성은 요소의 배경으로 사용하는 화상을 지정한다.

기본적으로 이미지는 전체 요소를 덮도록 반복됩니다.

    예시
    페이지의 배경 이미지 설정: 

    body {
    background-image: url("paper.gif");
    }


    예시
    이 예는 텍스트와 배경 이미지 의 잘못된 조합 을 보여줍니다 . 텍스트는 거의 읽을 수 없습니다. 

    body {
    background-image: url("bgdesert.jpg");
    }


참고: 배경 이미지 사용 시 텍스트에 방해가 되지 않는 이미지를 사용하세요.

배경 이미지는 \<p> 요소와 같은 특정 요소에 대해 설정할 수도 있습니다.

    예시
    p {
    background-image: url("paper.gif");
    }