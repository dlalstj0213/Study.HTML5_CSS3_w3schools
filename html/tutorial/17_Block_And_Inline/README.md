# HTML Block and Inline Elements
- 모든 HTML 요소에는 요소 유형에 따라 기본 표시 값이 있다.
- 표시 값에는 블록(Block)과 인라인(Inline)의 두 가지가 있다.

## Block-level Elements
- 블록 수준 요소(block-level element)는 항상 새 줄에서 시작한다.
- 블록 수준 요소(block-level element)는 항상 사용 가능한 전체 너비를 차지한다 (가능한 한 왼쪽과 오른쪽으로 확장).
- 블록 수준 요소(block-level element)에는 위쪽 및 아래쪽 여백이 있지만 인라인 요소에는 없다.
- `<div>` 요소는 블록 수준 요소(block-level element)이다.
```html
<div>Hello World</div>
```
- 다음은 HTML의 block-level element이다.

|Block-level Elements|||||||||
|---|---|---|---|---|---|---|---|---|
||`<address>`|`<article>`|`<aside>`|`<blockquote>`|`<canvas>`|`<dd>`|`<div>`|`<dl>`|
||`<dt>`|`<fieldset>`|`<figcaption>`|`<figure>`|`<footer>`|`<form>`|`<h1>-<h6>`|`<header>`|
||`<hr>`|`<li>`|`<main>`|`<nav>`|`<noscript>`|`<ol>`|`<p>`|`<pre>`|
||`<section>`|`<table>`|`<tfoot>`|`<ul>`|`<video>`||

## Inline Elements
- 인라인 요소는 새 줄에서 시작하지 않는다.
- 인라인 요소는 필요한만큼만 너비를 차지한다.
- 이것은 단락 내부의 `<span>` 요소이다.
```html
<span>Hello World</span>
```
|Inline Elements|||||||||
|---|---|---|---|---|---|---|---|---|
||`<a>`|`<abbr>`|`<acronym>`|`<b>`|`<bdo>`|`<big>`|`<br>`|`<button>`|
||`<cite>`|`<code>`|`<dfn>`|`<em>`|`<i>`|`<img>`|`<input>`|`<kbd>`|
||`<label>`|`<map>`|`<object>`|`<output>`|`<q>`|`<samp>`|`<script>`|`<select>`|
||`<small>`|`<span>`|`<strong>`|`<sub>`|`<sup>`|`<textarea>`|`<time>`|`<tt>`|
||`<var>`||||||||
> Note: 인라인 요소는 블록 수준 요소를 포함 할 수 없다!

## The `<div>` Element
- `<div>` 요소는 종종 다른 HTML 요소의 컨테이너로 사용된다.
- `<div>` 요소에는 필수 속성이 없지만 스타일, 클래스 및 ID는 공통이다.
- CSS와 함께 사용하면 `<div>` 요소를 사용하여 콘텐츠 블록의 스타일을 지정할 수 있다.
```html
<div style="background-color:black;color:white;padding:20px;">
  <h2>London</h2>
  <p>London is the capital city of England. It is the most populous city in the United Kingdom, with a metropolitan area of over 13 million inhabitants.</p>
</div>
```

## The `<span>` Element
- `<span>` 요소는 텍스트의 일부 또는 문서의 일부를 마크업하는 데 사용되는 인라인 컨테이너이다.
- `<span>` 요소에는 필수 속성이 없지만 스타일, 클래스 및 ID는 공통이다.
- CSS와 함께 사용하면 `<span>` 요소를 사용하여 텍스트 부분의 스타일을 지정할 수 있다.
```html
<p>My mother has <span style="color:blue;font-weight:bold">blue</span> eyes and my father has <span style="color:darkolivegreen;font-weight:bold">dark green</span> eyes.</p>
```