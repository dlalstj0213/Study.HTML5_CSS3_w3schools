# HTML Quotation and Citation Elements
- 인용과 인용요소

## HTML `<blockquote>` for Quotations
- HTML `<blockquote>` 요소는 다른 소스에서 인용 된 섹션을 정의한다.
- 브라우저는 일반적으로 `<blockquote>` 요소를 들여 쓴다.
```html
<p>Here is a quote from WWF's website:</p>
<blockquote cite="http://www.worldwildlife.org/who/index.html">
For 50 years, WWF has been protecting the future of nature.
The world's leading conservation organization,
WWF works in 100 countries and is supported by
1.2 million members in the United States and
close to 5 million globally.
</blockquote>
```

## HTML `<q>` for Short Quotations
- HTML `<q>` 태그는 짧은 인용문을 정의한다.
- 브라우저는 일반적으로 인용문 주위에 인용 부호를 삽입한다.
- `<q>`는 시작 부분과 끝 부분에 큰 따옴표(`""`)로 표시된다. 
```html
<p>WWF's goal is to: 
<q>Build a future where people live in harmony with nature.</q>
</p>
```

## HTML `<abbr>` for Abbreviations
- HTML `<abbr>` 태그는 "HTML", "CSS", "Mr.", "Dr.", "ASAP", "ATM"과 같은 약어 또는 두 문자어를 정의한다.
- 표시 약어는 브라우저, 번역 시스템 및 검색 엔진에 유용한 정보를 제공 할 수 있다.
> Tip: 요소 위로 마우스를 가져갈 때 약어 / 약어에 대한 설명을 표시하려면 전체 제목 속성을 사용하자.
```html
<p>The 
<abbr title="World Health Organization">WHO</abbr> 
was founded in 1948.</p>
```

## HTML `<address>` for Contact Information
- HTML `<address>` 태그는 문서 또는 기사의 작성자 / 소유자에 대한 연락처 정보를 정의한다.
- 연락처 정보는 이메일 주소, URL, 실제 주소, 전화 번호, 소셜 미디어 핸들 등이 될 수 있다.
- `<address>` 요소의 텍스트는 일반적으로 기울임 꼴로 렌더링되며 브라우저는 항상 `<address>` 요소 앞뒤에 줄 바꿈을 추가한다.
```html
<address>
Written by John Doe.<br>
Visit us at:<br>
Example.com<br>
Box 564, Disneyland<br>
USA
</address>
```

## HTML `<cite>` for Work Title
- HTML `<cite>` 태그는 창의적인 작품 (예 : 책,시, 노래, 영화, 그림, 조각 등)의 제목을 정의한다.
- 참고 : 사람의 이름은 저작물의 제목이 아니다.
- `<cite>` 요소의 텍스트는 일반적으로 기울임 꼴로 렌더링된다.
```html
<p><cite>The Scream</cite> by Edvard Munch. Painted in 1893.</p>
```

## HTML <bdo> for Bi-Directional Override
- BDO는 Bi-Directional Override를 의미합니다.
- HTML `<bdo>` 태그는 현재 텍스트 방향을 재정의하는 데 사용됩니다.
- 브라우저가 양방향 재정(BDO)의 `<bdo>`를 지원하는 경우 다음 줄이 오른쪽에서 왼쪽 (rtl=right to left)으로 작성됩니다.
```html
<bdo dir="rtl">This text will be written from right to left</bdo>
<bdo dir="rtl">tfel ot thgir morf nettirw eb lliw txet sihT</bdo>
```