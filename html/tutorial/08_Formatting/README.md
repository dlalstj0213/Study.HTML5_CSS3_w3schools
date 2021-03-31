# HTML Text Formatting
- HTML에는 특별한 의미를 가진 텍스트를 정의하기위한 여러 요소가 포함되어 있다.

## HTML 서식 요소(Formatting Elements)
- 서식 요소는 특수한 유형의 텍스트를 표시하도록 설계되어있다 :
  - `<b>` : 굵은 텍스트
  - `<strong>` : 중요한 텍스트
  - `<i>` : 기울임 꼴 텍스트
  - `<em>` : 강조된 텍스트
  - `<mark>` : 표시된 텍스트
  - `<small>` : 더 작은 텍스트
  - `<del>` : 삭제 된 텍스트
  - `<ins>` : 삽입 된 텍스트
  - `<sub>` : 아래 첨자 텍스트
  - `<sup>` : 위첨자 텍스트

## HTML `<b>` and `<strong>` Elements
- HTML `<b>` 요소는 특별한 중요성없이 굵은 텍스트를 정의한다.
```html
<p><b>This text is bold.</b></p>
```
- HTML `<strong>` 요소는 매우 중요한 텍스트를 정의한다. 내부 내용은 일반적으로 굵게 표시된다.
```html
<p><strong>This text is important!</strong></p>
```

## HTML `<i>` and `<em>` Elements
- HTML `<i>` 요소는 대체 음성 또는 분위기로 텍스트의 일부를 정의한다. 내부 콘텐츠는 일반적으로 기울임 꼴로 표시된다.
> Tip: `<i>` 태그는 기술 용어, 다른 언어의 문구, 생각, 선박 이름 등을 나타내는 데 자주 사용된다.
```html
<p><i>This text is italic.</i></p>
```
- HTML `<em>` 요소는 강조된 텍스트를 정의한다. 내부 콘텐츠는 일반적으로 기울임 꼴로 표시된다.
> Tip: 스크린 리더(screen reader)는 구두 스트레스(verbal stress)를 사용하여 `<em>`의 단어를 강조하여 발음한다.
```html
<p><em>This text is emphasized.</em></p>
```

## HTML `<small>` Element
- HTML `<small>` 요소는 더 작은 텍스트를 정의한다.
```html
<p>THIS IS <small>SOME SMALLER</small> TEXT.</p>
```

## HTML `<mark>` Element
- HTML `<mark>` 요소는 표시하거나 강조 표시해야하는 텍스트를 정의한다.
```html
<p>Do not forget to buy <mark>milk</mark> today.</p>
```

## HTML `<del>` Element
- HTML `<del>` 요소는 문서에서 삭제 된 텍스트를 정의한다. 브라우저는 일반적으로 삭제 된 텍스트에 한 줄을 표시한다.
```html
<p>My favorite color is <del>blue</del> red.</p>
```

## HTML `<ins>` Element
- HTML `<ins>` 요소는 문서에 삽입 된 텍스트를 정의한다. 브라우저는 일반적으로 삽입 된 텍스트에 밑줄을 긋는다.
```html
<p>My favorite color is <del>blue</del> <ins>red</ins>.</p>
```

## HTML `<sub>` Element
- HTML `<sub>` 요소는 아래 첨자 텍스트를 정의한다. 아래 첨자 텍스트는 일반 줄 아래에 절반 문자로 나타나며 때로는 더 작은 글꼴로 렌더링된다. 아래 첨자 텍스트는 H2O와 같은 화학식에 사용할 수 있다.
```html
<p>This is <sub>subscripted</sub> text.</p>
<p>H<sub>2</sub>O</p>
```

## HTML `<sup>` Element
- HTML `<sup>` 요소는 위첨자 텍스트를 정의한다. 위 첨자 텍스트는 일반 줄 위에 반 문자로 나타나며 때로는 더 작은 글꼴로 렌더링된다. WWW [1]과 같이 각주에 위 첨자 텍스트를 사용할 수 있다.
```html
<p>This is <sup>superscripted</sup> text.</p>
<p>WWW<sup>[1]</sup></p>
```