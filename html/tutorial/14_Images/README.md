# HTML Images
- 이미지는 웹 페이지의 디자인과 모양을 향상시킬 수 있다.
```html
<img src="pic_trulli.jpg" alt="Italian Trulli">
```

## HTML Images Syntax
- HTML `<img>` 태그는 웹 페이지에 이미지를 포함하는 데 사도된다.
- 이미지는 기술적으로 웹 페이지에 삽입되지 않는다. 이미지는 웹 페이지에 링크된다. `<img>` 태그는 참조 된 이미지를위한 보관 공간을 만든다.
- `<img>` 태그는 비어 있고 속성 만 포함하고 닫는 태그가 없습니다.
- `<img>` 태그에는 두 가지 필수 속성이 있습니다.
- `src`: 이미지의 경로를 지정한다.
- `alt`: 이미지의 대체 텍스트를 지정한다.
```html
<img src="url" alt="alternatetext">
```

## The `src` Attribute
- 필수 `src` 속성은 이미지에 대한 경로(URL)를 지정한다.
> Tip: 웹 페이지가 로드 될 때 그 순간 웹 서버에서 이미지를 가져와 페이지에 삽입하는 것은 브라우저이다. 따라서 이미지가 실제로 웹 페이지와 관련하여 동일한 위치에 있는지 확인해야한다. 그렇지 않으면 방문자에게 끊어진 링크 아이콘이 표시된다. 브라우저가 이미지를 찾을 수없는 경우 끊어진 링크 아이콘과 대체 텍스트가 표시된다.

## The `alt` Attribute
- 필수 `alt` 속성은 사용자가 어떤 이유로 이미지를 볼 수없는 경우 (느린 연결, `src` 속성의 오류 또는 사용자가 스크린 리더(screen reader)를 사용하는 경우) 이미지에 대한 대체 텍스트를 제공한다.
> Tip: 스크린 리더(screen reader)는 HTML 코드를 읽고 사용자가 콘텐츠를 "listen" 할 수 있게 하는 소프트웨어 프로그램이다. 스크린 리더는 시각 장애가 있거나 학습 장애가있는 사람들에게 유용하다.

## Image Size - Width and Height
- `style` 속성을 사용하여 이미지의 너비와 높이를 지정할 수 있다.
```html
<img src="img_girl.jpg" alt="Girl in a jacket" style="width:500px;height:600px;">
```
- 또는, 너비`width` 및 높이`height` 속성을 사용할 수 있다.
```html
<img src="img_girl.jpg" alt="Girl in a jacket" width="500" height="600">
```
- 너비 및 높이 속성은 항상 이미지의 너비와 높이를 **픽셀** 단위로 정의한다.
> Note: 항상 이미지의 너비와 높이를 지정하자. 너비와 높이를 지정하지 않으면 이미지가 로드되는 동안 웹 페이지가 깜박일 수 있다.

## Width and Height, or Style?
- 너비`width`, 높이`height` 및 스타일`style` 속성은 모두 HTML에서 유효하다.
- 그러나 `style` 속성을 사용하는 것이 좋다. 스타일 시트(style sheets)가 이미지 크기를 변경하는 것을 방지한다.
- `width`, `height`, `style` 비교 :
  - [**@see**](./images.html) **images.html**

## Images in Another Folder
- 하위 폴더에 이미지가있는 경우 `src` 속성에 폴더 이름을 포함해야한다.
```html
<img src="/images/html5.gif" alt="HTML5 Icon" style="width:128px;height:128px;">
```

## Images on Another Server/Website
- 일부 웹 사이트는 다른 서버의 이미지를 가리킨다.
- 다른 서버의 이미지를 가리키려면 `src` 속성에 절대(전체) URL을 지정해야한다.
```html
<img src="https://www.w3schools.com/images/w3schools_green.jpg" alt="W3Schools.com">
```
> Notes on external images: 외부 이미지는 저작권이있을 수 있다. 사용 허가를받지 못하면 저작권법에 위배 될 수 있다. 또한 외부 이미지를 제어 할 수 없으며 갑자기 제거되거나 변경 될 수 있다.

## Animated Images
- HTML은 애니메이션 GIF를 허용한다.
```html
<img src="programming.gif" alt="Computer Man" style="width:48px;height:48px;">
```

## Image as a Link
- 이미지를 링크로 사용하려면 `<a>` 태그 안에 `<img>` 태그를 넣는다.
```html
<a href="default.asp">
  <img src="smiley.gif" alt="HTML tutorial" style="width:42px;height:42px;">
</a>
```

## Image Floating
- CSS `float` 속성을 사용하여 이미지가 텍스트의 오른쪽이나 왼쪽으로 떠오르게 한다.
```html
<p><img src="smiley.gif" alt="Smiley face" style="float:right;width:42px;height:42px;">
The image will float to the right of the text.</p>

<p><img src="smiley.gif" alt="Smiley face" style="float:left;width:42px;height:42px;">
The image will float to the left of the text.</p>
```

