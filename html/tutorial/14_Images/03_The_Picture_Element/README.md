# HTML `<picture>` Element
- HTML `<picture>` 요소를 사용하면 장치 또는 화면 크기에 따라 다른 그림을 표시 할 수 있다.

## The HTML `<picture>` Element
- HTML `<picture>` 요소는 웹 개발자에게 이미지 리소스를 지정하는 데 더 많은 유연성을 제공한다.
- `<picture>` 요소는 각각 `srcset` 속성을 통해 서로 다른 이미지를 참조하는 하나 이상의 `<source>` 요소를 포함한다. 이렇게하면 브라우저가 현재보이는 모습 또는 장치에 가장 잘 맞는 이미지를 선택할 수 있다.
- 각 `<source>` 요소에는 이미지가 가장 적합한시기를 정의하는 미디어 속성이 있다.
```html
<picture>
  <source media="(min-width: 650px)" srcset="img_food.jpg">
  <source media="(min-width: 465px)" srcset="img_car.jpg">
  <img src="img_girl.jpg">
</picture>
```
> Note: 항상 `<img>` 요소를 `<picture>` 요소의 마지막 자식 요소로 지정해야한다. `<img>` 요소는 `<picture>` 요소를 지원하지 않거나 일치하는 `<source>` 태그가 없는 경우에 브라우저에서 사용된다.

## When to use the Picture Element
- `<picture>` 요소에는 **두 가지** 주요 용도가 있습니다
1. **대역폭 (Bandwidth)**
   1. 화면이나 장치가 작은 경우 큰 이미지 파일을 로드 할 필요가 없다. 브라우저는 속성 값이 일치하는 첫 번째 `<source>` 요소를 사용하고 다음 요소를 무시한다.

2. **형식/포맷 지원 (Format Support)**
   1. 일부 브라우저 또는 장치는 모든 이미지 형식을 지원하지 않을 수 있다. `<picture>` 요소를 사용하면 모든 형식의 이미지를 추가 할 수 있으며 브라우저는 인식하는 첫 번째 형식을 사용하고 다음 요소는 무시한다.
