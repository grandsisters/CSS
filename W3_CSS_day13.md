## CSS 배경 고정

***
### CSS 배경 고정
이 background-attachment속성은 배경 이미지가 스크롤되어야 하는지 또는 고정되어야 하는지를 지정합니다(나머지 페이지와 함께 스크롤되지 않음):

    예시
    배경 이미지가 고정되어야 함을 지정합니다.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: fixed;
    }


    예시
    배경 이미지가 페이지의 나머지 부분과 함께 스크롤되도록 지정합니다.

    body {
    background-image: url("img_tree.png");
    background-repeat: no-repeat;
    background-position: right top;
    background-attachment: scroll;
    }
