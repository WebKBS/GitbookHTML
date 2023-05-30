---
description: 자바스크립트 한국어 문자열 깨질때 대처법
---

# 문자열 깨질때

자바스크립트로 한글 메세지를 내보낼때 문자열이 깨질때가 간혹 있다.

그럴때 스크립트 태그에 charset을 지정해서 문자열 깨짐을 방지하는 방법이다.

```java
<script src="주소" charset='euc-kr'></script>
```

charset='euc-kr' 을 입력해주면 해결된다.
