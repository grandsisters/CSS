## 미디어 쿼리 알아보기

미디어 쿼리는 반응형 웹 디자인에서 가장 기본적인 개념이다.

***
### 미디어 쿼리

<br>

CSS 모듈인 미디어 쿼리는 사이트에 접속하는 장치에 따라 특정한 CSS 스타일을 사용하는 방법이다.

미디어 쿼리를 사용하면 접속하는 기기의 화면 크기에 따라 레이아웃이 달라진다.

사용자가 어떤 미디어를 사용하는가에 따라 사이트의 형태가 바뀌도록 CSS를 작성하는 방법을 미디어 쿼리라고 한다.

***
### 미디어 쿼리 구문

<br>

미디어 쿼리는 @media 속성을 사용해 특정 미디어에서 어떤 CSS를 적용할 것인지 지정해 준다.

    - 기본형 @media [only | not] 미디어 유형 [and 조건] * [and 조건]

    1. only: 미디어 쿼리를 지원하지 않는 웹 브라우저에서는 미디어 쿼리를 무시하고 실행하지 않는다.
    2. not: not 다음에 지정하는 미디어 유형을 제외하낟. 예를 들어 not tv라고 지정하면 TV를 제외한 미디어 유형에만 적용한다.
    3. and: 조건을 여러 개 연결해서 추가할 수 있다.

미디어 쿼리 구문은 style 태그 사이에 사용하며 대소 문자를 구별하지 않는다.

기본적으로 미디어 유형을 지정해야 하고 필요할 경우에는 and 연산자로 조건을 적용한다.

    - 예시 
    @media screen and (min-sidth: 768px) and (max-width: 1439px) {
        ...
    }

    위의 소스는 미디어 유형이 screen이면서 최소 너비가 768px이고 최대 너비는 1439px일 경우에 적용할 CSS를 정의한 구문이다.

***
### 미디어 유형의 종류

<br>

미디어 쿼리는 미디어별로 적용할 CSS를 따로 작성하므로 @media 속성 다음에 미디어 유형을 알려 줘야 한다.

|종류|설명|
|----|----|
|all|모든 미디어 유형에서 사용할 CSS를 정의한다.|
|print|인쇄 장치에서 사용할 CSS를 정의한다.|
|screen|컴퓨터 스크린에서 사용할 CSS를 정의한다. 스마트폰의 스크린도 포한된다.|
|tv|음성과 영상이 동시에 출력되는 TV에서 사용할 CSS를 정의한다.|
|aural|음성 합성 장치(주로 화면을 읽어 소리로 출력해 주는 장치)에서 사용할 CSS를 정의한다.|
|braille|점자 표시 장치에서 사용할 CSS를 정의한다.|
|handheld|패트(pad)처럼 손에 들고 다니는 장치를 위한 CSS를 정의한다.|
|projection|프로젝터를 위한 CSS를 정의한다.|
|tty|디스플레이 기능이 제한된 장치에 맞는 CSS를 정의한다. 이런 장치에서는 픽셀(px) 단위를 사용할 수 없다.|
|embossed|점자 프린터에서 사용할 CSS를 정의한다.|


    - 예시
    @meda screen { 화면용 스타일 작성
        ...
    }
    @media print { 인쇄용 스타일 작성
        ...
    }

