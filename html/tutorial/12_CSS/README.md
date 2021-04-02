# HTML Styles
- CSS는 Cascading Style Sheets를 의미한다.
- CSS는 많은 작업을 절약한다. 한 번에 여러 웹 페이지의 레이아웃을 제어 할 수 있다.

## What is CSS?
- CSS (Cascading Style Sheets)는 웹 페이지의 레이아웃 형식을 지정하는 데 사용된다.
- CSS를 사용하면 색상, 글꼴, 텍스트 크기, 요소 사이의 간격, 요소 배치 및 배치 방법, 사용할 배경 이미지 또는 배경 색상, 다양한 장치 및 화면 크기에 대한 다양한 디스플레이를 제어 할 수 있다. 훨씬 더!
> Tip: *Cascading*이라는 단어는 부모 요소에 적용된 스타일이 부모 내의 모든 자식 요소에도 적용됨을 의미한다. 따라서 본문 텍스트의 색상을 "파란색"으로 설정하면 본문 내의 모든 제목, 단락 및 기타 텍스트 요소도 동일한 색상을 갖게된다 (다른 것을 지정하지 않는 한!)

## Using CSS
- CSS는 3 가지 방법으로 HTML 문서에 추가 할 수 있다.
  - 인라인(**Inline**): HTML 요소 내부의 스타일 속성 사용
  - 내부(**Internal**): `<head>` 섹션에서 `<style>` 요소 사용
  - 외부(**External**): `<link>` 요소를 사용하여 외부 CSS 파일에 연결
- CSS를 추가하는 가장 일반적인 방법은 외부 CSS 파일에 스타일을 유지하는 것다.

## Inline CSS
- 인라인 CSS는 단일 HTML 요소에 고유 한 스타일을 적용하는 데 사용된다.
- 인라인 CSS는 HTML 요소의 스타일(`style=""`) 속성을 사용한다.
```html
<h1 style="color:blue;">A Blue Heading</h1>
<p style="color:red;">A red paragraph.</p>
```

## Internal CSS
- 내부 CSS는 단일 HTML 페이지의 스타일을 정의하는 데 사용된다.
- 내부 CSS는 `<style>` 요소 내에있는 HTML 페이지의 `<head>` 섹션에 정의됩니다.
```html
<!DOCTYPE html>
<html>
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## External CSS
- 외부 스타일 시트는 많은 HTML 페이지의 스타일을 정의하는 데 사용된다.
- 외부 스타일 시트를 사용하려면 각 HTML 페이지의 `<head>` 섹션에 링크를 추가해야한다.
```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="styles.css">
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```
- 외부 스타일 시트는 모든 텍스트 편집기에서 작성할 수 있다. 파일은 HTML 코드를 포함하지 않아야하며 `.css` 확장자로 저장해야한다.
```css
/* styles.css */
body {
  background-color: powderblue;
}
h1 {
  color: blue;
}
p {
  color: red;
}
```
> Tip: 외부 스타일 시트를 사용하면 하나의 파일을 변경하여 전체 웹 사이트의 모양을 변경할 수 있다!

## CSS Colors, Fonts and Sizes
- 일반적으로 사용되는 몇 가지 CSS 속성을 살펴보자. 더 자세한 내용은 [CSS챕터](../../../css) 통해 알아보자. ([@see CSS Chapter](../../../css))
- CSS `color` 속성은 사용할 텍스트 색상을 정의한다.
- CSS `font-family` 속성은 사용할 글꼴을 정의한다.
- CSS `font-size` 속성은 사용할 텍스트 크기를 정의한다.
```html
<!DOCTYPE html>
<html>
<head>
<style>
h1 {
  color: blue;
  font-family: verdana;
  font-size: 300%;
}
p {
  color: red;
  font-family: courier;
  font-size: 160%;
}
</style>
</head>
<body>

<h1>This is a heading</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

## CSS Border
- CSS `border` 속성은 HTML 요소 주위의 테두리를 정의한다.
> Tip: 거의 모든 HTML 요소에 테두리를 정의 할 수 있다.
```css
p {
  border: 2px solid powderblue;
}
```

## CSS Padding
- CSS 패딩(`padding`) 속성은 텍스트와 테두리 사이의 패딩(공백)을 정의한다.
```css
p {
  border: 2px solid powderblue;
  padding: 30px;
}
```

## CSS Margin
- CSS 여백(`margin`) 속성은 테두리 외부의 여백(공백)을 정의한다.
```css
p {
  border: 2px solid powderblue;
  margin: 50px;
}
```

## Link to External CSS
- 외부 스타일 시트는 전체 URL 또는 현재 웹 페이지에 **상대 경로**로 참조 할 수 있다.
```html
<!-- 스타일 시트에 링크 할 전체 URL -->
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```
```html
<!-- 현재 웹 사이트의 html 폴더에있는 스타일 시트에 연결 -->
<link rel="stylesheet" href="/html/styles.css">
```
```html
<!-- 현재 페이지와 같은 폴더에있는 스타일 시트에 연결 -->
<link rel="stylesheet" href="styles.css">
```