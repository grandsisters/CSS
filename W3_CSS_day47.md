## CSS Tables

CSS를 사용하여 HTML 테이블의 모양을 크게 개선할 수 있습니다.

---

### 테이블 테두리

CSS에서 표 테두리를 지정하려면 border속성을 사용하십시오 .

아래 예는 \<table>, \<th> 및 \<td> 요소에 검은색 테두리를 지정합니다.

    예시
    table, th, td {
    border: 1px solid black;
    }

---

### 전체 너비 테이블

위의 표는 경우에 따라 작게 보일 수 있습니다.

전체 화면(전체 너비)에 걸쳐 있어야 하는 테이블이 필요한 경우 \<table> 요소에 width: 100%를 추가 하세요.

    예시
    table {
    width: 100%;
    }

### 이중 테두리

위의 예에서 표에는 이중 테두리가 있습니다.

이는 table 요소와 \<th> 및 \<td> 요소 모두 별도의 테두리가 있기 때문입니다.

이중 테두리를 제거하려면 아래 예를 살펴보십시오.

---

### 테이블 테두리 축소

border-collapse : 테두리 축소 속성은 테이블 테두리를 단일 테두리로 축소할지 여부를 설정합니다.

    예시
    table {
    border-collapse: collapse;
    }

테이블 주위에 테두리만 지정하려면 \<table>에 대한 테두리 속성만 지정합니다.

    예시
    table {
    border: 1px solid black;
    }
