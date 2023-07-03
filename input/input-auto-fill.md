---
description: 크롬 자동완성 사용시 input 백그라운드 색상변경
---

# 크롬 input auto fill

input에 자동완성할때 백그라운드 색상이 자동으로 고정값이 들어가는 값을 커스텀하는 방법이다.

```css
input:-webkit-autofill {
    -webkit-box-shadow: 0 0 0 1000px #fff inset;
}
```
