---
description: 반응형 이미지 최적화 Picture태그 사용방법
---

# Picture

```html
<picture class="image">
    <source media="(min-width: 1024px)" srcset="~/images/contact/contact_back_desktop.jpg">
    <source media="(min-width: 320px)" srcset="~/images/contact/contact_back_mobile.jpg">
    <img src="~/images/contact/contact_back_desktop.jpg" alt="">
</picture>

```

반응형 웹을 만들때 HTML 태그로 반응형 이미지 최적화 하는 방법이다.\
picture태그를 사용하고 source태그에 이미지 주소를 넣어준다.

media 속성은 사용할 이미지의 css @media 태그와 같은 원하는 해상도를 적용할수 있으며\
source 태그 img 태그는 source가 적용되지 않을시 default로 사용할 이미지 주소이다. 반드시 넣어주자!
