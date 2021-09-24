## CSS 테두리 측면

***
### CSS 테두리 - 개별면
이전 페이지의 예에서 각 면에 대해 다른 테두리를 지정할 수 있음을 확인했습니다.

CSS에는 각 테두리(위, 오른쪽, 아래, 왼쪽)를 지정하는 속성도 있습니다.

    예시
    p {
    border-top-style: dotted;
    border-right-style: solid;
    border-bottom-style: dotted;
    border-left-style: solid;
    }

작동원리:

테두리 스타일 속성에 네 가지 값이 있는 경우:

- border-style: dotted solid double dashed;
    - 상단 테두리가 점선
    - 오른쪽 테두리가 솔리드
    - 하단 테두리는 이중
    - 왼쪽 테두리가 점선

테두리 스타일 속성에 세 가지 값이 있는 경우:

- border-style: dotted solid double;
    - 상단 테두리가 점선
    - 오른쪽과 왼쪽 테두리가 솔리드
    - 하단 테두리는 이중


테두리 스타일 속성에 두 가지 값이 있는 경우:

- border-style: dotted solid;
    - 상단 및 하단 테두리가 점으로 표시됩니다.
    - 오른쪽과 왼쪽 테두리가 솔리드


테두리 스타일 속성에 한 가지 값이 있는 경우:

- border-style: dotted;
    - 네 개의 테두리가 모두 점으로 표시됩니다.

    예시
    /* Four values */
    p {
    border-style: dotted solid double dashed;
    }

    /* Three values */
    p {
    border-style: dotted solid double;
    }

    /* Two values */
    p {
    border-style: dotted solid;
    }

    /* One value */
    p {
    border-style: dotted;
    }

테두리 스타일 속성은 위의 예에서 사용됩니다. 

그러나 테두리 너비 및 테두리 색상으로도 작동합니다.