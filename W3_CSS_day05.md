## CSS Comments

CSS 주석은 브라우저에 표시되지 않지만 소스 코드를 문서화하는 데 도움이 될 수 있습니다.

***
### CSS 주석
주석은 코드를 설명하는 데 사용되며 나중에 소스 코드를 편집할 때 도움이 될 수 있습니다.

주석은 브라우저에서 무시됩니다.

CSS 주석은 \<style>요소 내부에 배치 되며 /*으로 시작 하고 끝납니다 */.

    예시
    /* This is a single-line comment */
    p {
    color: red;
    }

코드에서 원하는 위치에 주석을 추가할 수 있습니다.

    예시
    p {
    color: red;  /* Set text color to red */
    }

주석은 여러 줄에 걸쳐 있을 수도 있습니다. 

    예시
    /* This is
    a multi-line
    comment */

    p {
    color: red;
    }

***
### HTML 및 CSS 주석
HTML 자습서에서 <!--...-->구문 을 사용하여 HTML 소스에 주석을 추가할 수 있다는 것을 배웠습니다 .

다음 예에서는 HTML과 CSS 주석의 조합을 사용합니다.

    예시
    <!DOCTYPE html>
    <html>
    <head>
    <style>
    p {
    color: red; /* Set text color to red */
    }
    </style>
    </head>
    <body>

    <h2>My Heading</h2>

    <!-- These paragraphs will be red -->
    <p>Hello World!</p>
    <p>This paragraph is styled with CSS.</p>
    <p>CSS comments are not shown in the output.</p>

    </body>
    </html>