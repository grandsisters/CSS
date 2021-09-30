## CSS Web Safe Fonts

웹 안전 글꼴이란 무엇입니까?

웹 안전 글꼴은 모든 브라우저와 장치에 보편적으로 설치되는 글꼴입니다.

---

### 대체 글꼴

그러나 100% 완전히 웹에 안전한 글꼴은 없습니다. 글꼴을 찾을 수 없거나 제대로 설치되지 않았을 가능성이 항상 있습니다.

따라서 항상 대체 글꼴을 사용하는 것이 매우 중요합니다.

이는 font-family 속성 에 유사한 "백업 글꼴" 목록을 추가해야 함을 의미합니다 .

첫 번째 글꼴이 작동하지 않으면 브라우저는 다음 글꼴을 시도하고 다음 글꼴을 시도하는 식으로 계속됩니다.

항상 일반 글꼴 패밀리 이름으로 목록을 끝내십시오.

    예시
    여기에는 Tahoma, Verdana 및 sans-serif의 세 가지 글꼴 유형이 있습니다.
    두 번째 및 세 번째 글꼴은 첫 번째 글꼴을 찾을 수 없는 경우를 위한 백업입니다.

    p {
    font-family: Tahoma, Verdana, sans-serif;
    }

---

### HTML 및 CSS를 위한 최고의 웹 안전 글꼴

다음 목록은 HTML 및 CSS에 가장 적합한 웹 안전 글꼴입니다.

- Arial (sans-serif)
- Verdana (sans-serif)
- Helvetica (sans-serif)
- Tahoma (sans-serif)
- Trebuchet MS (sans-serif)
- Times New Roman (serif)
- Georgia (serif)
- Garamond (serif)
- Courier New (monospace)
- Brush Script MT (cursive)

---

### CSS Font Fallbacks

### 일반적으로 사용되는 글꼴 대체

다음은 5가지 일반 글꼴 패밀리로 구성된 몇 가지 일반적으로 사용되는 대체 글꼴입니다.

Serif
Sans-serif
Monospace
Cursive
Fantasy

참고: 웹사이트를 게시하기 전에 항상 다른 브라우저와 장치에서 글꼴이 어떻게 나타나는지 확인하고 항상 대체 글꼴을 사용하십시오!

팁: [사용 가능한 모든 Google 글꼴 과 사용 방법](https://www.w3schools.com/css/css_font_google.asp) 도 확인 하세요.
