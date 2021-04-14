# HTML Layout Elements and Techniques
- 웹 사이트는 종종 여러 열(예 : 잡지 또는 신문)에 콘텐츠를 표시한다.

## HTML Layout Elements
- HTML에는 웹 페이지의 다른 부분을 정의하는 여러 의미 요소가 있다.

![이미지](../../../imgs/img_sem_elements.gif)

- `<header>`: 문서 또는 섹션의 헤더를 정의한다.
- `<nav>`:탐색 링크 세트를 정의한다.
- `<section>`: 문서의 섹션을 정의한다.
- `<article>`: 독립적인 콘텐츠를 정의한다.
- `<aside>`: 콘텐츠 이외의 콘텐츠를 정의한다 (예 : 사이드 바).
- `<footer>`: 문서 또는 섹션의 바닥 글을 정의한다.
- `<details>`: 사용자가 요청시 열고 닫을 수있는 추가 세부 정보를 정의한다.
- `<summary>`: `<details>` 요소의 제목을 정의한다.
- [**@see**](../27_Semantics) **more in HTML Semantics**

## HTML Layout Techniques
- 다중 열 레이아웃(Multicolumn Layouts)을 만드는 방법에는 네 가지가 있다. 각 기술에는 장단점이 존재한다.
  - CSS framework
  - CSS float property
  - CSS flexbox
  - CSS grid

## CSS Frameworks
- 레이아웃을 빠르게 만들고 싶다면 W3.CSS 또는 Bootstrap과 같은 CSS 프레임워크를 사용할 수 있다.

## CSS Float Layout
- CSS `float` 속성을 사용하여 전체 웹 레이아웃을 수행하는 것이 일반적이다. Float는 배우기 쉽다. - `float` 및 `clear` 속성이 어떻게 작동하는지 기억하기만 하면 된다. 
- 단점 : 플로팅(Floating) 요소는 문서 흐름에 연결되어있어 유연성이 떨어질 수 있다. 
- CSS Float and Clear Chapter에서 더 자세히 알아보자.

## CSS Flexbox Layout
- flexbox를 사용하면 페이지 레이아웃이 다양한 화면 크기와 다양한 디스플레이 장치를 수용해야 할 때 요소가 예측 가능하게 작동한다.
- CSS Flexbox Chapter에서 flexbox에 대해 자세히 알아보자.

## CSS Grid Layout
- CSS Grid Layout Module은 행과 열이있는 그리드 기반 레이아웃 시스템을 제공하므로 부동 및 위치 지정을 사용하지 않고도 웹 페이지를 더 쉽게 디자인 할 수 있다.
- CSS Grids View에서 CSS grids에 대해 자세히 알아보자.