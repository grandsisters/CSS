## CSS Pseudo-classes

---

### 의사 클래스는 무엇입니까?

의사 클래스는 요소의 특수 상태를 정의하는 데 사용됩니다.

예를 들어 다음과 같은 용도로 사용할 수 있습니다.

- 사용자가 요소 위에 마우스를 놓을 때 요소 스타일 지정
- 방문한 링크와 방문하지 않은 링크를 다르게 스타일 지정
- 포커스를 받을 때 요소 스타일 지정

---

### 통사론

의사 클래스의 구문:

    selector:pseudo-class {
    property: value;
    }

---

### 앵커 유사 클래스

링크는 다음과 같은 다양한 방식으로 표시될 수 있습니다.

    예시
    /_ unvisited link _/
    a:link {
    color: #FF0000;
    }

    /_ visited link _/
    a:visited {
    color: #00FF00;
    }

    /_ mouse over link _/
    a:hover {
    color: #FF00FF;
    }

    /_ selected link _/
    a:active {
    color: #0000FF;
    }

주 : a:hover 뒤에 와야합니다 a:link및 a:visited 위해 CSS 정의에하는 것이 효과적! a:active효과를 보려면 a:hoverCSS 정의 뒤에 와야 합니다 ! 의사 클래스 이름은 대소문자를 구분하지 않습니다.

---

### 의사 클래스 및 HTML 클래스

의사 클래스는 HTML 클래스와 결합할 수 있습니다.

예제의 링크 위로 마우스를 가져가면 색상이 변경됩니다.

    예시
    a.highlight:hover {
    color: #ff0000;
    }

---

### \<div>에 마우스를 가져갑니다.

:hover\<div> 요소에 의사 클래스를 사용하는 예 :

    예시
    div:hover {
    background-color: blue;
    }

---

### 간단한 툴팁 호버

\<div> 요소 위로 마우스를 가져가면 툴팁과 같은 \<p> 요소가 표시됩니다.

    예시
    p {
    display: none;
    background-color: yellow;
    padding: 20px;
    }

    div:hover p {
    display: block;
    }

---

### CSS - :first-child 의사 클래스

:first-child 의사 클래스는 다른 요소의 첫 번째 자식 인 지정된 요소와 일치합니다.

<br />

### 첫 번째 \<p> 요소와 일치

다음 예에서 선택기는 모든 요소의 첫 번째 자식인 모든 \<p> 요소와 일치합니다.

    예시
    p:first-child {
    color: blue;
    }

<br />

### 모든 \<p> 요소의 첫 번째 \<i> 요소와 일치

다음 예에서 선택기는 모든 \<p> 요소의 첫 번째 \<i> 요소와 일치합니다.

    예시
    p i:first-child {
    color: blue;
    }

<br />

### 모든 첫 번째 자식 \<p> 요소의 모든 \<i> 요소와 일치

다음 예에서 선택기는 다른 요소의 첫 번째 자식인 \<p> 요소의 모든 \<i> 요소와 일치합니다.

    예시
    p:first-child i {
    color: blue;
    }

---

### CSS - :lang 의사 클래스

:lang의사 클래스는 다른 언어에 대한 특별한 규칙을 정의 할 수 있습니다.

아래 예 :lang에서 lang="no"를 사용하여 \<q> 요소에 대한 따옴표를 정의합니다.

    예시

    <html>
    <head>
    <style>
    q:lang(no) {
    quotes: "~" "~";
    }
    </style>
    </head>
    <body>

    <p>Some text <q lang="no">A quote in a paragraph</q> Some text.</p>

    </body>
    </html>

---

### 모든 CSS 의사 클래스

| Selector             | Example               | Example description                                                                                    |
| -------------------- | --------------------- | ------------------------------------------------------------------------------------------------------ |
| :active              | a:active              | Selects the active link                                                                                |
| :checked             | input:checked         | Selects every checked \<input> element                                                                 |
| :disabled            | input:disabled        | Selects every disabled \<input> element                                                                |
| :empty               | p:empty               | Selects every \<p> element that has no children                                                        |
| :enabled             | input:enabled         | Selects every enabled \<input> element                                                                 |
| :first-child         | p:first-child         | Selects every \<p> elements that is the first child of its parent                                      |
| :first-of-type       | p:first-of-type       | Selects every \<p> element that is the first \<p> element of its parent                                |
| :focus               | input:focus           | Selects the \<input> element that has focus                                                            |
| :hover               | a:hover               | Selects links on mouse over                                                                            |
| :in-range            | input:in-range        | Selects \<input> elements with a value within a specified range                                        |
| :invalid             | input:invalid         | Selects all \<input> elements with an invalid value                                                    |
| :lang(language)      | p:lang(it)            | Selects every \<p> element with a lang attribute value starting with "it"                              |
| :last-child          | p:last-child          | Selects every \<p> elements that is the last child of its parent                                       |
| :last-of-type        | p:last-of-type        | Selects every \<p> element that is the last \<p> element of its parent                                 |
| :link                | a:link                | Selects all unvisited links                                                                            |
| :not(selector)       | :not(p)               | Selects every element that is not a \<p> element                                                       |
| :nth-child(n)        | p:nth-child(2)        | Selects every \<p> element that is the second child of its parent                                      |
| :nth-last-child(n)   | p:nth-last-child(2)   | Selects every \<p> element that is the second child of its parent, counting from the last child        |
| :nth-last-of-type(n) | p:nth-last-of-type(2) | Selects every \<p> element that is the second \<p> element of its parent, counting from the last child |
| :nth-of-type(n)      | p:nth-of-type(2)      | Selects every \<p> element that is the second \<p> element of its parent                               |
| :only-of-type        | p:only-of-type        | Selects every \<p> element that is the only \<p> element of its parent                                 |
| :only-child          | p:only-child          | Selects every \<p> element that is the only child of its parent                                        |
| :optional            | input:optional        | Selects \<input> elements with no "required" attribute                                                 |
| :out-of-range        | input:out-of-range    | Selects \<input> elements with a value outside a specified range                                       |
| :read-only           | input:read-only       | Selects \<input> elements with a "readonly" attribute specified                                        |
| :read-write          | input:read-write      | Selects \<input> elements with no "readonly" attribute                                                 |
| :required            | input:required        | Selects \<input> elements with a "required" attribute specified                                        |
| :root                | root                  | Selects the document's root element                                                                    |
| :target              | #news:target          | Selects the current active #news element (clicked on a URL containing that anchor name)                |
| :valid               | input:valid           | Selects all \<input> elements with a valid value                                                       |
| :visited             | a:visited             | Selects all visited links                                                                              |

---

### 모든 CSS 유사 요소

| Selector       | Example         | Example description                                          |
| -------------- | --------------- | ------------------------------------------------------------ |
| ::after        | p::after        | Insert content after every \<p> element                      |
| ::before       | p::before       | Insert content before every \<p> element                     |
| ::first-letter | p::first-letter | Selects the first letter of every \<p> element               |
| ::first-line   | p::first-line   | Selects the first line of every \<p> element                 |
| ::selection    | p::selection    | Selects the portion of an element that is selected by a user |
