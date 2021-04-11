# HTML JavaScript
- JavaScript는 HTML 페이지를보다 동적이고 대화식으로 만든다.

## The HTML `<script>` Tag
- HTML `<script>` 태그는 클라이언트 측 스크립트(JavaScript)를 정의하는 데 사용된다.
- `<script>` 요소는 스크립트 문을 포함하거나 `src` 속성을 통해 외부 스크립트 파일을 가리 킨다.
- JavaScript의 일반적인 용도는 이미지 조작, 양식 유효성 검사 및 콘텐츠의 동적 변경이다.
- HTML 요소를 선택하기 위해 JavaScript는 대부분 `document.getElementById()` 메서드를 사용한다.
```html
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
```

## A Taste of JavaScript
```js
// JavaScript can change content:
document.getElementById("demo").innerHTML = "Hello JavaScript!";

// JavaScript can change styles:
document.getElementById("demo").style.fontSize = "25px";
document.getElementById("demo").style.color = "red";
document.getElementById("demo").style.backgroundColor = "yellow";

// JavaScript can change attributes:
document.getElementById("image").src = "picture.gif";
```

## The HTML `<noscript>` Tag
- HTML `<noscript>` 태그는 브라우저에서 스크립트를 비활성화했거나 스크립트를 지원하지 않는 브라우저가있는 사용자에게 표시 할 대체 콘텐츠를 정의한다.
```html
<script>
document.getElementById("demo").innerHTML = "Hello JavaScript!";
</script>
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```