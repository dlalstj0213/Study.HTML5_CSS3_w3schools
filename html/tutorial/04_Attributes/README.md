# HTML Attributes
## HTML 속성(Attributes)
- 모든 HTML 요소는 속성을 가질 수 있다.
- 속성은 요소에 대한 추가 정보를 제공힌디.
- 속성은 항상 시작 태그에 지정된다.
- 속성은 일반적으로 `name = "value"`와 같은 이름 / 값 쌍으로 제공된다.

## The href Attribute
- `href = ""` (Hypertext Refernce)
- `<a>` (Anchor)
- `<a>` 태그는 하이퍼 링크를 정의합니다. `href` 속성은 링크가 이동하는 페이지의 **URL**을 지정한다.
```html
<a href="https://www.w3schools.com">Visit W3Schools</a>
```

## The src Attribute
- `src = ""` (Source)
- `<img>` 태그는 HTML 페이지에 이미지를 포함하는 데 사용된다. `src` 속성은 표시 할 이미지의 **경로(Path)** 를 지정합니다.
```html
<img src="img_girl.jpg">
```
- `src` 속성에 URL을 지정하는 두 가지 방법 : 
1. **Absolute URL** (절대 URL) : 다른 웹 사이트에서 호스팅되는 외부 이미지에 대한 링크. ex) `src = "https://www.w3schools.com/images/img_girl.jpg".`
> Notes: 외부 이미지는 저작권이있을 수 있다. 그래서 사용 허가를 받지 못하면 저작권법에 위배 될 수 있다. 또한 갑자기 제거되거나 변경 될 수 있기 때문에 외부 이미지를 제어 할 수 없다.

2. **Relative URL** (상대 URL) : 웹 사이트 내에서 호스팅되는 이미지에 대한 링크. 여기서 URL은 도메인 이름을 포함하지 않는다. URL이 슬래시없이 시작되면 현재 페이지를 기준으로 한다. <br>ex) `src = "img_girl.jpg"` <br>URL이 슬래시로 시작하면 도메인을 기준으로 한다. <br>ex) `src = "/ images / img_girl.jpg"`
> Tip: 도메인을 변경해도 깨지지 않기 때문에, 거의 항상 상대 URL을 사용하는 것이 가장 좋다.

## The width and height Attributes
- `<img>` 태그에는 이미지의 너비와 높이 (픽셀 단위)를 지정하는 너비 및 높이 속성도 포함되어야힌다.
```html
<img src="img_girl.jpg" width="500" height="600">
```

## The alt Attribute
- `<img>` 태그에 필요한 `alt` 속성은 어떤 이유로 이미지를 표시 할 수 없는 경우 이미지의 대체 텍스트를 지정한다. 이러한 경우는 연결 속도가 느리거나 `src` 속성의 오류 또는 사용자가 스크린 리더를 사용하기 때문에 발생할 수 있다.
```html
<img src="img_girl.jpg" alt="Girl with a jacket">
```
## The style Attribute
- `style` 속성은 색상, 글꼴, 크기 등과 같은 요소에 스타일을 추가하는 데 사용된다.
```html
<p style="color:red;">This is a red paragraph.</p>
```

## The lang Attribute
- 웹 페이지의 언어를 선언하려면 항상 `<html>` 태그 내에 `lang` 속성을 포함해야한다. 이는 검색 엔진과 브라우저를 지원하기위한 것이다.
```html
<!DOCTYPE html>
<html lang="en">
<body>
...
</body>
</html>
```
- `lang` 속성의 언어 코드에 국가 코드를 추가 할 수도 있다. 따라서 처음 두 문자는 HTML 페이지의 언어를 정의하고 마지막 두 문자는 국가를 정의한다.
```html
<!DOCTYPE html>
<html lang="en-US">
<body>
...
</body>
</html>
```

## The title Attribute
- `title` 속성은 요소에 대한 추가 정보를 정의한다.
- 제목 속성의 값은 요소 위로 마우스를 가져 가면 도구 설명으로 표시된다.
```html
<p title="I'm a tooltip">This is a paragraph.</p>
```

## We Suggest: Always Use Lowercase Attributes
- HTML 표준에는 소문자 속성 이름이 필요하지 않다.
- 제목 속성 (및 기타 모든 속성)은 제목 또는 TITLE과 같이 대문자 또는 소문자로 작성할 수 있다.
- XHTML과 같은 더 엄격한 문서 유형에 대해 소문자 속성을 요구한다.

## We Suggest: Always Quote Attribute Values
- HTML 표준은 속성 값을 따옴표로 묶을 필요가 없다.
- XHTML과 같은 더 엄격한 문서 유형에 대해서는 따옴표를 요구한다.
```html
<!--GOOD-->
<a href="https://www.w3schools.com/html/">Visit our HTML tutorial</a>
<!--BAD-->
<a href=https://www.w3schools.com/html/>Visit our HTML tutorial</a>
```

## Single or Double Quotes?
- 속성 값 주위의 큰 따옴표는 HTML에서 가장 일반적이지만 작은 따옴표도 사용할 수 있다.
- 어떤 상황에서는 속성 값 자체에 큰 따옴표가 포함 된 경우 작은 따옴표를 사용해야한다.
```html
<p title='John "ShotGun" Nelson'>
```
- 혹은 그 반대로도:
```html
<p title="John 'ShotGun' Nelson">
```

### <참고>
- 그 외 rkr HTML 요소에 대한 모든 속성의 전체 목록
  - [HTML Attribute Reference (W3Schools)](https://www.w3schools.com/tags/ref_attributes.asp)