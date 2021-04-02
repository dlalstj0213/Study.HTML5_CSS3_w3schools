# HTML Links - Different Colors
- HTML 링크는 방문했는지, 방문하지 않았는지, 활성 상태인지에 따라 다른 색상으로 표시된다.

## HTML Link Colors
- 기본적으로 링크는 다음과 같이 표시된다 (모든 브라우저에서).
  - 방문하지 않은 링크는 밑줄과 파란색이다.
  - 방문한 링크는 밑줄과 자주색으로 표시된다.
  - 활성 링크는 밑줄과 빨간색으로 표시된다.
- CSS를 사용하여 링크 상태 색상을 변경할 수 있다.
```html
<style>
/* 방문하지 않은 링크는 밑줄이 없는 녹색으로 표시 */
a:link {
  color: green;
  background-color: transparent;
  text-decoration: none;
}

/* 방문한 링크는 밑줄이없는 분홍색으로 표시 */
a:visited {
  color: pink;
  background-color: transparent;
  text-decoration: none;
}

/* 링크 `a : hover` 위로 마우스를 가져 가면 빨간색과 밑줄을 표시 */
a:hover {
  color: red;
  background-color: transparent;
  text-decoration: underline;
}

/* 활성 링크는 노란색으로 밑줄이 긋기 */
a:active {
  color: yellow;
  background-color: transparent;
  text-decoration: underline;
}
</style>
```

## Link Buttons
- CSS를 사용하여 링크 스타일을 버튼으로 지정할 수도 있다.
```html
<style>
a:link, a:visited {
  background-color: #f44336;
  color: white;
  padding: 15px 25px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
}

a:hover, a:active {
  background-color: red;
}
</style>
```