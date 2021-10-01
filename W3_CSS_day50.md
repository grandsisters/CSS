## CSS Table Style

---

### 테이블 패딩

테두리와 표의 내용 사이의 공간을 제어하려면 padding요소의 \<td> 및 \<th>속성을 사용하십시오 .

예시
th, td {
padding: 15px;
text-align: left;
}

---

### 수평 디바이더

수평 구분선의 경우 border-bottom속성을 \<th> 및 \<td>에 추가합니다 .

    예시
    th, td {
    border-bottom: 1px solid #ddd;
    }

---

### 호버블 테이블

:hover selector를 \<tr>에 사용하여 마우스 오버 시 테이블 행을 강조 표시합니다.

    예시
    tr:hover {background-color: yellow;}

---

### 줄무늬 테이블

얼룩말 줄무늬 테이블의 경우 :nth-child()선택기를 사용하면 모든 짝수(또는 홀수) 테이블 행에 background-color를 추가합니다.

    예시
    tr:nth-child(even) {background-color: #f2f2f2;}

---

### 테이블 색상

아래 예는 \<th> 요소의 배경색과 텍스트 색상을 지정합니다.

    예시
    th {
    background-color: #04AA6D;
    color: white;
    }
