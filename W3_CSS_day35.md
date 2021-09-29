## CSS Text Spacing

---

### 텍스트 들여쓰기

text-indent속성은 텍스트의 첫 번째 줄의 들여 쓰기를 지정하는 데 사용됩니다 :

    예시
    p {
    text-indent: 50px;
    }

---

### 문자 간격

letter-spacing속성은 텍스트에서 문자 사이의 간격을 지정하는 데 사용됩니다.

다음 예는 문자 사이의 간격을 늘리거나 줄이는 방법을 보여줍니다.

    예시
    h1 {
    letter-spacing: 5px;
    }

    h2 {
    letter-spacing: -2px;
    }

---

### 라인 높이

line-height속성은 줄 사이의 간격을 지정하는 데 사용됩니다.

    예시
    p.small {
    line-height: 0.8;
    }

    p.big {
    line-height: 1.8;
    }

---

### 단어 간격

word-spacing속성은 텍스트의 단어 사이의 간격을 지정하는 데 사용됩니다.

다음 예는 단어 사이의 간격을 늘리거나 줄이는 방법을 보여줍니다.

    예시
    p.one {
    word-spacing: 10px;
    }

    p.two {
    word-spacing: -2px;
    }

---

### 여백

white-space속성은 요소 내부에 공백을 처리하는 방법을 지정합니다.

이 예는 요소 내부의 텍스트 줄 바꿈을 비활성화하는 방법을 보여줍니다.

    예시
    p {
    white-space: nowrap;
    }
