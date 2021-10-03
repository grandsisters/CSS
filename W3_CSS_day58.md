## CSS Layout - display: inline-block

---

### display: inline-block

display:inline 과 비교하여 가장 큰 차이점은 display: inline-block을 사용하면 요소에 너비와 높이를 설정할 수 있습니다.

또한 display: inline-block의 경우 상단 및 하단 여백/패딩이 고려되지만 디스플레이: 인라인/패딩은 그렇지 않습니다.

display: block과 비교하여 가장 큰 차이점은 디스플레이입니다. 인라인 블록은 요소 뒤에 줄 바꿈을 추가하지 않으므로 요소가 다른 요소 옆에 있을 수 있습니다.

다음 예제는 인라인, display: inline-block 및 display: block의 다양한 표시 동작을 보여줍니다.

    예시
    span.a {
    display: inline; /* the default for span */
    width: 100px;
    height: 100px;
    padding: 5px;
    border: 1px solid blue;
    background-color: yellow;
    }

    span.b {
    display: inline-block;
    width: 100px;
    height: 100px;
    padding: 5px;
    border: 1px solid blue;
    background-color: yellow;
    }

    span.c {
    display: block;
    width: 100px;
    height: 100px;
    padding: 5px;
    border: 1px solid blue;
    background-color: yellow;
    }

---

### 인라인 블록을 사용하여 탐색 링크 만들기

display: inline-blocl의 일반적인 용도 중 하나는 목록 항목을 세로 대신 가로로 표시하는 것입니다.

다음 예에서는 수평 탐색 링크를 생성합니다.

    예시
    .nav {
    background-color: yellow;
    list-style-type: none;
    text-align: center;
    padding: 0;
    margin: 0;
    }

    .nav li {
    display: inline-block;
    font-size: 20px;
    padding: 20px;
    }
