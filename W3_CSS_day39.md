## CSS Font Style

---

### 글꼴 스타일

이 font-style속성은 주로 기울임꼴 텍스트를 지정하는 데 사용됩니다.

이 속성에는 세 가지 값이 있습니다.

- normal - 텍스트가 정상적으로 표시됩니다.
- italic - 텍스트가 기울임꼴로 표시됩니다.
- oblique - 텍스트가 "기울임"입니다(oblique는 기울임꼴과 매우 유사하지만 덜 지원됨)

  예시
  p.normal {
  font-style: normal;
  }

  p.italic {
  font-style: italic;
  }

  p.oblique {
  font-style: oblique;
  }

---

### 글꼴 두께

font-weight특성은 폰트의 중량을 지정

    예시
    p.normal {
    font-weight: normal;
    }

    p.thick {
    font-weight: bold;
    }

---

### 글꼴 변형

이 font-variant속성은 텍스트를 작은 대문자로 표시할지 여부를 지정합니다.

소문자 글꼴에서는 모든 소문자가 대문자로 변환됩니다. 그러나 변환된 대문자는 텍스트의 원래 대문자보다 작은 글꼴 크기로 나타납니다.

    예시
    p.normal {
    font-variant: normal;
    }

    p.small {
    font-variant: small-caps;
    }
