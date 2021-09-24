## CSS 약식 테두리 속성

***
### CSS 테두리 - 약식 속성
이전 페이지에서 보았듯이 테두리를 다룰 때 고려해야 할 속성이 많이 있습니다.

코드를 줄이기 위해 하나의 속성에 모든 개별 테두리 속성을 지정할 수도 있습니다.

border속성은 다음 각 테두리 속성에 대한 약식 속성이다 :

- border-width
- border-style (필수)
- border-color


    예시
    p {
    border: 5px solid red;
    }


한 면에 대해서만 모든 개별 테두리 속성을 지정할 수도 있습니다.

    왼쪽 테두리
    p {
    border-left: 6px solid red;
    background-color: lightgrey;
    }

    하단 테두리
    p {
    border-bottom: 6px solid red;
    background-color: lightgrey;
    }