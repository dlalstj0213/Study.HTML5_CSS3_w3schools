# HTML Iframes
- HTML iframe은 웹 페이지 내에 웹 페이지를 표시하는 데 사용된다.

## HTML Iframe Syntax
- HTML `<iframe>` 태그는 인라인 프레임(inline frame)을 지정한다.
- 인라인 프레임(inline frame)은 현재 HTML 문서 내에 다른 문서를 포함하는 데 사용된다.
```html
<iframe src="url" title="description">
```
> Tip: 항상 `<iframe>`에 대한 `<title>` 속성을 포함하는 것이 좋다. 왜냐하면 스크린 리더에서 iframe의 내용을 읽는 데 사용되기 때문이다.

## Iframe - Set Height and Width
- 높이 및 너비 속성을 사용하여 iframe의 크기를 지정한다.
- 높이와 너비는 기본적으로 픽셀 단위로 지정된다.
```html
<iframe src="demo_iframe.htm" height="200" width="300" title="Iframe Example"></iframe>
```
- 또는 스타일 속성을 추가하고 CSS 높이 및 너비 속성을 사용할 수 있다.
```html
<iframe src="demo_iframe.htm" style="height:200px;width:300px;" title="Iframe Example"></iframe>
```

## Iframe - Remove the Border
- 기본적으로 iframe에는 테두리가 있다.
- 테두리를 제거하려면 스타일 속성을 추가하고 CSS 테두리 속성을 사용한다.
```html
<iframe src="demo_iframe.htm" style="border:none;" title="Iframe Example"></iframe>
```
- CSS를 사용하면 iframe 테두리의 크기, 스타일 및 색상을 변경할 수도 있다.
```html
<iframe src="demo_iframe.htm" style="border:2px solid red;" title="Iframe Example"></iframe>
```

## Iframe - Target for a Link
- iframe을 링크의 대상 프레임으로 사용할 수 있다.
- 링크의 대상 속성은 iframe의 `name` 속성을 참조해야한다.
```html
<iframe src="demo_iframe.htm" name="iframe_a" title="Iframe Example"></iframe>

<p><a href="https://www.w3schools.com" target="iframe_a">W3Schools.com</a></p>
```

## See More About Iframe
**[@see](./iframe.html)** **Iframe**