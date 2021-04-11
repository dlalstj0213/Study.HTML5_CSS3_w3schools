# HTML File Paths
- 파일 경로는 웹 사이트의 폴더 구조에서 파일의 위치를 ​​설명한다.

## File Path Examples
|경로(Path)|설명(Description)|
|:---|:---|
|`<img src="picture.jpg">`|"picture.jpg"파일은 현재 페이지와 같은 폴더에 있다.|
|`<img src="images/picture.jpg">`|"picture.jpg"파일은 현재 폴더의 이미지 폴더에 있다.|
|`<img src="/images/picture.jpg">	`|"picture.jpg"파일은 현재 웹의 루트에있는 이미지 폴더에 있다.|
|`<img src="../picture.jpg">`|"picture.jpg"파일은 현재 폴더에서 한 수준 위의 폴더에 있다.|

## HTML File Paths
- 파일 경로는 웹 사이트의 폴더 구조에서 파일의 위치를 ​​설명한다.
- 파일 경로는 다음과 같이 외부 파일에 연결할 때 사용된다.
  - Web pages
  - Images
  - Style sheets
  - JavaScripts

## Absolute File Paths
- 절대 파일 경로는 파일의 전체 URL이다.
```html
<img src="https://www.w3schools.com/images/picture.jpg" alt="Mountain">
```
- **[@see](../14_Images)** **Images**

## Relative File Paths
- 상대 파일 경로는 현재 페이지에 상대적인 파일을 가리킨다.
- 아래의 코드에서 파일 경로는 현재 웹의 루트에있는 이미지 폴더의 파일을 가리킨다.
```html
<img src="/images/picture.jpg" alt="Mountain">
```
- 아래의 코드에서 파일 경로는 현재 폴더에있는 이미지 폴더의 파일을 가리킨다.
```html
<img src="images/picture.jpg" alt="Mountain">
```
- 아래의 코드에서 파일 경로는 현재 폴더에서 한 수준 위의 폴더에 있는 이미지 폴더의 파일을 가리킨다.
```html
<img src="../images/picture.jpg" alt="Mountain">
```

## Best Practice
- 가능한 경우 상대 파일 경로를 사용하는 것이 가장 좋다.
- 상대 파일 경로를 사용할 때 웹 페이지는 현재 기본 URL에 바인딩되지 않는다. 모든 링크는 자신의 컴퓨터 (localhost)와 현재 공용 도메인 및 향후 공용 도메인에서 작동한다.