# HTML Colors
- HTML 색상은 미리 정의 된 색상 이름 또는 RGB, HEX, HSL, RGBA 또는 HSLA 값으로 지정된다.

## Color Names
- HTML에서는 색상 이름을 사용하여 색상을 지정할 수 있다.
```html
<h1 style="background-color:Tomato;">Tomato</h1>
```
### 참고
- HTML supports [140 standard color names](https://www.w3schools.com/colors/colors_names.asp).

## Background Color
```html
<h1 style="background-color:DodgerBlue;">Hello World</h1>
<p style="background-color:Tomato;">Lorem ipsum...</p>
```

## Text Color
```html
<h1 style="color:Tomato;">Hello World</h1>
<p style="color:DodgerBlue;">Lorem ipsum...</p>
<p style="color:MediumSeaGreen;">Ut wisi enim...</p>
```

## Border Color
```html
<h1 style="border:2px solid Tomato;">Hello World</h1>
<h1 style="border:2px solid DodgerBlue;">Hello World</h1>
<h1 style="border:2px solid Violet;">Hello World</h1>
```

## Color Values
- HTML에서는 RGB 값, HEX 값, HSL 값, RGBA 값 및 HSLA 값을 사용하여 색상을 지정할 수도 있다.
- RGBA 또는 HSLA 색상 값을 사용하여 투명 색상을 지정할 수도 있다.
```html
<h1 style="background-color:rgb(255, 99, 71);">rgb(255, 99, 71)</h1>
<h1 style="background-color:#ff6347;">#ff6347</h1>
<h1 style="background-color:hsl(9, 100%, 64%);">hsl(9, 100%, 64%)</h1>
<h1 style="background-color:rgba(255, 99, 71, 0.5);">rgba(255, 99, 71, 0.5)</h1>
<h1 style="background-color:hsla(9, 100%, 64%, 0.5);">hsla(9, 100%, 64%, 0.5)</h1>
```