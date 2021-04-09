***
## 표 스타일
***

### 표 제목의 위치를 정해 주는 caption-side속성

표 제목은 caption태그를 이용해 캡션으로 표시한다.

캡션은 기본적으로 표 위쪽에 표시되지만 caption-side속성을 이용하면 표 아래쪽으로 옮길 수 있다.

    - 기본형
    caption-side: top | bottom

|종류|설명|
|----|----|
|top|캡션을 표 윗부분에 표시한다. 기본값|
|bottom|캡션을 표 아랫부분에 표시한다.|

***

### 표에 테두리를 그려 주는 border속성

표 테두리는 border속성을 사용하는데 표 바깥 테두리와 셀 테두리를 각각 지정한다.

    - 예시

    table {
        caption-side: bottom;  // 표 캡션 위치 아래로
        border: 1px solid balck; // 표 테두리는 검은색 실선으로
    }

    td, th {
        border: 1px dtted black    // 셀 테두리는 검은색 점선으로
        padding: 10px;  // 셀 테두리와 내용 사이의 여백
        text-align: center; // 셀 내용 정렬 방법
    }

***

### 셀 사이의 여백을 지정하는 border-spacing속성

표와 셀에 따로 테두리를 지정하면 셀과 셀 사이에 여백이 조금 생긴다.

border-apcing속성을 사용하면 셀과 셀 사이의 여백을 조절할 수 있다.

    - 기본형
    border-spacing: 수평거리 수직거리

border-spacing속성값은 수평 거리의 값과 수직 거리의 값을 공백으로 구별해서 나타내는데, 두 값이 같다면 1개만 지정해도 된다.

***

### 표와 셀 테두리를 합쳐 주는 border-collapse속성

table태그와 td태그에서 border속성을 사용하면 셀과 셀 사이에 여백이 생기면서 두 줄로 표시된다. 

이때 두 줄로 그냥 둘 것인지 아니면 합쳐서 하나로 표시할 것인지 결정하는 것이 border-collapse속성이다.

이 속성은 table태그에 적용되는 스타일에만 지정하면 된다.

|종류|설명|
|----|----|
|collapse|표와 셀의 테두리를 합쳐 하나로 표시한다.|
|separate|표와 셀의 테두리를 따로 표시한다. 기본값|

***
