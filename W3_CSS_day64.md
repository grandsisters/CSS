## CSS Navigation Bar

---

### Navigation Bars

사용하기 쉬운 탐색 기능은 모든 웹 사이트에서 중요합니다.

CSS를 사용하면 지루한 HTML 메뉴를 멋진 탐색 모음으로 변환할 수 있습니다.

---

### Navigation Bar = List of Links

탐색 모음에는 표준 HTML이 기본으로 필요합니다.

우리의 예에서는 표준 HTML 목록에서 탐색 모음을 만들 것입니다.

탐색 모음은 기본적으로 링크 목록이므로 \<ul> 및 \<li> 요소를 사용하는 것이 완벽합니다.

    예시
    <ul>
    <li><a href="default.asp">Home</a></li>
    <li><a href="news.asp">News</a></li>
    <li><a href="contact.asp">Contact</a></li>
    <li><a href="about.asp">About</a></li>
    </ul>

이제 목록에서 글머리 기호와 여백 및 패딩을 제거해 보겠습니다.

    예시
    ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    }

설명된 예:

- list-style-type: none;- 불릿마크를 제거합니다. 탐색 모음에는 목록 마커가 필요하지 않습니다.
- 설정 margin: 0; 및 padding: 0; 브라우저 기본 설정을 제거하는
