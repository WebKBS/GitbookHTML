---
description: input x 표시 css로 커스텀하기
---

# Input cancel버튼 커스텀하기

Default

```css
input[type=search]::-webkit-search-decoration,
input[type=search]::-webkit-search-cancel-button,
input[type=search]::-webkit-search-results-button,
input[type=search]::-webkit-search-results-decoration{
    -webkit-appearance: none;
    appearance: none;
    width: 20px;
    height: 20px;
    background: no-repeat url(경로) center center;
    cursor: pointer;
}
```

appearance는 고정으로 반드시 넣어주고

width와 height, background등은 자유롭게.



위처럼 사용하다가 ios에서 테스트해보니, x표시가  미리 나타나는 버그가 발견 되었다.

```css
input[type=search]::-webkit-search-cancel-button {
    -webkit-appearance: none;
    appearance: none;
    width: 20px;
    height: 20px;
    background: url(경로) no-repeat center right / 20px auto;
}
```

```css
input[type=search]::-webkit-search-cancel-button
```

이부분 하나만 사용하니 해결.
