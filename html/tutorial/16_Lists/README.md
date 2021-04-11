# HTML Lists
- HTML 목록을 사용하면 웹 개발자가 목록에서 관련 항목 집합을 그룹화 할 수 있다.

## Unordered HTML List
- 정렬되지 않은 목록은 `<ul>` 태그로 시작한다. 각 목록 항목은 `<li>` 태그로 시작한다.
- 목록 항목은 기본적으로 글 머리 기호 (작은 검은 색 원)로 표시됩니다.
```html
<ul>
  <li>Coffee</li>
  <li>Tea</li>
  <li>Milk</li>
</ul>
```
- **[@see](./01_Unordered_Lists/README.md)** **Unordered Lists**

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
- **[@see](./02_Ordered_Lists/README.md)** **Ordered Lists**

## HTML Description Lists
- HTML은 설명 목록도 지원한다.
- 설명 목록은 각 용어에 대한 설명이 포함 된 용어 목록이다.
- `<dl>` 태그는 설명 목록을 정의하고 `<dt>` 태그는 용어 (이름)를 정의하며 `<dd>` 태그는 각 용어를 설명한다.
```html
<dl>
  <dt>Coffee</dt>
  <dd>- black hot drink</dd>
  <dt>Milk</dt>
  <dd>- white cold drink</dd>
</dl>
```