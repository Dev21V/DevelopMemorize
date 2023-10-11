# Mark Down 개요
#markdown #overview


## 목차
[[#Mark Down 개요]]
	[[#목차]]	
	[[#1. Mark Down에 관하여]]
		[[#1.2. Mark Down의 장-단점]]
	[[#2. MarkDown 문법 (사용법)]]
		[[#2.1. Header (헤더, 제목)]]
		[[#2.2. Horizontal Rules 수평선]]
		[[#2.3. Line Breaks 줄 바꿈]]
		[[#2.4. Emphasis 강조]]
		[[#2.5. Blockquotes 인용]]	
		[[#2.6. Lists 목록]]	
			[[#2.6.1. Unorderd lists 순서가 없는 목록]]
			[[#2.6.2 Orderd lists 순서가 있는 목록]]	
				[[#2.6.2.1. 일반적인 리스트]]	
				[[#2.6.2.2. 리스트 안 리스트]]	
				[[#2.6.2.3. 혼합 리스트]]	
		[[#2.7. Backslash Escapes]]	
		[[#2.8. Links (Anchor) 링크]]	
			[[#2.8.1. 외부 링크]]	
			[[#2.8.2. 내부(해시) 링크]]	
		[[#2.9. 이미지]]
		[[#2.10. 코드 블럭]]	
		[[#2.11. 체크 리스트]]
		[[#2.12. Table 테이블]]		
	[[#3. 마무리]]		
## 1. Mark Down에 관하여
### 1.1. Mark Down 이란?
Mark Down은 Text 기반의 Mark Up Language 로 2004년 존 그루버에 의해 만들어졌으며 쉽게 쓰고 읽을 수 있으며 HTML로 변환이 가능하다.
특수기호와 문자를 이용한 매우 간단한 구조의 문법을 사용하며 웹에서도 보다 빠르게 컨텐츠를 작성하고 보다 직관적으로 인식할 수 있다.

### 1.2. Mark Down의 장-단점
#### 1.2.1. 장점
1. 간결하다
2. 별도의 도구 없이 작성 가능하다.
3. 다양한 형태로 변환이 가능하다.
4. Text로 저장되어 용량이 적어 보관에 용이하다.
5. Text File이기 때문에 VCS(Version Controll System)을 이용하여 변경 이력을 관리 가능하다.
6. 지원하는 프로그램과 플랫폼이 다양하다 ex) Github, Notion, Obsidian

#### 1.2.2. 단점
1. 표준이 없다.
2. 표준이 없어 도구에 따라 변환방식이나 생성물이 다르다.
3. 모든 HTML 마크업을 대신하지는 못한다.

## 2. MarkDown 문법 (사용법)
### 2.1. Header (헤더, 제목)

	# 으로 시작하는 텍스트
	# 은 하나부터 여섯개까지 가능
	HTML 에서의 <h1~6> 태그와 같음
	H1 은 === 으로 대체 가능
	H2 는 --- 으로 대체 가능

	This is an H1
	========
	This is an H2
	--------

This is an H1
===
This is an H2
---

> # This is an H1
> ## This is an H2
> ### This is an H3
> #### This is an H4
> ##### This is an H5
> ###### This is an H6

# This is an H1
## This is an H2
### This is an H3
#### This is an H4
##### This is an H5
###### This is an H6
^MDheader
### 2.2. Horizontal Rules 수평선
> - 또는 * 또는 _ 를 3개 이상 작성.
> 단 -을 사용할 경우 header로 인식할 수 있으니 이 전 라인은 비워두어야 함.

	***
	******
	- - -
	------------------
***

### 2.3. Line Breaks 줄 바꿈
	<br> 을 이용하여 줄바꿈 가능
	엔터로 칸을 띄면 다음행으로 넘어가게 됨. <br>은 하나의 문장에서 줄바꿈
	단, 지금 작성되고 있는 옵시디언에서는 엔터도 줄바꿈

	푸른 하늘 펼쳐진
	추억으로 덮어질 <br>
	지금 나랑 떠날래
	We fly away, All night All day <br>
	눈 앞에 펼친 Paradise
	오늘 밤의 짜릿함

푸른 하늘 펼쳐진
추억으로 덮어질 <br>
지금 나랑 떠날래
We fly away, All night All day <br>
눈 앞에 펼친 Paradise
오늘 밤의 짜릿함

### 2.4. Emphasis 강조
> 기울여 쓰기(Itatic) : * 혹은 _ 로 감싼 텍스트.
> 두껍게 쓰기(Bold): ** 또는 __ 로 감싼 텍스트.
> 취소선: ~~ 로 감싼 텍스트

	_This will be Itatic_
	**This will be bold**
	~~This will be cancled~~
	_You **can** ~~combine~~ them_

_This will be Italic_
**This will be bold**
~~This wiill be cancled~~
_You **can** ~~combine~~ them_

### 2.5. Blockquotes 인용
	> 으로 시작하는 Text
	> 는 3개까지 가능.
	Obsidian에서는 추가적으로 더 가능.

	> 늘 같은 곳을 바라보던 너의 그 눈이 좋아
	>> 변한 세상에서 너 만은 그대로 있어줘
	>>> you`re my sunshine

> 늘 같은 곳을 바라보던 너의 그 눈이 좋아
>> 변한 세상에서 너 만은 그대로 있어줘
>>> you`re my sunshine
>>>> 늘 같은 곳을 헤매이던 너와 내 시간 속에
>>>>> 날 잊어버린다 해도
>>>>>> 다시 한번 너를 만나러 갈 테니까

	인용구 안에는 제목이나 리스트, 텍스트 박스도 넣을 수 있음.
	옵시디언에서는 제목, 리스트 미지원

> # 111
> * dsadsasad
> `asdasd`


![[Pasted image 20231011151426.png]]
일반적인 MD에서의 예시
### 2.6. Lists  목록
#### 2.6.1. Unorderd lists 순서가 없는 목록
	*, +, - 를 이용하여 순서가 없는 목록을 만들 수 있다.
	들여쓰기를 하면 모양이 바뀜.
	Obisdian에서는 모양이 바뀌지 않음.

	* 머리
		* 가슴
			* 배
	+ 머리
		+ 가슴
			+ 배
				* 다리 
	- 머리
	-  코
	-  입

* 머리
	* 가슴
		* 배 
+ 머리
	+ 가슴
		+ 배
			* 다리
- 머리
- 가슴
- 배

![[Pasted image 20231011151403.png]]
일반적인 MD에서의 예시

#### 2.6.2 Orderd lists 순서가 있는 목록


	숫자를 기입하면 순서가 있는 목록이 됨.
	들여쓰기를 하면 모양이 바뀜.
	어떤 숫자인지는 중요하지 않음. 그냥 순서대로 됨.
	단 Obsidian에서는 적은 그대로 나옴.

##### 2.6.2.1. 일반적인 리스트

	1. 아이네
	2. 징버거
	6. 비챤
	3. 릴파 
	5. 고세구
	4. 주르르 

1. 아이네
2. 징버거
6. 비챤
3. 릴파
5. 고세구
4. 주르르

##### 2.6.2.2. 리스트 안 리스트

	리스트 안 리스트를 사용하려면 tab과 함께 숫자 1번부터 나열헤야 적용

	1.  리스트 1번
		1. 리스트 1-1
	2.  리스트 2번
	3. 리스트 3번
		1. 리스트 3-1
		2. 리스트 3-2

1. 리스트 1번
	1. 리스트 1-1
2. 리스트 2번
3. 리스트 3번
	1. 리스트 3-1
	2. 리스트 3-2

![[Pasted image 20231011151333.png]]

일반적인 MD에서의 리스트 예시

##### 2.6.2.3. 혼합 리스트
	1. 머리
		* 머리카락
		*  뚝배기
			+ 털
	2.다리
		-다리털
		-발가락
			1.허벅지

1. 머리
	* 머리카락
	* 뚝배기
		+ 털
2. 다리
	- 다리털
	- 발가락
		1. 허벅지

![[Pasted image 20231011151938.png]]

일반적인 MD에서의 예시


### 2.7. Backslash Escapes
	 특수문자를 표현할 때, 표시될 문자 앞에 \를 넣고 특수문자를 사용하면 됨.
	 * 특수 문자 출력 안됨
	 - 특수 문자 출력 안됨
	 \* 특수 문자 출력
	 \- 특수 문자 출력

* 특수 문자 출력 안됨
- 특수 문자 출력 안됨
\*  특수 문자 출력
\- 특수 문자 출력
\# hash mark#
\[square brackets]


### 2.8. Links (Anchor) 링크
#### 2.8.1. 외부 링크
	[Google](Http://wwww.google.com "구글")
	구글 www.google.com
	구글 <www.google.com>
	My mail <temp@gmail.com>
	
	
[Google](Http://wwww.google.com "구글")
구글 www.google.com
구글 <www.google.com>
My mail <temp@gmail.com>

#### 2.8.2. 내부(해시) 링크
	[보여지는 내용](#이동할 헤드(제목))
	괄호 안의 링크를 쓸 때는 띄어쓰기는 -로 연결, 영어는 모두 소문자로 작성

	[1.Headers 헤더](#1-headers-헤더)
	[2. Emphasis 강조](#2-emphasis-강조)
	[3. Blockquotes 인용](#3-blockquotes-인용)

[[#2.1. Header (헤더, 제목)]]
### 2.9. 이미지
	링크와 비슷하지만 앞에 !가 붙음.
	인라인 이미지 ![alt text](/test.png)
	링크 이미지 ![alt text](img_url)
	이미지 사이즈 변경위해선 html img tag <img width="OOOpx" height="OOOpx"></img>로 표현

	![텍스트](이미지 파일경로.jpg)
	![텍스트](이미지 파일 URL)

![스바루](https://w0.peakpx.com/wallpaper/791/53/HD-wallpaper-oozora-subaru-hololive-school-uniform-short-hair-curtain-smiling-anime.jpg)

옵시디언에서는 이미지를 붙여넣기만 해도 
들어가게 됨.
![[Pasted image 20231011153213.jpg]]

### 2.10. 코드 블럭
	간단한 인라인 코드는 텍스트 앞뒤로 `로 감싸면 됨.
> ``` 혹은 ~~~ 코드.
> ``` 옆에 언어 지정하면 Syntax Color 적용.



	```java
	System.out.prinln("hello world!")
	```

```java
	System.out.prinln("hello world!")
```

### 2.11. 체크 리스트
	 줄 앞에 - [x] 를 써서 완료된 리스트 표시.
	 줄 앞에 - []를 써서 미완료 된 리스트 표시.
	 체크 안에서 강조 외에 여러기능 사용 가능

	- [x] this is a complete item.
	- [ ] this is an incomplete item.

- [x] this is a coplete item.
- [ ] this is an incomplete item.

> - [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported

- [x] @mentions, #refs, [links](), **formatting**, and <del>tags</del> supported

### 2.12. Table 테이블
> 헤더와 셀을 구분할 때 3개 이상의 -(hyphen/dash) 기호가 필요.
> 헤더와 셀을 구분하면서 : (Colons) 기호로 셀(열/칸) 안에 내용 정렬 가능.
> 가장 좌측과 가장 우측에 있는 | (Vertical bar) 기호는 생략 가능

> Obsidian의 경우 편하게 플러그인 Advanced Table을 쓰도록 하자..

	테이블 생성
	헤더1|헤더2|헤더3
	---|---|---|---|
	셀1|셀2|셀3|셀4

헤더1|헤더2|헤더3|헤더4
---|---|---|---
셀1|셀2|셀3|셀4
셀5|셀6|셀7|셀8

	테이블 정렬
	헤더1|헤더2|헤더3
	:---|:---|:---
	Left|Center|Right
	1|2|3
	4|5|6
	7|8|9

헤더1|헤더2|헤더3
:---|:---|:---
Left|Center|Right
1|2|3
4|5|6
7|8|9


### 3. 마무리
MarkDown 문법에 대해서 정리해보았다.
여기에 적혀진 내용들은 거의 다 대중적인 Mark Down 문법에 대해서 작성하였으며
Obsidian에서는 약간 다르게 적용될 수 있다.
일부 Obsidian에서 다르게 적용되는 예외 사항도 적어놓았으니 참고하도록 하자.


[[#Mark Down 개요]]
	[[#목차]]	
	[[#1. Mark Down에 관하여]]
		[[#1.2. Mark Down의 장-단점]]
	[[#2. MarkDown 문법 (사용법)]]
		[[#2.1. Header (헤더, 제목)]]
		[[#2.2. Horizontal Rules 수평선]]
		[[#2.3. Line Breaks 줄 바꿈]]
		[[#2.4. Emphasis 강조]]
		[[#2.5. Blockquotes 인용]]	
		[[#2.6. Lists 목록]]	
			[[#2.6.1. Unorderd lists 순서가 없는 목록]]
			[[#2.6.2 Orderd lists 순서가 있는 목록]]	
				[[#2.6.2.1. 일반적인 리스트]]	
				[[#2.6.2.2. 리스트 안 리스트]]	
				[[#2.6.2.3. 혼합 리스트]]	
		[[#2.7. Backslash Escapes]]	
		[[#2.8. Links (Anchor) 링크]]	
			[[#2.8.1. 외부 링크]]	
			[[#2.8.2. 내부(해시) 링크]]	
		[[#2.9. 이미지]]
		[[#2.10. 코드 블럭]]	
		[[#2.11. 체크 리스트]]
		[[#2.12. Table 테이블]]		
	[[#3. 마무리]]		
