## CSS Text Alignment

---

### 텍스트 정렬

text-align속성은 텍스트의 수평 정렬을 설정하는 데 사용됩니다.

텍스트는 왼쪽 또는 오른쪽 정렬, 중앙 정렬 또는 양쪽 정렬이 가능합니다.

다음 예제는 가운데 정렬 및 왼쪽 및 오른쪽 정렬된 텍스트를 보여줍니다(텍스트 방향이 왼쪽에서 오른쪽인 경우 왼쪽 정렬이 기본값이고 텍스트 방향이 오른쪽에서 왼쪽인 경우 오른쪽 정렬이 기본값임).

    예시
    h1 {
    text-align: center;
    }

    h2 {
    text-align: left;
    }

    h3 {
    text-align: right;
    }

텍스트 정렬 속성을 "정렬"로 설정하면 각 줄이 늘어져 모든 줄이 너비가 같고 왼쪽과 오른쪽 여백이 직선입니다(잡지 및 신문에서처럼).

    예시
    div {
    text-align: justify;
    }

---

### 텍스트 방향

direction 및 unicode-bidi특성 : 요소의 텍스트 방향을 변경하는데 사용될 수있다

    예시
    p {
    direction: rtl;
    unicode-bidi: bidi-override;
    }

---

### 수직 정렬

vertical-align속성은 요소의 수직 배향을 설정한다.

    예시
    텍스트에서 이미지의 수직 정렬 설정:

    img.a {
    vertical-align: baseline;
    }

    img.b {
    vertical-align: text-top;
    }

    img.c {
    vertical-align: text-bottom;
    }

    img.d {
    vertical-align: sub;
    }

    img.e {
    vertical-align: super;
    }
