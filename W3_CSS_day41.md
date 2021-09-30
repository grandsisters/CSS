## CSS Google Fonts

---

### 구글 폰트

HTML에서 표준 글꼴을 사용하지 않으려면 Google 글꼴을 사용할 수 있습니다.

Google 글꼴은 무료로 사용할 수 있으며 1000개 이상의 글꼴 중에서 선택할 수 있습니다.

---

### Google 글꼴 사용 방법

\<head> 섹션에 특별한 스타일 시트 링크를 추가한 다음 CSS에서 글꼴을 참조하기만 하면 됩니다.

    예시1
    여기서는 Google Fonts의 "Sofia"라는 글꼴을 사용하려고 합니다.

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
    <style>
    body {
    font-family: "Sofia", sans-serif;
    }
    </style>
    </head>

    예시2
    여기서는 Google Fonts의 "Trirong"이라는 글꼴을 사용하려고 합니다.

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Trirong">
    <style>
    body {
    font-family: "Trirong", serif;
    }
    </style>
    </head>

    예시3
    여기서는 Google Fonts에서 "Audiowide"라는 글꼴을 사용하려고 합니다.

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide">
    <style>
    body {
    font-family: "Audiowide", sans-serif;
    }
    </style>
    </head>

참고: CSS에서 글꼴을 지정할 때 항상 최소한 하나의 대체 글꼴을 나열하십시오(예기치 않은 동작을 방지하기 위해). 따라서 여기에서도 목록 끝에 일반 글꼴 모음(예: serif 또는 sans-serif)을 추가해야 합니다.

---

### 여러 Google 글꼴 사용

여러 Google 글꼴을 사용하려면 다음과 같이 글꼴 이름을 파이프 문자(|)로 구분하면 됩니다.

    예시
    여러 글꼴 요청:

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Audiowide|Sofia|Trirong">
    <style>
    h1.a {font-family: "Audiowide", sans-serif;}
    h1.b {font-family: "Sofia", sans-serif;}
    h1.c {font-family: "Trirong", serif;}
    </style>
    </head>

참고: 여러 글꼴을 요청하면 웹 페이지 속도가 느려질 수 있습니다! 그러니 조심하세요.

---

### Google 글꼴 스타일 지정

물론 CSS를 사용하여 원하는 대로 Google 글꼴의 스타일을 지정할 수 있습니다!

    예시
    "Sofia" 글꼴 스타일 지정:

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia">
    <style>
    body {
    font-family: "Sofia", sans-serif;
    font-size: 30px;
    text-shadow: 3px 3px 3px #ababab;
    }
    </style>
    </head>

---

### 글꼴 효과 활성화

Google은 또한 사용할 수 있는 다양한 글꼴 효과를 활성화했습니다.

먼저 Google API에 추가한 다음 특수 효과를 사용할 요소에 특수 클래스 이름을 추가합니다. 클래스 이름은 항상 로 시작 하고 로 끝납니다 .effect=effectnamefont-effect-effectname

    예시
    "Sofia" 글꼴에 불 효과 추가:

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=fire">
    <style>
    body {
    font-family: "Sofia", sans-serif;
    font-size: 30px;
    }
    </style>
    </head>
    <body>

    <h1 class="font-effect-fire">Sofia on Fire</h1>

    </body>

여러 글꼴 효과를 요청하려면 다음과 같이 효과 이름을 파이프 문자( |)로 구분하면 됩니다.

    예시
    "Sofia" 글꼴에 여러 효과 추가:

    <head>
    <link rel="stylesheet" href="https://fonts.googleapis.com/css?family=Sofia&effect=neon|outline|emboss|shadow-multiple">
    <style>
    body {
    font-family: "Sofia", sans-serif;
    font-size: 30px;
    }
    </style>
    </head>
    <body>

    <h1 class="font-effect-neon">Neon Effect</h1>
    <h1 class="font-effect-outline">Outline Effect</h1>
    <h1 class="font-effect-emboss">Emboss Effect</h1>
    <h1 class="font-effect-shadow-multiple">Multiple Shadow Effect</h1>

    </body>
