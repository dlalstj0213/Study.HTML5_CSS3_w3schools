# Unordered Lists
- HTML `<ul>` 태그는 정렬되지 않은 (글 머리 기호) 목록을 정의한다.

## Unordered HTML List
- 정렬되지 않은 목록은 `<ul>` 태그로 시작한다. 각 목록 항목은 `<li>` 태그로 시작한다.
- 목록 항목은 기본적으로 글 머리 기호 (작은 검은 색 원)로 표시된다.
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

## Unordered HTML List - Choose List Item Marker
- CSS `list-style-type` 속성은 목록 항목 마커의 스타일을 정의하는 데 사용된다. 다음 값 중 하나를 가질 수 있다.

|값(Value)|설명(Description)|
|:----|:----|
|disc|목록 항목 마커를 **글 머리 기호**로 설정(**기본값**)|
|circle|목록 항목 마커를 **원**으로 설정|
|square|목록 항목 마커를 **사각형**으로 설정|
|none|목록 항목은 표시되지 않음으로 설정|
```html
<!-- Example - Disc -->
<ul style="list-style-type:disc;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<!-- Example - Circle -->
<ul style="list-style-type:circle;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<!-- Example - Square -->
<ul style="list-style-type:square;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>

<!-- Example - None -->
<ul style="list-style-type:none;">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```

## Nested HTML Lists
- 목록은 중첩 될 수 있다(목록 내부 목록).
```html
<ul>
  <li>Coffee</li>
  <li>Tea
    <ul>
      <li>Black tea</li>
      <li>Green tea</li>
    </ul>
  </li>
  <li>Milk</li>
</ul>
```
> Note: 목록 항목 (`<li>`)에는 새 목록과 이미지 및 링크와 같은 기타 HTML 요소가 포함될 수 있다.

## Horizontal List with CSS
- HTML 목록은 CSS를 사용하여 다양한 방식으로 스타일을 지정할 수 있다.
- 한 가지 인기있는 방법은 목록을 **가로**로 스타일을 지정하여 **탐색 메뉴**를 만드는 것이다.
- **[@see]()** **Horizontal List**