## CSS Specificity

---

### 특이성이란 무엇입니까?

동일한 요소를 가리키는 두 개 이상의 충돌하는 CSS 규칙이 있는 경우 브라우저는 몇 가지 규칙을 따라 어떤 규칙이 가장 구체적인지 결정하므로 우선합니다.

특정성을 요소에 궁극적으로 적용되는 스타일 선언을 결정하는 점수/순위로 생각하십시오.

범용 선택기(\*)는 특이성이 낮은 반면 ID 선택기는 매우 유니크합니다!

참고: 특정성은 CSS 규칙이 일부 요소에 적용되지 않는 일반적인 이유입니다.

---

### 특이성 계층

모든 선택자는 특이성 계층 구조에서 위치를 가집니다. 선택기의 특이성 수준을 정의하는 네 가지 범주가 있습니다.

인라인 스타일 - 인라인 스타일은 스타일을 지정할 요소에 직접 첨부됩니다. 예: \<h1 style="color: #ffffff;">.

ID - ID는 #navbar와 같은 페이지 요소의 고유 식별자입니다.

클래스, 속성 및 유사 클래스 - 이 범주에는 .classes, [속성] 및 :hover, :focus 등과 같은 유사 클래스가 포함됩니다.

요소 및 유사 요소 - 이 범주에는 h1, div, :before 및 :after와 같은 요소 이름 및 유사 요소가 포함됩니다.

---

### 특이성을 계산하는 방법?

특이도 계산 방법을 기억하십시오!

0에서 시작하여 스타일 속성에 대해 1000을 추가하고 각 ID에 대해 100을 추가하고 각 속성, 클래스 또는 의사 클래스에 대해 10을 추가하고 각 요소 이름 또는 의사 요소에 대해 1을 추가합니다.

다음 세 가지 코드 조각을 고려하십시오.

    예시
    A: h1
    B: #content h1
    C: <div id="content"><h1 style="color: #ffffff">Heading</h1></div>

    A의 특이도는 1(요소 1개)
    B의 특이도는 101(ID 참조 1개 및 요소 1개)
    C의 특이도는 1000(인라인 스타일링)

1 < 101 < 1000이므로 세 번째 규칙(C)이 더 높은 수준의 특이도를 가지므로 적용됩니다.

---

### 특이성 규칙

동일한 특이성: 최신 규칙이 카운트 - 동일한 규칙이 외부 스타일 시트에 두 번 작성되면 스타일 시트의 하위 규칙이 스타일을 지정할 요소에 더 가깝기 때문에 다음과 같이 적용됩니다.

    예시
    h1 {background-color: yellow;}
    h1 {background-color: red;}

후자의 규칙이 항상 적용됩니다.

<br />

ID 선택자는 속성 선택자보다 특이성이 높습니다 . 다음 세 가지 코드 라인을 보십시오.

    예시
    div#a {background-color: green;}
    #a {background-color: yellow;}
    div[id=a] {background-color: blue;}

첫 번째 규칙은 다른 두 규칙보다 더 구체적이며 적용됩니다.

<br />

상황별 선택기는 단일 요소 선택기보다 더 구체적입니다 . 포함된 스타일 시트는 스타일을 지정할 요소에 더 가깝습니다. 따라서 다음 상황에서

    예시
    From external CSS file:
    #content h1 {background-color: red;}

    In HTML file:
    <style>
    #content h1 {
    background-color: yellow;
    }
    </style>

후자의 규칙이 적용됩니다.

<br />

클래스 선택기는 여러 요소 선택기를 능가합니다. .intro와 같은 클래스 선택기는 h1, p, div 등을 능가합니다.

    예시
    .intro {background-color: yellow;}
    h1 {background-color: red;}

유니버설 셀렉터와 상속된 값은 0 - * 의 특이성을 가지며 본문 *과 유사한 것은 0의 특이성을 갖습니다. 상속된 값의 특이도도 0입니다.
