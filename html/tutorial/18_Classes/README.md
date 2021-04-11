# HTML class Attribute
- HTML 클래스 속성은 HTML 요소에 대한 클래스를 지정하는 데 사용된다.
- 여러 HTML 요소가 동일한 클래스를 공유 할 수 있다.

## Using The class Attribute
- 클래스 속성은 스타일 시트에서 클래스 이름을 가리키는데 자주 사용된다. 또한 특정 클래스 이름으로 요소에 액세스하고 조작하기 위해 JavaScript에서 사용할 수도 있다.
- 아래의 코드에서는 "city"값을 가진 클래스 속성이있는 세 개의 `<div>` 요소는 모두 head 섹션의 .city 스타일 정의에 따라 동일하게 스타일이 지정됨을 볼 수 있다.
```html
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
  color: white;
  border: 2px solid black;
  margin: 20px;
  padding: 20px;
}
</style>
</head>
<body>

<div class="city">
  <h2>London</h2>
  <p>London is the capital of England.</p>
</div>

<div class="city">
  <h2>Paris</h2>
  <p>Paris is the capital of France.</p>
</div>

<div class="city">
  <h2>Tokyo</h2>
  <p>Tokyo is the capital of Japan.</p>
</div>

</body>
</html>
```
> Tip: 클래스 속성은 모든 HTML 요소에서 사용할 수 있다.

> Note: 클래스 이름은 대소 문자를 구분한다!

## The Syntax For Class
- `class`에 CSS를 정의하려면 마침표 (.) 문자와 클래스 이름을 입력한다. 그런 다음 중괄호 {} 내에 CSS 속성을 정의한다.
```html
<!DOCTYPE html>
<html>
<head>
<style>
.city {
  background-color: tomato;
}
</style>
</head>
<body>

<h2 class="city">London</h2>
<p>London is the capital of England.</p>

</body>
</html>
```

## Multiple Classes
- HTML 요소는 둘 이상의 클래스에 속할 수 있다.
- 여러 클래스를 정의하려면 클래스 이름을 공백으로 구분한다. (예 : `<div class = "city main">`. 요소는 지정된 모든 클래스에 따라 스타일이 지정된다.)
- 아해의 코드에서 첫 번째 `<h2>` 요소는 도시 클래스와 기본 클래스 모두에 속하며 두 클래스 모두에서 CSS 스타일을 가져온다.
```html
<h2 class="city main">London</h2>
<h2 class="city">Paris</h2>
<h2 class="city">Tokyo</h2>
```

## Different Elements Can Share Same Class
- 다른 HTML 요소는 동일한 클래스 이름을 가리킬 수 있다.
- 아래의 코드에서 `<h2>`와 `<p>`는 모두 "city"클래스를 가리키며 동일한 스타일을 공유한다.
```html
<h2 class="city">Paris</h2>
<p class="city">Paris is the capital of France</p>
```

## Use of The class Attribute in JavaScript
- 클래스 이름은 JavaScript에서 특정 요소에 대한 특정 작업을 수행하는 데 사용할 수도 있다.
- JavaScript는 `getElementsByClassName()` 메서드를 사용하여 특정 클래스 이름을 가진 요소에 액세스 할 수 있다.
```html
<script>
function myFunction() {
  var x = document.getElementsByClassName("city");
  for (var i = 0; i < x.length; i++) {
    x[i].style.display = "none";
  }
}
</script>
```