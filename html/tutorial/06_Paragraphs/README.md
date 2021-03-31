# Paragraphs
- 단락(Paragraph)은 항상 새 줄에서 시작하며 일반적으로 텍스트 블록이다.

## HTML Paragraphs
- HTML `<p>` 요소는 단락을 정의한다.
- 단락은 항상 새 줄에서 시작되며 브라우저는 단락 앞뒤에 공백 (여백)을 자동으로 추가한다.
```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

## HTML Display
- HTML이 어떻게 표시 될지 확신 할 수 없다.
- 크거나 작은 화면 및 크기 조정 된 창은 다른 결과를 생성한다.
- HTML을 사용하면 HTML 코드에 공백이나 줄을 추가하여 표시를 변경할 수 없다.
- 브라우저는 페이지가 표시 될 때 추가 공백과 줄을 자동으로 제거한다.
```html
<p>
This paragraph
contains a lot of lines
in the source code,
but the browser
ignores it.
</p>

<p>
This paragraph
contains         a lot of spaces
in the source         code,
but the        browser
ignores it.
</p>
```

## HTML 수평(Horizontal) 규칙(Rules)
- `<hr>` 태그는 HTML 페이지에서 주제별 구분을 정의하며 대부분 가로 규칙으로 표시된다.
- `<hr>` 요소는 HTML 페이지에서 콘텐츠를 분리 (또는 변경 정의)하는 데 사용된다.
```html
<h1>This is heading 1</h1>
<p>This is some text.</p>
<hr>
<h2>This is heading 2</h2>
<p>This is some other text.</p>
<hr>
```
- `<hr>` 태그는 빈 태그로 종료 태그가 없음을 의미한다.

## HTML 줄 바꿈(Line Breaks)
- HTML `<br>` 요소는 줄 바꿈을 정의한다.
- 새 단락을 시작하지 않고 줄 바꿈 (새 줄)을 사용하려면 `<br>`을 사용한다.
```html
<p>This is<br>a paragraph<br>with line breaks.</p>
```
- `<br>` 태그는 빈 태그로 종료 태그가 없음을 의미합니다.

## The Poem Problem
```html
<p>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</p>
```
- 이 시는 한 줄로 표시된다. ([@see: HTML Display](#html-display))

## Solution - The HTML `<pre>` Element
- HTML `<pre>` 요소는 미리 서식이 지정된 텍스트를 정의한다.
- `<pre>` 요소 내부의 텍스트는 고정 너비 글꼴 (일반적으로 Courier)로 표시되며 공백과 줄 바꿈을 모두 유지한다.
```html
<pre>
  My Bonnie lies over the ocean.

  My Bonnie lies over the sea.

  My Bonnie lies over the ocean.

  Oh, bring back my Bonnie to me.
</pre>
```