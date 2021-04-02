# HTML Links - Create Bookmarks
- HTML 링크를 사용하여 책갈피를 만들 수 있으므로 사용자가 웹 페이지의 특정 부분으로 이동할 수 있다.

## Create a Bookmark in HTML
- 웹 페이지가 매우 긴 경우 책갈피가 유용 할 수 있다.
- 책갈피를 만들려면 먼저 책갈피를 만든 다음 링크를 추가한다.
- 링크를 클릭하면 페이지가 북마크가있는 위치까지 아래 또는 위로 스크롤된다.
1. 먼저 `id` 속성을 사용하여 북마크를 만든다.
```html
<h2 id="C4">Chapter 4</h2>
```
2. 그런 다음 동일한 페이지 내에서 책갈피에 대한 링크 ( "Jump to Chapter 4")를 추가한다.
```html
<a href="#C4">Jump to Chapter 4</a>
```
- 다른 페이지의 책갈피에 대한 링크를 추가 할 수도 있다.
```html
<a href="html_demo.html#C4">Jump to Chapter 4</a>
```