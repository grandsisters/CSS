***
## 목록 스타일

웹 사이트에서 자주 등장하는 메뉴 항목은 대부분 목록과 링크를 결합하여 만든다.

여기에 CSS를 적용하면 훨씬 멋진 사이트 메뉴가 된다.
***

### 불릿 모양과 번호 스타일을 지정하는 list-style-type속성

순서 없는 목록의 경우 목록 앞에 다양한 불릿 모양을 넣을 수 있고, 순서 목록에서는 번호 스타일을 지정할 수 있다.

이때 list-style-type속성을 사용하여 불릿의 모양이나 번호 스타일을 지정할 수 있다.

|종류|설명|
|----|----|
|disc|채운 원 모양|
|circle|빈 원 모양|
|square|채운 사각형 모양|
|decimal|1부터 시작하는 10진수|
|decimal-leading-zero|앞에 0이 붙는 10진수|
|lower-roman|로마 숫자 소문자|
|upper-roman|로마 숫자 대문자|
|lower-alpha 또는 lower-latin|알파벳 소문자|
|upper-alpha 또는 upper-latin|알파벳 대문자|
|none|불릿이나 숫자를 없앤다|

***

### 불릿 대신 이미지를 사용하는 list-style-image속성

list-style-type속성에서 바꿀 수 있는 불릿의 유형은 3가지뿐이어서 단조로운 편이다.

list-style-image속성을 이용하면 불릿을 원하는 이미지로 바꿀 수 있다.

이 경우 불릿에 들어갈 이미지는 불릿 크기만큼 작아야 좋다.

    - 기본형
    list-style-image: url(이미지 경로) | none

***

### 목록을 들여 쓰는 list-style-position속성

list-style-position속성을 사용하면 불릿이나 번호의 위치를 들여 쓸 수 있다.

속성값으로 inside를 지정하면 불릿이나 번호가 실제 내용이 시작되는 위치보다 좀 더 안으로 들여써진 듯한 효과가 난다.

이 속성은 텍스트 문단 사이에 있는 목록을 더 쉽게 구분해 준다

    - 기본형
    list-style-position: inside | outside

|종류|설명|
|----|----|
|inside|불릿이나 번호를 기본 위치보다 안으로 들여 쓴다.|
|outside|기본값이다.|

***

### 목록 속성을 한꺼번에 표시하는 list-style속성

list-style속성을 사용하면 지금까지 설명한 list-style-type, list-style-image, list-style-position속성을 한꺼번에 표시할 수 있다.

그래서 다음과 같이 소스를 간단히 줄여서 사용할 수 있다.

    불릿 없애기
    ul {list-style-type: none;}

            ->

    속성 줄여서 표시하기
    ul {list-style: none;}


    소문자 목록 만들고 들여쓰기
    ol {
        list-style-type: lower-alpha;
        list-style-position: inside;
    }

            ->

    속성 줄여서 표시하기
    ol{
        list-style: lower-alpha inside;
    }