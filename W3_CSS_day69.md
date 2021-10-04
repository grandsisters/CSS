## CSS 이미지 스프라이트

---

### 이미지 스프라이트

이미지 스프라이트는 단일 이미지에 넣은 이미지 모음입니다.

이미지가 많은 웹 페이지는 로드하는 데 오랜 시간이 걸리고 여러 서버 요청을 생성할 수 있습니다.

이미지 스프라이트를 사용하면 서버 요청 수가 줄어들고 대역폭이 절약됩니다.

---

### 이미지 스프라이트 - 간단한 예

세 개의 개별 이미지를 사용하는 대신 다음 단일 이미지("img_navsprites.gif")를 사용합니다.

<img src='https://www.w3schools.com/css/img_navsprites.gif'>

CSS를 사용하면 필요한 이미지의 일부만 표시할 수 있습니다.

다음 예에서 CSS는 "img_navsprites.gif" 이미지에서 표시할 부분을 지정합니다.

    예시
    #home {
    width: 46px;
    height: 44px;
    background: url(img_navsprites.gif) 0 0;
    }

설명된 예:

- \<img id="home" src="img_trans.gif">- src 속성은 비워둘 수 없기 때문에 작은 투명 이미지만 정의합니다. 표시된 이미지는 CSS에서 지정한 배경 이미지가 됩니다.
- width: 46px; height: 44px; - 사용하려는 이미지 부분을 정의합니다.
- background: url(img_navsprites.gif) 0 0; - 배경 이미지 및 위치 정의(왼쪽 0px, 위쪽 0px)

이것은 이미지 스프라이트를 사용하는 가장 쉬운 방법입니다. 이제 링크와 호버 효과를 사용하여 확장하려고 합니다.

---

### 이미지 스프라이트 - 탐색 목록 만들기

탐색 목록을 만들기 위해 스프라이트 이미지("img_navsprites.gif")를 사용하려고 합니다.

링크가 될 수 있고 배경 이미지도 지원하기 때문에 HTML 목록을 사용합니다.

    예시
    #navlist {
    position: relative;
    }

    #navlist li {
    margin: 0;
    padding: 0;
    list-style: none;
    position: absolute;
    top: 0;
    }

    #navlist li, #navlist a {
    height: 44px;
    display: block;
    }

    #home {
    left: 0px;
    width: 46px;
    background: url('img_navsprites.gif') 0 0;
    }

    #prev {
    left: 63px;
    width: 43px;
    background: url('img_navsprites.gif') -47px 0;
    }

    #next {
    left: 129px;
    width: 43px;
    background: url('img_navsprites.gif') -91px 0;
    }

설명된 예:

- #navlist {position:relative;} - 위치는 내부에 절대 위치를 허용하도록 상대적으로 설정됩니다.
- #navlist li {margin:0;padding:0;list-style:none;position:absolute;top:0;} - 여백과 패딩이 0으로 설정되고 목록 스타일이 제거되고 모든 목록 항목이 절대 위치에 배치됩니다.
- #navlist li, #navlist a {height:44px;display:block;} - 모든 이미지의 높이는 44px입니다.

이제 각 특정 부품에 대한 위치 지정 및 스타일 지정을 시작합니다.

- #home {left:0px;width:46px;} - 왼쪽 끝까지 배치, 이미지 너비는 46px
- #home {background:url(img_navsprites.gif) 0 0;} - 배경 이미지와 위치 정의(왼쪽 0px, 위쪽 0px)
- #prev {left:63px;width:43px;} - 오른쪽으로 63px 위치(#home width 46px + 항목 사이의 추가 공간), 너비는 43px입니다.
- #prev {background:url('img_navsprites.gif') -47px 0;} - 배경 이미지를 오른쪽으로 47px 정의합니다(#home 너비 46px + 1px 줄 구분선).
- #next {left:129px;width:43px;}- 오른쪽으로 129px 위치(#prev의 시작은 63px + #prev width 43px + 추가 공백), 너비는 43px입니다.
- #next {background:url('img_navsprites.gif') -91px 0;} - 배경 이미지를 오른쪽으로 91px 정의합니다. (#home width 46px + 1px line divider + #prev width 43px + 1px line Divider )

---

### 이미지 스프라이트 - 호버 효과

이제 탐색 목록에 호버 효과를 추가하려고 합니다.

    팁 ::hover 선택은 링크에서뿐만 아니라 모든 요소에 사용할 수 있습니다.

새 이미지("img_navsprites_hover.gif")에는 3개의 탐색 이미지와 호버 효과에 사용할 3개의 이미지가 포함되어 있습니다.

<img src='https://www.w3schools.com/css/img_navsprites_hover.gif'>

이것은 6개의 개별 파일이 아닌 하나의 단일 이미지이기 때문에 사용자가 이미지 위로 마우스를 가져갈 때 로딩 지연 이 없습니다 .

호버 효과를 추가하기 위해 세 줄의 코드만 추가합니다.

    예시
    #home a:hover {
    background: url('img_navsprites_hover.gif') 0 -45px;
    }

    #prev a:hover {
    background: url('img_navsprites_hover.gif') -47px -45px;
    }

    #next a:hover {
    background: url('img_navsprites_hover.gif') -91px -45px;
    }

설명된 예:

- #home a:hover {background: url('img_navsprites_hover.gif') 0 -45px;} - 세 개의 모든 호버 이미지에 대해 동일한 배경 위치를 지정하고 45px만 더 아래로 지정합니다.
