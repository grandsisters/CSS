## CSS를 추가하는 방법
브라우저가 스타일 시트를 읽을 때 스타일 시트의 정보에 따라 HTML 문서의 형식을 지정합니다.

***
### CSS를 삽입하는 세 가지 방법
스타일 시트를 삽입하는 방법에는 세 가지가 있습니다.

- 외부 CSS
- 내부 CSS
- 인라인 CSS

***
### 외부 CSS
외부 스타일 시트를 사용하면 파일 하나만 변경하여 전체 웹 사이트의 모양을 변경할 수 있습니다!

각 HTML 페이지는 헤드 섹션 내부의 \<link> 요소 내부에 외부 스타일 시트 파일에 대한 참조를 포함해야 합니다.

    예시
    외부 스타일은 HTML 페이지의 <head> 섹션 내 <link> 요소 내에서 정의됩니다.

    <!DOCTYPE html>
    <html>
    <head>
    <link rel="stylesheet" href="mystyle.css">
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>

외부 스타일 시트는 모든 텍스트 편집기에서 작성할 수 있으며 .css 확장자로 저장해야 합니다.

외부 .css 파일에는 HTML 태그가 포함되어서는 안 됩니다.

"mystyle.css" 파일의 모양은 다음과 같습니다.

    "mystyle.css"
    body {
    background-color: lightblue;
    }

    h1 {
    color: navy;
    margin-left: 20px;
    }

참고: 속성 값과 단위(예: margin-left: 20 px;) 사이에 공백을 추가하지 마십시오 . 올바른 방법은 다음과 같습니다.margin-left: 20px;

***
### 내부 CSS
하나의 HTML 페이지에 고유한 스타일이 있는 경우 내부 스타일 시트를 사용할 수 있습니다.

내부 스타일은 헤드 섹션 내부의 \<style> 요소 내부에 정의됩니다.

    예시
    내부 스타일은 HTML 페이지의 <head> 섹션 내 <style> 요소 내에서 정의됩니다.

    <!DOCTYPE html>
    <html>
    <head>
    <style>
    body {
    background-color: linen;
    }

    h1 {
    color: maroon;
    margin-left: 40px;
    }
    </style>
    </head>
    <body>

    <h1>This is a heading</h1>
    <p>This is a paragraph.</p>

    </body>
    </html>

***
### 인라인 CSS
인라인 스타일을 사용하여 단일 요소에 고유한 스타일을 적용할 수 있습니다.

인라인 스타일을 사용하려면 해당 요소에 style 속성을 추가하세요. style 속성은 모든 CSS 속성을 포함할 수 있습니다.

    예시
    인라인 스타일은 관련 요소의 "style" 속성 내에서 정의됩니다.

    <!DOCTYPE html>
    <html>
    <body>

    <h1 style="color:blue;text-align:center;">This is a heading</h1>
    <p style="color:red;">This is a paragraph.</p>

    </body>
    </html>

팁: 인라인 스타일은 스타일 시트의 많은 장점을 잃습니다(컨텐츠와 프리젠테이션을 혼합하여). 이 방법은 아껴서 사용하십시오.

***
### 여러 스타일 시트
다른 스타일 시트의 동일한 선택기(요소)에 대해 일부 속성이 정의된 경우 마지막으로 읽은 스타일 시트의 값이 사용됩니다. 

외부 스타일 시트 에 \<h1> 요소에 대해 다음과 같은 스타일이 있다고 가정합니다 .

    h1 {
    color: navy;
    }

그런 다음 내부 스타일 시트 에도 \<h1> 요소에 대해 다음과 같은 스타일이 있다고 가정합니다 .

    h1 {
    color: orange;   
    }

    예시
    내부 스타일이 외부 스타일 시트에 대한 링크 뒤에 정의 되면 <h1> 요소는 "주황색"이 됩니다.

    <head>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
    <style>
    h1 {
    color: orange;
    }
    </style>
    </head>


    예시
    그러나 외부 스타일 시트에 대한 링크 전에 내부 스타일이 정의된 경우 <h1> 요소는 "네이비"가 됩니다. 

    <head>
    <style>
    h1 {
    color: orange;
    }
    </style>
    <link rel="stylesheet" type="text/css" href="mystyle.css">
    </head>

***
### 계단식 순서
HTML 요소에 대해 지정된 스타일이 둘 이상 있을 때 어떤 스타일이 사용됩니까?

페이지의 모든 스타일은 다음 규칙에 따라 새로운 "가상" 스타일 시트로 "계단"되며, 여기서 1번이 가장 높은 우선 순위를 갖습니다.

1.인라인 스타일(HTML 요소 내부)

2.외부 및 내부 스타일 시트(헤드 섹션에 있음)

3.브라우저 기본값

따라서 인라인 스타일이 가장 높은 우선 순위를 가지며 외부 및 내부 스타일과 브라우저 기본값을 재정의합니다.