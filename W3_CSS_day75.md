## CSS The !important Rule

---

### !important란?

!importantCSS 의 규칙은 일반보다 속성/값에 더 많은 중요성을 추가하는 데 사용됩니다.

실제로 !important규칙 을 사용하면 해당 요소의 특정 속성에 대한 모든 이전 스타일 지정 규칙을 재정의합니다!

예를 살펴보겠습니다.

    예시
    #myid {
    background-color: blue;
    }

    .myclass {
    background-color: gray;
    }

    p {
    background-color: red !important;
    }

위의 예에서 ID 선택기와 클래스 선택기가 더 높은 특이성을 가지고 있더라도 세 단락 모두 빨간색 배경색을 갖습니다.

---

### Important About !important

!important 규칙을 재정의하는 유일한 방법은 소스 코드에 동일하거나 더 높은 특수성을 가진 선언에 다른 !important 규칙을 포함하는 것입니다. 여기서 문제가 시작됩니다! 이렇게 하면 CSS 코드가 혼동되고 디버깅이 어려워집니다. 특히 스타일시트가 큰 경우 더욱 그렇습니다.

여기에서 간단한 예제를 만들었습니다. CSS 소스 코드를 보면 어떤 색상이 가장 중요한지 명확하지 않습니다.

    예시
    #myid {
    background-color: blue !important;
    }

    .myclass {
    background-color: gray !important;
    }

    p {
    background-color: red !important;
    }

팁:!important 규칙 에 대해 아는 것이 좋지만 꼭 필요한 경우가 아니면 사용하지 마십시오.

---

### Maybe One or Two Fair Uses of !important

!important 사용 방법 중 하나는 다른 방법으로 재정의할 수 없는 스타일을 재정의해야 하는 경우입니다.

이는 CMS(Content Management System)에서 작업 중이고 CSS 코드를 편집할 수 없는 경우일 수 있습니다. 그런 다음 사용자 정의 스타일을 설정하여 일부 CMS 스타일을 재정의할 수 있습니다.

!important 또 다른 사용 방법은 페이지의 모든 단추를 특별히 찾고 싶다고 가정해 보십시오. 여기서 버튼은 회색 배경색, 흰색 텍스트, 일부 패딩 및 테두리로 스타일링됩니다.

    예시
    .button {
    background-color: #8c8c8c;
    color: white;
    padding: 5px;
    border: 1px solid black;
    }

버튼의 모양은 더 높은 특정성을 가진 다른 요소 안에 넣으면 때때로 변경될 수 있으며 속성이 충돌합니다. 다음은 이에 대한 예입니다.

    예시
    .button {
    background-color: #8c8c8c;
    color: white;
    padding: 5px;
    border: 1px solid black;
    }

    #myDiv a {
    color: red;
    background-color: yellow;
    }

모든 버튼이 동일한 모양을 갖도록 "강제"하려면 다음 !important 과 같이 버튼의 속성에 규칙을 추가할 수 있습니다 .

    예시
    .button {
    background-color: #8c8c8c !important;
    color: white !important;
    padding: 5px !important;
    border: 1px solid black !important;
    }

    #myDiv a {
    color: red;
    background-color: yellow;
    }
