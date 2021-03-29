# HTML Elements
## HTML 요소(Elements)
- HTML 요소(Elements)는 시작 태그(start tag), 일부 콘텐츠(contents) 및 종료 태그(end tag)로 정의된다.
- ex) `<tagName>Content goes here...</tagName>`

## 중첩(Nested) HTML Elements
- HTML 요소는 중첩 될 수 있다 (즉, 요소에 다른 요소가 포함될 수 있음).
- ex)
```html
<!DOCTYPE html>
<html>
<body>
    <h1>My First Heading</h1>
    <p>My first paragraph.</p>
</body>
</html>
```
- `<html>` 요소는 루트 요소이며 전체 HTML 문서를 정의한다.
- `<body>` 요소는 문서의 본문을 정의한다.


## Never Skip the End Tag
- 종료 태그를 잊어 버린 경우에도 일부 HTML 요소는 올바르게 표시된다.
- **하지만**, 앞에서 말한 것을 의존하지 말자! 종료 태그를 잊어 버리면 예상치 못한 결과와 오류가 발생할 수 있다!

## Empty HTML Elements
- 콘텐츠가 없는 HTML 요소를 빈 요소(Empty Elements)라고 한다.
```html
<p>This is a <br> paragraph with a line break.</p>
```
- `<br>` 태그는 줄 바꿈을 정의하며 닫는 태그가없는 빈 요소이다.

## HTML is Not Case Sensitive
- HTML 태그는 대소 문자를 구분하지 않는다. `<P>`는 `<p>`와 동일 함을 의미한다.
- HTML 표준에는 소문자 태그가 필요하지 않지만, XHTML과 같은 더 엄격한 문서 유형에는 소문자를 요구한다.

### <참고>
- 그 외 사용 가는한 모든 HTML 태그의 전체 목록
  - [HTML Tag Reference (W3Schools)](https://www.w3schools.com/tags/default.asp)