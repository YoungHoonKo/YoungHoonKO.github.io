---
title: How 2 use Typora
author: YoungHoon Ko
date: 2022-07-10 10:31:00 +0900
categories: [Markdown, Md-Basics]
tags: [markdown]
image: /assets/img/screenshot/강아지.JPEG
---

# 마크다운 문법

[toc]

**소스 코드는 cmd(ctrl)+ /로 확인할 수 있습니다.**

## 목차 설정방법

~~~markdown
[toc]을 사용하면 위에 보이는 목차 처럼 목차가 생성 됩니다. 새로운 항목을 추가할 때 마다 목차가 갱신되어 실시간으로 확인할 수 있습니다.
~~~

## 블럭 요소

### 헤더

헤더는 1-6가지의 크기가 있다. 사용은 #, ##, ### --- 이렇게 사용한다.

~~~markdown
# This is an H1
## Tis is an H2
### This is an H3
~~~

사용할 때 # 뒤에 한 칸 띄우고 원하는 내용을 입력하면 된다.

### 인용

'>'를 사용해서 인용문을 작성할 수 있다.'>'의 갯수에 따라 모양이 달라진다.

~~~markdown
> 안녕하세요
> 저는 고영훈입니다.
> 만나서 반갑습니다.
>> 저는 홍길동의 친구입니다.
~~~

> 이 문장은 '>'을 사용한 인용 예문입니다.
>
> > 이 문장은 '>>'을 사용한 인용 예문입니다.



### 리스트

#### un-ordered list

'*', '+', '-' 를 사용해서 리스트를 만들 수 있다. 숫자와 같이 정렬되지 않았기 때문에 불규칙 리스트라 부름

~~~markdown
* 1
	* 이렇게 리스트 밑에 또 다른 리스트를 만들 수 있습니다.제한 없이 만들 수 있습니다.
+ 2
	+ 숫자 이
		+ two
- 3

~~~

* 이것은 예문
  * 이것은 예문
    * 이것은 예문
      * 이것은 예문

#### ordered list

1, 2, 3, 4 -- 등의 숫자를 사용해서 정렬된 리스트를 만듭니다.

~~~ markdown
1. 예문1
2. 예문2
3. 예문3
~~~

1. 예문1
2. 예문2
3. 예문3

### 체크리스트

'- [ ]' 이 문법을 사용하면 가능합니다. '-'와 '[ ]' 사이에 한 칸 띄우는 것이 매우 중요합니다.그리고 '[ ]' 이 대괄호 안에도 한 칸 띄워 주셔야합니다.

- [ ] 체크리스트 예시1
- [ ] 체크리스트 예시2

### 코드블럭

'~~~'을 친 후에 원하는 언어 이름을 입력하면 그 언어 문법을 사용할 수 있습니다. 물론 실행은 되지 않지만  원하는 언어의 문법에 맞춰 적을 수 있습니다.

~~~python
print("hello")
print("Typora")
~~~

### 표

타이포라에서는 도표도 만들 수 있습니다.

~~~markdown
| 첫 번째 제목 | 두 번째 제목 |
~~~

위 처럼 생성 후 표의 크기를 조절할 수 있습니다.

| 언어    | 단어  |
| ------- | ----- |
| Korean  | 물    |
| English | Water |



### 각주

footnote를 이렇게 넣을 수 있습니다(맨 밑을 한 번 확인하세요).[^footnote]

### 수평선

'***'와 '---'을 사용해서 수평선을 그을 수 있습니다. 이것 말고 명령어인 '<hr/>'이가 있습니다.

***

---

<hr/>

~~~markdown
***
---
<hr />
~~~

### 링크

#### Reference Link

[github][id]는 저의 guthub 주소입니다.

링크를 타고 들어가시려면 cmd(ctrl)을 누르고 클릭하시면 됩니다.

~~~markdown
[링크 이름][변수]
[변수]: 링크 주소
위의 형식을 취합니다. [변수]는 각주와 비슷하게 맨 밑에 적는 것이 좋습니다.
~~~



#### Internal Link

[github](https://github.com/YoungHoonKo/Developement-Study.git '깃허브') 이것도 제 github 주소입니다.

~~~markdown
[링크이름](링크주소'제목')의 형식을 취합니다.제목은 적어도, 안 적어도 됩니다.
~~~

### URL

<https://github.com/YoungHoonKo/Developement-Study.git>

~~~markdown
위 처럼 주소만 보여주는 url 주소는 <http://www.example.com>의 형식을 취합니다.
~~~

### 이미지

![강아지](/assets/img/screenshot/강아지.JPEG)

~~~markdown
![사진 이름](사진 주소) 이렇게 입력해주시면 위 처럼 사진을 띄울 수 있습니다.
~~~

### 강조

*안녕하세요*

_안녕하세요_

위 글씨는 이탤릭체로 약간 기울어진 모습을 볼 수 있습니다.

~~~markdown
*내용*
_내용_
~~~

### 굵은 글씨

**안녕하세요**

__안녕하세요__

글씨를 굵게 강조하고 싶을 때 사용하면 됩니다.

~~~markdown
**내용**
__내용__
~~~

### 코드

~~~markdown
코드블럭과는 다르게 사용됩니다.
마크다운 코드블럭으로 설명할 수 없어서 cmd(ctrl)+/를 눌러서 소스 코드를 확인해보시기 바랍니다.
~~~

`print('hello')` 이렇게 사용합니다.

### 지움 표시

~~실수로 쓴 글자~~~ 이렇게 글자에 줄을 그을 수 있습니다.

물결 두 개를 글자 양옆에 적어 주시면 됩니다.

### 밑줄

<u>글자</u>

 '<u></u>'태그를 사용하면 밑줄을 그을 수 있습니다.태그 사이에 밑줄 그을 내용을 입력하시면 됩니다.

### 이모티콘

:smile: 

': smile:'이런 식으로 : 뒤에 이모티콘 표정과 관련된 문자를 입력하거나 스크롤 해서 찾을 수 있습니다.



[^footnote]: 각주

[id]: https://github.com/YoungHoonKo	"깃허브 주소"