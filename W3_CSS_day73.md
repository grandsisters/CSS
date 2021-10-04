## CSS Units

---

### CSS 단위

CSS에는 길이를 표현하는 몇 가지 다른 단위가 있습니다.

많은 CSS 속성은 너비, 여백, 패딩, 글꼴 크기 등과 같은 "길이" 값을 사용합니다.

길이는 10px, 2em 등과 같은 길이 단위 뒤에 오는 숫자입니다.

    예시
    px(픽셀)를 사용하여 다른 길이 값 설정:

    h1 {
    font-size: 60px;
    }

    p {
    font-size: 25px;
    line-height: 50px;
    }

참고: 숫자와 단위 사이에는 공백이 올 수 없습니다. 그러나 값이 0인 경우 단위를 생략할 수 있습니다.

일부 CSS 속성의 경우 음수 길이가 허용됩니다.

길이 단위에는 절대 및 상대 의 두 가지 유형이 있습니다 .

---

### 절대 길이

절대 길이 단위는 고정되어 있으며 이들 중 하나로 표현된 길이는 정확히 그 크기로 나타납니다.

화면 크기가 매우 다양하기 때문에 절대 길이 단위는 화면에서 사용하지 않는 것이 좋습니다. 그러나 인쇄 레이아웃과 같이 출력 매체가 알려진 경우 사용할 수 있습니다.

| Unit  | Description                  |
| ----- | ---------------------------- |
| cm    | centimeters                  |
| mm    | millimeters                  |
| in    | inches (1in = 96px = 2.54cm) |
| px \* | pixels (1px = 1/96th of 1in) |
| pt    | points (1pt = 1/72 of 1in)   |
| pc    | picas (1pc = 12 pt)          |

픽셀(px)은 시청 장치를 기준으로 합니다. 낮은 dpi 장치의 경우 1px는 디스플레이의 하나의 장치 픽셀(점)입니다. 프린터 및 고해상도 화면의 경우 1px는 여러 장치 픽셀을 의미합니다.

---

### 상대 길이

상대 길이 단위는 다른 길이 속성에 상대적인 길이를 지정합니다. 상대 길이 단위는 다른 렌더링 매체 사이에서 더 잘 확장됩니다.

| Unit | Description                                                                               |
| ---- | ----------------------------------------------------------------------------------------- |
| em   | Relative to the font-size of the element (2em means 2 times the size of the current font) |
| ex   | Relative to the x-height of the current font (rarely used)                                |
| ch   | Relative to width of the "0" (zero)                                                       |
| rem  | Relative to font-size of the root element                                                 |
| vw   | Relative to 1% of the width of the viewport\*                                             |
| vh   | Relative to 1% of the height of the viewport\*                                            |
| vmin | Relative to 1% of viewport's\* smaller dimension                                          |
| vmax | Relative to 1% of viewport's\* larger dimension                                           |
| %    | Relative to the parent element                                                            |

팁: em 및 rem 단위는 완벽하게 확장 가능한 레이아웃을 만드는 데 실용적입니다!

뷰포트 = 브라우저 창 크기. 뷰포트의 너비가 50cm이면 1vw = 0.5cm입니다.
