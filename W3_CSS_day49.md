## CSS Table Alignment

---

### 수평 정렬

이 text-align속성은 \<th> 또는 \<td>에 있는 콘텐츠의 수평 정렬(예: 왼쪽, 오른쪽 또는 중앙)을 설정합니다.

기본적으로 \<th> 요소의 내용은 가운데 정렬되고 \<td> 요소의 내용은 왼쪽 정렬됩니다.

\<td> 요소의 내용도 가운데 정렬하려면 text-align: center을 사용하십시오 .

    예시
    td {
    text-align: center;
    }

내용을 왼쪽 정렬하려면 text-align: left속성을 사용하여 \<th> 요소의 정렬을 강제로 왼쪽 정렬 합니다.

    예시
    th {
    text-align: left;
    }

---

### 수직 정렬

이 vertical-align속성은 \<th> 또는 \<td>에 있는 콘텐츠의 수직 정렬(예: 위쪽, 아래쪽 또는 중간)을 설정합니다.

기본적으로 테이블 내용의 수직 정렬은 center입니다(\<th> 및 \<td> 요소 모두).

다음 예제에서는 \<td> 요소의 세로 텍스트 정렬을 맨 아래로 설정합니다.

    예시
    td {
    height: 50px;
    vertical-align: bottom;
    }
