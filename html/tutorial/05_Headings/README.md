# HTML Headings
- HTML 제목은 웹 페이지에 표시 할 제목 또는 부제목이다.
- HTML 제목은 `<h1>` ~ `<h6>` 태그로 정의된다.
- `<h1>`은 가장 중요한 제목을 정의한다. `<h6>`은 가장 덜 중요한 제목을 정의한다.
```html
<h1>Heading 1</h1>
<h2>Heading 2</h2>
<h3>Heading 3</h3>
<h4>Heading 4</h4>
<h5>Heading 5</h5>
<h6>Heading 6</h6>
```
> Note: 브라우저는 제목 앞뒤에 공백(여백)을 자동으로 추가한다.

## Headings Are Important
- 검색 엔진은 제목을 사용하여 웹 페이지의 구조와 콘텐츠를 색인화한다.
- 사용자는 종종 제목으로 페이지를 훑어 본다. 제목을 사용하여 문서 구조를 표시하는 것이 중요하다.
- `<h1>` 머리글은 기본 머리글, `<h2>` 머리글, 덜 중요한 `<h3>` 등으로 사용되어야 한다.
> Note: 제목에만 HTML 제목을 사용하자. 제목을 사용하여 텍스트를 크게 또는 굵게 표시하지 말자.

## Bigger Headings
- 각 HTML 제목에는 기본 크기가 있다. 그러나 CSS `font-size` 속성을 사용하여 `style` 속성으로 모든 제목의 크기를 지정할 수 있다.
```html
<h1 style="font-size:60px;">Heading 1</h1>
```