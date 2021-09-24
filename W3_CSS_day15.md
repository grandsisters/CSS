## CSS Borders

CSS 테두리 속성을 사용하면 요소 테두리의 스타일, 너비 및 색상을 지정할 수 있습니다.

***
### CSS 테두리 스타일
border-style디스플레이 테두리 속성 지정은 어떤 종류.

다음 값이 허용됩니다.

- dotted - 점선 테두리를 정의합니다.
- dashed - 점선 테두리를 정의합니다.
- solid - 단색 테두리를 정의합니다.
- double - 이중 테두리 정의
- groove- 3D 홈 테두리를 정의합니다. 효과는 테두리 색상 값에 따라 다릅니다.
- ridge- 3D 융기된 테두리를 정의합니다. 효과는 테두리 색상 값에 따라 다릅니다.
- inset- 3D 삽입 테두리를 정의합니다. 효과는 테두리 색상 값에 따라 다릅니다.
- outset- 3D 아웃셋 테두리를 정의합니다. 효과는 테두리 색상 값에 따라 다릅니다.
- none - 경계를 정의하지 않음
- hidden - 숨겨진 테두리를 정의합니다.
- border-style속성은 네가지 값 중의 하나 (상단 테두리 오른쪽 테두리, 아래쪽 테두리, 왼쪽 테두리) 할 수 있습니다.

    예시
    다양한 테두리 스타일 시연:

    p.dotted {border-style: dotted;}

    p.dashed {border-style: dashed;}

    p.solid {border-style: solid;}

    p.double {border-style: double;}

    p.groove {border-style: groove;}

    p.ridge {border-style: ridge;}

    p.inset {border-style: inset;}

    p.outset {border-style: outset;}

    p.none {border-style: none;}

    p.hidden {border-style: hidden;}

    p.mix {border-style: dotted dashed solid double;}
    


참고: OTHER CSS 테두리 속성은 border-style속성이 설정 되지 않는 한 아무 효과도 없습니다 !