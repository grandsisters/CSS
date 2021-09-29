## CSS Text

CSS에는 텍스트 서식을 지정하는 많은 속성이 있습니다.

---

### 텍스트 색상

color속성은 텍스트의 색상을 설정하는 데 사용됩니다. 색상은 다음에 의해 지정됩니다.

- 색상 이름 - "빨간색"과 같은
- 16진수 값 - 예: "#ff0000"
- RGB 값 - "rgb(255,0,0)"

페이지의 기본 텍스트 색상은 본문 선택기에서 정의됩니다.

    예시
    body {
    color: blue;
    }

    h1 {
    color: green;
    }

참고: W3C 호환 CSS의 경우: color속성을 정의하는 경우 background-color도 정의해야 합니다.

---

### 텍스트 색상 및 배경 색상

이 예에서는 background-color속성과 color속성을 모두 정의합니다.

    예시
    body {
    background-color: lightgrey;
    color: blue;
    }

    h1 {
    background-color: black;
    color: white;
    }

    div {
    background-color: blue;
    color: white;
    }
