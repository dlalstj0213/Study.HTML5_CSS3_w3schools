# HTML Links
- 링크는 거의 모든 웹 페이지에서 찾아 볼 수 있다. 링크를 통해 사용자는 페이지 간에 클릭 할 수 있다.

## HTML Links - Hyperlinks
- TML 링크는 하이퍼 링크(Hyperlinks)다.
- 링크를 클릭하면 다른 문서로 이동할 수 있다.
- 링크 위로 마우스를 이동하면 마우스 화살표가 작은 손 모양으로 바뀐다.
> Note: 링크는 텍스트 일 ​​필요가 없다. 링크는 이미지 또는 기타 HTML 요소가 될 수 있다!

## HTML Links - Syntax
- HTML `<a>` 태그는 하이퍼 링크를 정의한다.
```html
<a href="url">link text</a>
```
- `<a>` 요소의 가장 중요한 속성은 링크의 목적지를 나타내는 `href` 속성이다다.
- 링크 텍스트는 사용자가 볼 수 있는 부분이다.
- 링크 텍스트를 클릭하면 지정된 URL 주소로 전송된다.
```html
<a href="https://www.w3schools.com/">Visit W3Schools.com!</a>
```
- 기본적으로 링크는 모든 브라우저에서 다음과 같이 나타난다.
  - 방문하지 않은 링크는 밑줄과 파란색이다.
  - 방문한 링크는 밑줄과 자주색으로 표시된다.
  - 활성 링크는 밑줄과 빨간색으로 표시된다.
> Tip: 링크는 물론 CSS로 스타일을 지정하여 다른 모습을 얻을 수 있다!
> **@see more** [Links_Colors](./01_Link_Colors) **and** [Links_Bookmarks](./02_Link_Bookmarks)

## HTML Links - The target Attribute
- 기본적으로 링크 된 페이지는 현재 브라우저 창에 표시된다. 이를 변경하려면 링크에 대해 다른 대상을 지정해야한다.
- `target` 속성은 링크 된 문서를 열 위치를 지정한다.
- 대상 속성은 다음 값 중 하나를 가질 수 있다.
  - `_self`: 기본값. 클릭 한 것과 동일한 창 / 탭에서 문서를 연다.
  - `_blank`: 새 창 또는 탭에서 문서를 연다.
  - `_parent`: 상위 프레임에서 문서를 연다.
  - `_top`: 창의 전체 본문에서 문서를 연다.
```html
<!-- target = "_ blank"를 사용하여 새 브라우저 창 또는 탭에서 링크 된 문서를 엽니 다. -->
<a href="https://www.w3schools.com/" target="_blank">Visit W3Schools!</a>
```

## Absolute URLs vs. Relative URLs
- 로컬 링크 (동일한 웹 사이트 내의 페이지에 대한 링크)는 상대(Relative) URL ( `https://www`부분 제외)으로 지정된다.
```html
<!-- Absolute URLs -->
<p><a href="https://www.w3.org/">W3C</a></p>
<p><a href="https://www.google.com/">Google</a></p>

<!-- Relative URLs -->
<p><a href="html_images.asp">HTML Images</a></p>
<p><a href="/css/default.asp">CSS Tutorial</a></p>
```

## HTML Links - Use an Image as a Link
- 이미지를 링크로 사용하려면 `<a>` 태그 안에 `<img>` 태그를 넣는다.
```html
<a href="default.asp">
<img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

## Link to an Email Address
- 사용자의 이메일 프로그램을 여는 링크를 생성하려면 (새 이메일을 보낼 수 있도록) `href` 속성 내에서 `mailto :`를 사용한다.
```html
<a href="mailto:someone@example.com">Send email</a>
```

## Button as a Link
- HTML 버튼을 링크로 사용하려면 JavaScript 코드를 추가해야한다.
- JavaScript를 사용하면 버튼 클릭과 같은 특정 이벤트에서 발생하는 작업을 지정할 수 있다.
```html
<button onclick="document.location='default.asp'">HTML Tutorial</button>
```

## Link Titles
- `title` 속성은 요소에 대한 추가 정보를 지정한다. 정보는 마우스가 요소 위로 이동할 때 대부분의 경우 도구 설명 텍스트로 표시된다.
```html
<a href="https://www.w3schools.com/html/" title="Go to W3Schools HTML section">Visit our HTML Tutorial</a>
```

## More on Absolute URLs and Relative URLs
```html
<!-- 전체 URL을 사용하여 웹 페이지에 연결 -->
<a href="https://www.w3schools.com/html/default.asp">HTML tutorial</a>
```
```html
<!-- 현재 웹 사이트의 html 폴더에있는 페이지에 링크 -->
<a href="/html/default.asp">HTML tutorial</a>
```
```html
<!-- 현재 페이지와 같은 폴더에있는 페이지에 링크 -->
<a href="default.asp">HTML tutorial</a>
```