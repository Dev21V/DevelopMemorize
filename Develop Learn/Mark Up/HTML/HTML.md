# 1.HTML 개요
#HTML #HTML5 #markup
## 1.1. HTML이란
HTML이란 HyperText Mark-up Language의 줄임말로 웹 사이트의 모습을 기술하기 위한 마크업 언어이다.   
팀 버너스리가 최초로 제안했다.   
웹 개발에 있어서 기초가 되는 마크업 언어로,  문서의 내용 이외의 문서의 구조나 서식 같은것을 포함한다.   
프로그래밍 언어가 아니다!   

# 2. 목차

# 3. HTML5

## 3.1. HTML5의 기본요소
HTML 문서는 기본적으로 Elements의 모임이다.   
Element는 아래의 형식으로 명세한다<br>
<TagName 속성1="Value" … 속성n="Value">Content</TagName>

요소 | 의미 | 코드예 
:--- | :--- | :--- 
태그(tag) |'<'와'>'로 둘러싸인 문자열<br>시작태그 <>와 종료태그</>로 구성 | `<title>Content</title>` <br> `<title> , </title> 부분`
내용(content) | 태그로 둘러싸인 문자열 |  `<title>`Content`</title>` <br> `Content 부분`
엘리먼트(element) | 태그와 내용을 포함한 전체 문자열 <br> HTML문서의 기본 구성 단위 <br> 상위 엘리먼트 안에 하위 엘리먼트가 계층적으로 포함될 수 있음 | *`<title>content<title>`*<br> `문자열 전체`
속성(attribute) | 엘리먼트의 상세한 표현(기능)설정 사항을 지시 <br> 시작 태그 안에 사용 | `<title color="red"></title` <br> `color 부분`
속성값(value) | 속성값 (' ' 또는 " " 로 감싸야함) | `<title color="red"></title` <br> `red 부분`

``` HTML
<!DOCTYPE html> <!-- 문서의 버전에 관한 정보를 나타낸다. 본 문서가 HTML5 라는 것을 명시함. -->
<html lang="en"> <!-- html 파일임을 정의. html 태그는 head 태그와 body 태그로 이루어짐. -->
<head><!-- 메타 데이터의 집합으로 웹 페이지에 직접적으로 보이지 않는 정보임. head 태그는 title, meta, link, style, script 태그로 구성됨. -->
  <meta charset="UTF-8"> <!-- meta 태그는 <meta 속성="속성값" />으로 스스토 닫는 태그이기 때문에 이렇게 나타낸다. 보기에 charset="utf-8"는 글자 깨짐에 대해 다른 언어에서도 볼수 있도록 표기한 것이다. -->
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Document</title> <!-- title 태그는 페이지를 대표하는 내용의 제목을 넣어야 함. -->
</head>
<body><!-- 본문의 내용을 담는 공간이다. -->

</body>
</html>
```

## 3.2. 기본 적인 태그
- `<!Doctype>` 문서의 버전에 관한 정보를 나타낸다.<br> HTML5의 경우 `<!Doctype html>`로 작성하면 됨.
- `<html>`: HTML이 적용되는 범위를 지정하는 태그로 위의 태그를 제외하고 감싸주면 된다.
- `<head>`:HTML 문서의 속성 범위를 지정하는 태그로 title이나 meta data를 넣는 곳이다.
- `<body>`:HTML 문서의 본문 범위를 지정하는 태그이다. 
- `<title>`:HTML의 제목을 선언하는 태그
- `<meta>`:HTML의 부가정보를 선언하는 태그.
- `<link>`:외부 CSS파일, Favicon등을 연결하는 태그.


## 3.3. `<head>`태그 정리
head는 title, CSS의 링크,Favicon, 이외  다른 meta data(설명,작성자,중요한 키워드 등 )를 포함한다. 그 외 script파일을 불러오거나 웹 폰트등을 불러오는 link등이 head 사이에 삽입된다.   
### 3.3.1. `<meta>`
html 문서에 대한 정보를 담고 있는 태그이다.   
문자 인코딩, 문서 키워드, 요약 등
> ex)
> `<meta charset="utf-8">`
> : 웹 페이지의 문자 인코딩 방식을 utf-8로 지정해라.

### 3.3.2. `<title>`
문서 제목   
`<title>` 안의 내용이 웹 브라우저의 제목 표시줄에 표시된다.   
> ex)
> `<title>웹 페이지 제목</title>`
> : `웹 페이지 제목` 이 제목 표시줄에 표시됨.

### 3.3.3. `<link>`
외부 파일을 연결할 때 사용된다.   
```HTML
<link rel="shortcut icon" type="image/x-icon" href="./favicon.ico" />
```
link 요소의 속성들을 살펴보면, 'href'는 해당 css파일의 주소를 적게 된다. 'type'과 'rel'에는 각각의 맞게 적어주게 되며, link 요소의 쓰임새가 css파일 연결 외에도 다른 외부요소를 연결하는 데에도 쓰이기 때문에 type 과 rel을 적어준다.   

==참고로 'rel'속성은 'relationship (관계)'의 줄임 말.==

> ex)
> `<link href="/style.css" rel="stylesheet" type="text/css" />`
> rel="stylesheet" 는 연결할 파일이 stylesheet 라는 의미   
> type="text/css" 는 스타일시트 코드가 텍스트 파일로 된 css 유형이라는 의미

### 3.3.4.`<style>`
스타일 정보를 정의할 때 사용하는 태그

```HTML
<!DOCTYPE html> 
<html> 
<head> 
	<style> .myDiv { border: 5px outset red; background-color: lightblue; text-align: center; } 
	</style> 
</head> 
<body> 
	<div class="myDiv"> 
		<h2>This is a heading in a div element</h2> 
		<p>This is some text in a div element.</p> 
	</div> 
	<p>This is some text outside the div element.</p> 
</body> 
</html>
```

![sdd](https://blog.kakaocdn.net/dn/ocbSS/btrZzLbxckw/wLliNh3PsZtuCCc9iMknOK/img.png)
![[Pasted image 20231012142806.png]]

### 3.3.5. `<script>`
```HTML
<script type="text/javascript" src="http://code.jquery.com/jquery-latest.min.js"></script>
```

```HTML
<script> 
	document.write("Hello World !"); </script>
```

`<script>` 태그는 두가지 방향으로 사용할 수 있는데, 위와 같이 src 속성을 넣어 외부에 있는 js를 불러와 사용할 수 있으며 혹은 src 속성을 사용하지 않고, `<script>` 태그 사이에 javasrcipt 코드를 넣어 사용하실 수 도 있다.

## 3.4. 글자/폰트 관련 태그
