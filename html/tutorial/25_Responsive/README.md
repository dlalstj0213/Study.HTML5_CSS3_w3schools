# HTML Responsive Web Design
- 반응형 웹 디자인은 모든 장치에서 잘 보이는 웹 페이지를 만드는 것이다!
- 반응형 웹 디자인은 다양한 화면 크기와 뷰포트에 맞게 자동으로 조정된다.

## What is Responsive Web Design?
- 반응형 웹 디자인은 HTML 및 CSS를 사용하여 웹 사이트의 크기를 자동으로 조정, 숨기기, 축소 또는 확대하여 모든 장치 (데스크톱, 태블릿 및 휴대폰)에서보기 좋게 만드는 것이다.

## Setting The Viewport
- 반응형 웹 사이트를 만들려면 모든 웹 페이지에 다음 `<meta>` 태그를 추가해야한다.
```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```
- 그러면 페이지의 뷰포트가 설정되어 페이지의 크기와 크기 조정을 제어하는 ​​방법에 대한 브라우저 지침이 제공된다.


## Responsive Images
- 반응형 이미지는 모든 브라우저 크기에 맞게 잘 확장되는 이미지이다.

### Using the width Property
- CSS `width` 속성이 100%로 설정되면 이미지가 반응형이되고 확대 / 축소된다.
```html
<img src="img_girl.jpg" style="width:100%;">
```
- 위의 코드에서 이미지는 원래 크기보다 크게 확대 될 수 있다. 대부분의 경우의 더 나은 솔루션은 `width` 대신 `max-width` 속성을 사용하는 것이다.

### Using the max-width Property
- `max-width` 속성이 100%로 설정된 경우에 이미지가 필요한 경우 축소되지만 원래 크기보다 크게 확대되지는 않는다.
```html
<img src="img_girl.jpg" style="max-width:100%;height:auto;">
```

### Show Different Images Depending on Browser Width
- HTML `<picture>` 요소를 사용하면 브라우저 창 크기에 따라 다른 이미지를 정의 할 수 있다.
```html
<picture>
  <source srcset="img_smallflower.jpg" media="(max-width: 600px)">
  <source srcset="img_flowers.jpg" media="(max-width: 1500px)">
  <source srcset="flowers.jpg">
  <img src="img_smallflower.jpg" alt="Flowers">
</picture>
```

## Responsive Text Size
- 텍스트 크기는 "뷰포트 너비"를 의미하는 **"vw"** 단위로 설정할 수 있다.
- 이렇게하면 텍스트 크기가 브라우저 창의 크기를 따른다.
```html
<h1 style="font-size:10vw">Hello World</h1>
```
- 뷰포트는 브라우저 창 크기이다. 1vw = 뷰포트 너비의 1%. 뷰포트 너비가 50cm이면 1vw는 0.5cm입니다.

## Media Queries
- 텍스트와 이미지의 크기를 조정하는 것 외에도 반응형 웹 페이지에서 미디어 쿼리를 사용하는 것도 일반적이다.
- 미디어 쿼리를 사용하면 브라우저 크기에 따라 완전히 다른 스타일을 정의 할 수 있다.
- [**@see**](./01_media_query_1.html) **Media Query-1** : 세 개의 `<div>` 요소가 큰 화면에서는 가로로 표시되고 작은 화면에서는 세로로 쌓 이도록 브라우저 창의 크기를 조정한다.

## Responsive Web Page - Full Example
- [**@see**](./02_media_query_2.html) **Media Query-2**

## Responsive Web Design - Frameworks
- W3.CSS
- Bootstrap