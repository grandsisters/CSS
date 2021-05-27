***
## 가상 클래스와 가상 요소

***

### 사용자 동작에 반응하는 가상 클래스

<br>

사용자가 웹 요소를 클릭하거나 마우스 포인터를 올려놓는 등 특정 동작을 할 때 스타일이 바뀌도록 만들고 싶다면 가상 클래스 선택자를 사용한다.

1) 방문하지 않은 링크에 스타일을 적용하는 ':link 가상 클래스 선택자'

    웹 문서의 링크 중에서 사용자가 아직 방뭄하지 않은 링크에 스타일을 적용한다.
    텍스트 링크는 기본적으로 파라색 글자와 밑줄로 표시된다.
    이때 링크의 밑줄을 없애거나 색상을 바꾸려면 :link 선택자 를 사용한다.

2) 방문한 링크에 스타일을 적용하는 ':visited 가상 클래스 선택자'

    웹 문서의 링크 중에서 한 번 이상 방문한 링크에 스타일을 적용한다. 
    한 번 이상 방문한 텍스트 링크는 보라색이 기본값이다.
    이때 사용자가 방문한 텍스트 링크와 색상이 달라지지 않게 하려면 :visited 선택자 를 사용해 조절한다

3) 특정 요소에 마우스 포인터를 욜려놓으면 스타일을 적용하는 ':hover 가상 클래스 선택자'

    :hover 선택자 는 웹 요소 위로 마우스 포인터를 올려놓을 때 스타일을 적용한다.
    즉, 이 가상 클래스 선택자를 응용하면 이미지 위로 마우스 포인터를 올려놓았을 때 다른 이미지로 바뀌거나,
    메인 메뉴 위로 마우스 포인터를 올려놓았을 때 서브메뉴가 나타나는 효과를 만들 수 있다.

4) 웹 요소를 활성화했을 때 스타일을 적용하는 ':active 가상 클래스 선택자'

    :active 선택자 는 웹 요소의 링크나 이미지 등을 활성화했을 때, 즉 클릭했을 때 스타일을 지정한다.
    예를 들어 어떤 웹 요소의 링크를 클릭하는 순간의 스타일을 지정할 수 있다.

5) 웹 요소에 초점이 맞추어졌을 때 스타일을 적용하는 ':focus 가상 클래스 선택자'

    :focus 선택자 는 웹 요소에 초점이 맞추어졌을 때 스타일을 적용한다.
    예를 들어 텍스트 필드 안에 마우스 포인터를 올려놓거나, 웹 문서에서 tab을 눌러 입력 커서를 이동했을 때 스타일을 지정한다.

<br>

위의 1~4의 가상 클래스 선택자는 메뉴 링크에서 자주 사용하는데, 다음과 같은 순서로 정의해야 한다.

이 순서가 바뀌면 스타일을 정의하더라도 제대로 적용되지 않는다.

    1. :link
    2. :visited
    3. :hover
    4. :active

***

### 요소 상태에 따른 가상 클래스

<br>

웹 사이트나 애플리케이션 화면에서 요소의 상태에 따라 스타일을 적용할 수 있는데, 이때 가상 클래스 선택자를 사용한다.

- 앵커 대상에 스타일을 적용하는 ':target 가상 클래스 선택자'

    문서에서 같은 사이트나 다른 사이트의 페이지로 이동할 때에는 링크를 이용하고, 같은 문서 안에서 다른 위치로 이동할 때에는 앵커를 이용한다.
    이때 :target 선택자를 사용하면 앵커로 연결된 부분, 즉 앵커의 목적지가 되는 부분의 스타일을 쉽게 적용할 수 있다.

- 요소의 사용 여부에 따라 스타일을 적용하는 ':enabled 와 :disabled 가상클래스 선택자'

    해당 요소가 사용할 수 있는 상태일 때 스타일을 지정하려면 :enabled 선택자를 사용하고, 
    반대로 사용할 수 없는 상태일 때 스타일을 지정하려면 :disabled 선택자를 사용한다.

- 선택한 항목의 스타일을 적용하는 ':checked 가상 클래스 선택자'

    폼의 라디오 박스나 체크 박스에서 선택된 항목에는 checked라는 속성이 추가된다.
    이렇게 checked 속성이 있는 요소의 스타일을 지정할 때 :checked 선택자를 사용하면 편리하다.

- 특정 요소를 제외하고 스타일을 적용하는 ':not 가상 클래스 선택자'

    :not 선택자는 이름에서도 알 수 있듯이 부정의 의미가 있다. 
    여기서 not은 '괄호 안에 있는 요소를 제외한'이라는 의미이다.