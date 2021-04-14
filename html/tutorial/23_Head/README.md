# HTML - The Head Element
- HTML `<head>` 요소는 `<title>`, `<style>`, `<meta>`, `<link>`, `<script>` 및 `<base>` 요소에 대한 컨테이너이다.

## The HTML `<head>` Element
- `<head>` 요소는 메타 데이터(metadata, 데이터에 대한 데이터)의 컨테이너이며 `<html>` 태그와 `<body>` 태그 사이에 배치된다.
- HTML 메타 데이터(metadata)는 HTML 문서에 대한 데이터이다. 메타 데이터는 화면상 시각적으로 표시되지 않는다.
- 메타 데이터는 일반적으로 문서 제목(title), 문자 집합(character set), 스타일(style), 스크립트(script) 및 기타 메타 정보를 정의한다.

## The HTML `<title>` Element
- `<title>` 요소는 문서의 제목을 정의한다. `<title>`은 텍스트 전용이어야하며 브라우저의 제목 표시 줄이나 페이지의 탭에 표시된다.
- HTML 문서에는 `<title>` 요소가 필요하다!
- 페이지 제목의 내용은 검색 엔진 최적화(Search Engine Optimization, SEO)에 매우 중요하다! 페이지 제목은 검색 엔진 알고리즘에서 검색 결과에 페이지를 나열 할 때 순서를 결정하는 데 사용된다.
- `<title>` 요소 :
  - 브라우저 도구 모음에서 제목을 정의한다.
  - 페이지가 즐겨 찾기에 추가 될 때 페이지 제목을 제공한다.
  - 검색 엔진 결과(search engine-results)에 페이지 제목을 표시한다.
- 따라서 제목을 최대한 정확하고 의미있게 만들어야 한다!
```html
<!DOCTYPE html>
<html>
<head>
  <title>A Meaningful Page Title</title>
</head>
<body>

The content of the document......

</body>
</html>
```

## The HTML `<style>` Element
- `<style>` 요소는 단일 HTML 페이지에 대한 스타일 정보를 정의하는 데 사용된다.
```html
<style>
  body {background-color: powderblue;}
  h1 {color: red;}
  p {color: blue;}
</style>
```

## The HTML `<link>` Element
- `<link>` 요소는 현재 문서와 외부 리소스 간의 관계를 정의한다.
- `<link>` 태그는 외부 스타일 시트에 연결하는 데 가장 자주 사용된다.
```html
<link rel="stylesheet" href="mystyle.css">
```

## The HTML `<meta>` Element
- `<meta>` 요소는 일반적으로 문자 집합(character set), 페이지 설명(page description), 키워드(keywords), 문서 작성자(author of the document) 및 뷰포트 설정(viewport settings)을 지정하는 데 사용된다.
- 메타 데이터는 페이지에 표시되지 않지만 브라우저 (콘텐츠 표시 또는 페이지 다시로드 방법), 검색 엔진 (키워드) 및 기타 웹 서비스에서 사용된다.
```html
<!-- Define the character set used: -->
<meta charset="UTF-8">

<!-- Define keywords for search engines: -->
<meta name="keywords" content="HTML, CSS, JavaScript">

<!-- Define a description of your web page: -->
<meta name="description" content="Free Web tutorials">

<!-- Define the author of a page: -->
<meta name="author" content="John Doe">

<!-- Refresh document every 30 seconds: -->
<meta http-equiv="refresh" content="30">

<!-- Setting the viewport to make your website look good on all devices: -->
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

## Setting The Viewport
- 뷰포트는 웹 페이지에서 사용자가 볼 수있는 영역이다. 장치에 따라 다르며 컴퓨터 화면보다 휴대폰에서 더 작다.
- 모든 웹 페이지에 다음 `<meta>` 요소를 포함해야한다.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- 뷰포트는 페이지의 크기와 크기 조정을 제어하는 ​​방법에 대한 브라우저 지침을 제공한다.
- `width = device-width` 부분은 장치의 화면 너비를 따르도록 페이지 너비를 설정한다(장치에 따라 다름).
- `initial-scale = 1.0` 부분은 브라우저에서 페이지를 처음로드 할 때 초기 확대 / 축소 수준을 설정한다.

## The HTML `<script>` Element
- `<script>` 요소는 클라이언트 측 JavaScript를 정의하는 데 사용된다.
```html
<script>
function myFunction() {
  document.getElementById("demo").innerHTML = "Hello JavaScript!";
}
</script>
```

## The HTML `<base>` Element
- `<base>` 요소는 페이지의 모든 상대 URL에 대한 기본 URL 및 / 또는 대상을 지정한다.
- `<base>` 태그에는 `href` 또는 대상 속성이 있거나 둘 다 있어야한다.
- 문서에는 하나의 `<base>` 요소만 있을 수 있다!
```html
<head>
<base href="https://www.w3schools.com/" target="_blank">
</head>

<body>
<img src="images/stickman.gif" width="24" height="39" alt="Stickman">
<a href="tags/tag_base.asp">HTML base Tag</a>
</body>
```
- 링크는 `target = "_ blank"` 속성이 없는 경우에도 새 창에서 열린다. 이는 기본 요소의 대상 속성이 `"_blank"`로 설정되어 있기 때문이다.