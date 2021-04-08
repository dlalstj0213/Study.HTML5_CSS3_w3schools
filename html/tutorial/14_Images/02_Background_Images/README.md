# HTML Background Images
- 거의 모든 HTML 요소에 대해 배경 이미지를 지정할 수 있다.

## Background Image on a HTML element
- HTML 요소에 배경 이미지를 추가하려면 HTML `style` 속성과 CSS `background-image` 속성을 사용한다.
```html
<div style="background-image: url('img_girl.jpg');">
```
- 또한 `<head>` 섹션의 `<style>` 요소에 배경 이미지를 지정할 수도 있다.
```html
<style>
div {
  background-image: url('img_girl.jpg');
}
</style>
```

## Background Image on a Page
- 전체 페이지에 배경 이미지가 포함되도록하려면 `<body>` 요소에 배경 이미지를 지정해야한다.
```html
<style>
body {
  background-image: url('img_girl.jpg');
}
</style>
```

## Background Repeat
- 배경 이미지가 요소보다 작으면 요소 끝에 도달 할 때까지 이미지가 가로 및 세로로 반복된다.
- 배경 이미지가 반복되는 것을 방지하려면 `background-repeat` 속성을 `no-repeat`로 설정해야한다.
```html
<style>
body {
  background-image: url('example_img_girl.jpg');
  background-repeat: no-repeat;
}
</style>
```

## Background Cover
- 배경 이미지가 전체 요소를 덮도록하려면 `background-size` 속성을 덮도록 설정할 수 있다.
- 또한 전체 요소가 항상 덮여 있는지 확인하려면 `background-attachment` 속성을 `fixed`로 설정한다.
- 이렇게하면 배경 이미지가 늘어나지 않고 전체 요소를 덮을 것이다. (이미지는 원래 비율을 유지함).
```html
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: cover;
}
</style>
```

## Background Stretch
- 배경 이미지를 전체 요소에 맞게 늘리려면 `background-size` 속성을 `100 % 100 %`로 설정할 수 있다.
- 브라우저 창 크기를 조정하면 이미지가 늘어나지 만 항상 전체 요소를 덮는 것을 볼 수 있다.
```html
<style>
body {
  background-image: url('img_girl.jpg');
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-size: 100% 100%;
}
</style>
```

## See More About Background Images
[**@see**](./01_background_images.html) **Background Images**

[**@see**](./02_background_repeat.html) **Background Repeat**

[**@see**](./03_background_no_repeat.html) **Background No Repeat**

[**@see**](./04_background_cover.html) **Background Cover**

[**@see**](./05_background_stretch.html) **Background Stretch**