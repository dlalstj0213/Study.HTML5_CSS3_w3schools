# HTML Ordered Lists
- HTML `<ol>` 태그는 정렬 된 목록을 정의한다. 정렬 된 목록은 숫자 또는 알파벳일 수 있다.

## Ordered HTML List
- 정렬 된 목록은 `<ol>` 태그로 시작한다. 각 목록 항목은 `<li>` 태그로 시작한다.
- 목록 항목은 기본적으로 숫자로 표시된다.
```html
<ol>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

## Ordered HTML List - The Type Attribute
- `<ol>` 태그의 `type` 속성은 목록 항목 마커의 유형을 정의한다.

|목록항목 종류(Type)|설명(Description)|
|:-----|:----|
|`type="1"`|목록 항목은 **숫자**로 번호 설정(**기본값**)|
|`type="A"`|목록 항목은 **대문자**로 번호가 매겨집니다.|
|`type="a"`|목록 항목은 **소문자**로 번호가 매겨집니다.|
|`type="I"`|목록 항목은 **대문자 로마 숫자**로 번호가 매겨집니다.|
|`type="i"`|목록 항목은 **소문자 로마 숫자**로 번호가 매겨집니다.|

```html
<!-- Numbers: -->
<ol type="1">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<!-- Uppercase Letters: -->
<ol type="A">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<!-- Lowercase Letters: -->
<ol type="a">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<!-- Uppercase Roman Numbers: -->
<ol type="I">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<!-- Lowercase Roman Numbers: -->
<ol type="i">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

## Control List Counting
- 기본적으로 정렬 된 목록은 1부터 계산된다. 지정된 숫자부터 계산을 시작하려면 시작 속성을 사용할 수 있다.
```html
<ol start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>

<ol type="I" start="50">
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ol>
```

## Nested HTML Lists
- 목록은 중첩 될 수 있다(목록 내부 목록).
```html
<ol>
  <li>Coffee</li>
  <li>Tea
    <ol>
      <li>Black tea</li>
      <li>Green tea</li>
    </ol>
  </li>
  <li>Milk</li>
</ol>
```
> Note: 목록 항목 (`<li>`)에는 새 목록과 이미지 및 링크와 같은 기타 HTML 요소가 포함될 수 있다.