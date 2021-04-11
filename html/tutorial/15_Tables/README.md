# HTML Tables
- HTML 테이블을 사용하면 웹 개발자가 데이터를 행과 열로 정렬 할 수 있다.

## Define an HTML Table
- `<table>` 태그는 HTML 테이블을 정의한다.
- 각 테이블 행은 `<tr>` 태그로 정의된다. 각 테이블 헤더는 `<th>` 태그로 정의된다. 각 테이블 데이터 / 셀은 `<td>` 태그로 정의된다.
```html
<table style="width:100%">
  <tr>
    <th>head1</th>
    <th>head2</th>
    <th>head3</th>
  </tr>
  <tr>
    <td>cell1_1</td>
    <td>cell1_2</td>
    <td>cell1_3</td>
  </tr>
  <tr>
    <td>cell2_1</td>
    <td>cell2_2</td>
    <td>cell2_3</td>
  </tr>
</table>
```
> Note: `<td>` 요소는 테이블의 데이터 컨테이너이다. 모든 종류의 HTML 요소를 포함 할 수 있다. 텍스트, 이미지, 목록, 기타 표 등

## HTML Table - Add a Border
- 표에 테두리를 추가하려면 CSS `border` 속성을 사용한다.
```css
table, th, td {
  border: 1px solid black;
}
```
- 테이블과 테이블 셀 모두에 테두리를 정의해야함을 잊지말자.

## HTML Table - Collapsed Borders
- 테두리가 하나의 테두리로 축소되도록하려면 CSS `border-collapse` 속성을 추가한다.
```css
table, th, td {
  border: 1px solid black;
  border-collapse: collapse;
}
```

## HTML Table - Add Cell Padding
- 셀 패딩은 셀 내용과 테두리 사이의 간격을 지정한다.
- 패딩을 지정하지 않으면 테이블 셀이 패딩없이 표시된다.
- 패딩을 설정하려면 CSS `padding` 속성을 사용한다.
```css
th, td {
  padding: 15px;
}
```

## HTML Table - Left-align Headings
- 기본적으로 표 제목은 굵게 표시되며 가운데에 표시된다.
- 표 제목을 왼쪽 정렬하려면 CSS `text-align` 속성을 사용한다.
```css
th {
  text-align: left;
}
```

## HTML Table - Add Border Spacing
- 테두리 간격은 셀 사이의 간격을 지정한다.
- 표의 테두리 간격을 설정하려면 CSS `border-spacing` 속성을 사용한다.
```css
table {
  border-spacing: 5px;
}
```
> Note: 표에 접힌 테두리가 있는 경우 테두리 간격이 적용되지 않는다.

## HTML Table - Cell that Spans Many Columns
- 셀을 두 개 이상의 열로 확장하려면 `colspan` 속성을 사용한다.
```html
<table style="width:100%">
  <tr>
    <th>Name</th>
    <th colspan="2">Telephone</th>
  </tr>
  <tr>
    <td>Bill Gates</td>
    <td>55577854</td>
    <td>55577855</td>
  </tr>
</table>
```

## HTML Table - Cell that Spans Many Rows
- 셀을 두 개 이상의 행으로 확장하려면 `rowspan` 속성을 사용한다.
```html
<table style="width:100%">
  <tr>
    <th>Name:</th>
    <td>Bill Gates</td>
  </tr>
  <tr>
    <th rowspan="2">Telephone:</th>
    <td>55577854</td>
  </tr>
  <tr>
    <td>55577855</td>
  </tr>
</table>
```

## HTML Table - Add a Caption
- 표에 캡션을 추가하려면 `<caption>` 태그를 사용한다.
```html
<table style="width:100%">
  <caption>Monthly savings</caption>
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$100</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$50</td>
  </tr>
</table>
```
> Note: `<caption>` 태그는 `<table>` 태그 바로 뒤에 삽입해야합니다.

## A Special Style for One Table
- 특정 테이블에 대한 특수 스타일을 정의하려면 테이블에 `id` 속성을 추가한다.
- **[@see](./tables.html)** **Tables**