# HTML id Attribute
- HTML `id` 속성은 HTML 요소의 고유 ID를 지정하는 데 사용된다.
- HTML 문서에서 동일한 ID를 가진 요소를 두 개 이상 가질 수 없다.(즉, id 중복 X)

## Using The id Attribute
- `id` 속성은 HTML 요소의 고유 ID를 지정한다. `id` 속성의 값은 HTML 문서 내에서 고유해야한다.
- `id` 속성은 스타일 시트에서 특정 스타일 선언을 가리키는 데 사용된다. 또한 JavaScript에서 특정 ID를 가진 요소에 액세스하고 조작하는 데 사용된다.
- `id`의 구문은 다음과 같습니다. 해시 문자 (#)를 쓰고 뒤에 id 이름을 입력한다. 그런 다음 중괄호 {} 내에 CSS 속성을 정의한다.
- 아래의 코드에는 ID 이름 "myHeader"를 가리키는 `<h1>` 요소가 있다. 이 `<h1>` 요소는 head 섹션의 #myHeader 스타일 정의에 따라 스타일이 지정된다.
```html
<!DOCTYPE html>
<html>
<head>
<style>
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}
</style>
</head>
<body>

<h1 id="myHeader">My Header</h1>

</body>
</html>
```
> Note: ID 이름은 대소 문자를 구분한다!

> Note: ID 이름은 하나 이상의 문자를 포함해야하며 공백 (공백, 탭 등)을 포함하지 않아야 한다.

## Difference Between Class and ID
- 클래스 이름은 여러 HTML 요소에서 사용할 수 있지만 ID 이름은 페이지 내 하나의 HTML 요소에서만 사용해야한다.
```html
<style>
/* Style the element with the id "myHeader" */
#myHeader {
  background-color: lightblue;
  color: black;
  padding: 40px;
  text-align: center;
}

/* Style all elements with the class name "city" */
.city {
  background-color: tomato;
  color: white;
  padding: 10px;
}
</style>

<!-- An element with a unique id -->
<h1 id="myHeader">My Cities</h1>

<!-- Multiple elements with same class -->
<h2 class="city">London</h2>
<p>London is the capital of England.</p>

<h2 class="city">Paris</h2>
<p>Paris is the capital of France.</p>

<h2 class="city">Tokyo</h2>
<p>Tokyo is the capital of Japan.</p>
```

## HTML Bookmarks with ID and Links
- HTML 북마크는 독자가 웹 페이지의 특정 부분으로 이동할 수 있도록하는 데 사용된다.
- 페이지가 매우 긴 경우 책갈피가 유용 할 수 있다.
- 책갈피를 사용하려면 먼저 책갈피를 만든 다음 링크를 추가해야한다.
- 그런 다음 링크를 클릭하면 페이지가 북마크가있는 위치로 스크롤된다.
```html
<p><a href="#C4">Jump to Chapter 4</a></p>
<p><a href="#C10">Jump to Chapter 10</a></p>
<h2 id="C4">Chapter 4</h2>
<p>This chapter explains ba bla bla</p>
<h2 id="C10">Chapter 10</h2>
<p>This chapter explains ba bla bla</p>
```
## Using The id Attribute in JavaScript
- `id` 속성은 JavaScript에서 특정 요소에 대한 일부 작업을 수행하는 데 사용할 수도 있다.
- JavaScript는 `getElementById()` 메소드를 사용하여 특정 ID를 가진 요소에 액세스 할 수 있다.
```html
<script>
function displayResult() {
  document.getElementById("myHeader").innerHTML = "Have a nice day!";
}
</script>
```